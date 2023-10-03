# Análise da Expectativa de Vida e Produto Interno Bruto
# 1. Introdução
Esse projeto investiga a relação entre a economia de um país e a expectativa de vida de seus cidadãos. É parte integrante do curso de [Data Science Foundations](https://www.codecademy.com/enrolled/paths/data-science-foundations), do Codecademy. Os objetivos desse projeto são preparar os dados, realizar análises gráficas e, por fim, explicar os resultados do estudo com base nas questões levantadas.

As ferramentas utilizadas foram:
- Python 3.0 (com as bibliotecas Pandas, Seaborn, Matplotlib, SciPy e Statsmodels)
- Jupyter Notebook
- Github

O dataset foi disponibilizado pelo Codecademy e provém dos bancos de dados da [World Health Organization](https://apps.who.int/gho/data/node.main.688) e [World Bank](https://data.worldbank.org/indicator/NY.GDP.MKTP.CD).

# 2. Briefing
Essas são as questões que esse projeto procura responder:
- A expectativa de vida tem aumentado ao longo dos anos nos seis países?
- O PIB tem aumentado ao longo dos anos nos seis países?
- Qual é a expectativa de vida média em cada país?
- Há uma relação entre expectativa de vida e PIB?

# 3. Resolução
## 3.1. Estrutura dos dados
Os atributos do conjunto de dados são:
| Atributos |	Descrição |
| --------- | --------- |
| Country | País |
| Year | Ano |
| Life expectancy at birth (years) | Expectativa de vida ao nascer, em anos |
| GDP | Produto Interno Bruto, em dólares americanos |

O conjunto de dados contém 96 linhas e 4 colunas, e traz informações sobre seis países: Chile, China, Alemanha, México, Estados Unidos da América e Zimbábue. Os dados se referem ao período entre 2000 e 2015.

## 3.2. Visualização de dados e Insights
Para responder às questões do projeto e encontrar insights sobre os dados, gerei gráficos que pudessem auxiliar na visualização dos dados para cada um dos seis países. 

_1 - Expectativa de vida ao longo dos anos_

![image](https://github.com/gabrielaguzzo/life-expectancy-and-gpd/assets/142359788/2b899e23-90e0-4e1a-85b8-739349dfa84c)

É possível observar que todos os países vem apresentando um crescimento na sua expectativa de vida, ainda que alguns países tenham apresentado algumas quedas, como Chile e México no período de 2007 a 2010.

_2 - PIB ao longo dos anos_

![image](https://github.com/gabrielaguzzo/life-expectancy-and-gpd/assets/142359788/bba5726d-5cc6-4a4f-ad93-9d60ec361083)

Todos os países apresentaram crescimento ao longo dos anos, sendo interessante observar o crescimendo do PIB de Zimbábue a partir de 2008, após uma sucessão de quedas. Todos os países, com excessão da China e Zimbábue, apresentaram uma queda no PIB em meados de 2009. Chile e México apresentam uma queda a partir de 2013/2014.

_3 - Expectativa de vida média_

![image](https://github.com/gabrielaguzzo/life-expectancy-and-gpd/assets/142359788/1e134876-eaec-43fa-bccd-99802c113222)

A Alemanha possui a maior expectativa de vida média, enquanto Zimbábue, além de apresentar a menor (cerca de 50 anos) apresenta a maior variação ao longo dos anos.

_4 - Relação entre expectativa de vida e PIB_

![image](https://github.com/gabrielaguzzo/life-expectancy-and-gpd/assets/142359788/e50a36bf-a1da-4387-99b5-a950dc4ea7f4)

Países como os EUA, o México, o Zimbabué e a Alemanha, têm relações lineares entre o PIB e a expectativa de vida. Em geral, pode-se observar um aumento do PIB e da expectativa de vida em todos os países, apresentando uma correlação positiva, que é confirmada pelos coeficientes de Pearson calculados acima de 0.90 para cada país.

## 3.3. Análise preditiva

A análise preditiva foi realizada para os países que apresentam relação linear entre PIB e expectativa de vida, quais sejam EUA, México, Zimbábue e Alemanha. Para cada país foi feita uma regressão linear e obtida a equação da reta, que possibilita encontrar qual o PIB esperado que um país alcance para determinada expectativa de vida.

# 4. Conclusões

Este projeto foi capaz de fazer algumas visualizações de dados, embora o dataset tivesse apenas 96 linhas e 4 colunas. O projeto também conseguiu responder a algumas das questões colocadas no início:
- **A expectativa de vida tem aumentado ao longo dos anos nos seis países?**

  Sim, principalmente para o Zimbábue.
  
- **O PIB tem aumentado ao longo dos anos nos seis países?**

  Sim, sendo interessante o comportamento do PIB no Zimbábue, que a partir de 2008 apresentou crescimento após um longo período de quedas.
  
- **Qual é a expectativa de vida média em cada país?**

  Gira em torno dos 70 a 80 anos, com destaque para a Alemanha como tendo a maior expectativa de vida média (cerca de 81 anos) e para o Zimbábue, com a menor expectativa de vida média (cerca de 50 anos).
  
- **Há uma relação entre expectativa de vida e PIB?**

  Sim, há uma forte correlação positiva entre expectativa de vida e PIB em todos os seis países.

# 5. Futuras pesquisas

