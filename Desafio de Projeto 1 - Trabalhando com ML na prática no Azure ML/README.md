# Previsão da Demanda de Bicicletas com Machine Learning

**Subtítulo:** Um estudo de caso usando Regressão Linear

**Autor:** Gleybson Araújo

**Data:** 22 de março de 2024

**Resumo:**

Este projeto demonstra o desenvolvimento de um modelo de Machine Learning para prever a demanda de bicicletas em um determinado dia do ano. O modelo utiliza dados históricos de aluguel, condições climáticas e sazonalidade para prever a quantidade de bicicletas que serão alugadas.

**Introdução**

O uso de bicicletas como meio de transporte urbano tem crescido significativamente nos últimos anos. Os sistemas de compartilhamento de bicicletas oferecem uma alternativa conveniente e sustentável para o transporte individual, mas exigem um planejamento cuidadoso para garantir a disponibilidade de bicicletas para os usuários.

A previsão da demanda de bicicletas é um problema crucial para a operação eficiente dos sistemas de compartilhamento. Diversos fatores podem influenciar a demanda, como:

-   **Condições climáticas:**
    -   Temperatura
    -   Precipitação
    -   Vento
-   **Sazonalidade:**
    -   Feriados
    -   Eventos especiais
    -   Dias da semana
    -   Horário do dia

**Abordagem Metodológica**

Neste projeto, utilizamos o aprendizado por regressão linear para prever a demanda de bicicletas. A regressão linear é um modelo estatístico que mapeia uma variável dependente (demanda de bicicletas) em uma combinação linear de variáveis independentes (condições climáticas e sazonalidade).

**Modelo:**

-   Regressão Linear NRMSE

**Métricas de avaliação:**
- NRMSE (Normalized Root Mean Square Error)

**Ferramentas:**

-  Azure Machine Learning

**Dados:**

-  [Capital Bikeshare](https://capitalbikeshare.com/system-data)

**Passo a passo seguido**
- [# Explore Automated Machine Learning in Azure Machine Learning](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html)


**Resultados**
-

-   **Gráfico:**  Previsão da demanda de bicicletas vs. demanda real
		<img src="/azure/predict_true.png">
-   **Histograma:**  Diferença entre a demanda prevista e a real
		<img src="/azure/residuals.png">
-   **Teste e implatação:**
    Input:
    ```javascript
    { "Inputs": { 
	    "data": [ 
			  { 
			    "day": 1, 
			    "mnth": 1, 
			    "year": 2022, 
			    "season": 2, 
			    "holiday": 0, 
			    "weekday": 1, 
			    "workingday": 1, 
			    "weathersit": 2, 
			    "temp": 0.3, 
			    "atemp": 0.3, 
			    "hum": 0.3, 
			    "windspeed": 0.3 
			  } 
		    ] 
	    }, 
	    "GlobalParameters": 1.0 
    }
    ```
Saída: 
```javascript
{ 
	"Results": [ 
		336.50140662701915 
	] 
}
```
**Conclusões e Implicações**

-   **Resumo dos resultados e aprendizados do projeto**
Como resultado final do modelo treinado, foi previso que, aproximadamente, 336 bicicletas serão alugadas no dia 01/01/2022. 
O projeto foi uma ótima introdução ao Azure Machine Learning, de modo que o passo a passo é bem intuitivo e toda a ferramenta em si é de fácil uso.
	
-   **Discussão das implicações práticas da previsão da demanda:**
    -   Otimização da disponibilidade de bicicletas
    -   Redução de custos operacionais
    -   Melhoria da experiência do usuário
-   **Sugestões para aprimoramento do modelo e futuras pesquisas:**
    -   Utilização de outros algoritmos de aprendizado de máquina
    -   Inclusão de novas features
    -   Aplicação do modelo em outros contextos
