# AnaliseExploratoria-DataWrangling-ECommerce
Projeto em 3 partes feito no curso Big Data Real-Time Analytics com Python e Spark da Data Science Academy, onde são feitos Análise Exploratória de Dados, Engenharia de Atributos e Pré-Processamento de Dados para um conjunto de dados de um e-commerce fictício utilizando linguagem Python e os pacotes NumPy, Pandas, SciKit Learn, Matplotlib e Seaborn.


Na Análise Exploratória de Dados, os dados são carregados e é feita, inicialmente, uma visão geral do conjunto de dados, como seu formato, além de informações sobre as colunas presentes. Após isso, as variáveis são divididas em dois grupos, as numéricas e as categóricas. Ao fazer esta separação, é importante considerarmos a informação presente, e não apenas o formato do dado. Por exemplo, temos uma variável "entregue_no_prazo", com valores 0 e 1, o que pode indicar, a princípio, que temos uma variável numérica. Porém, os valores 0 e 1 representam entregas no prazo e em atraso, respectivamente, ou seja, trata-se de uma variável categórica, mesmo que representada por números.

Variáveis numéricas e categóricas podem ser resumidas com o uso da função describe(), porém, como mostrado no notebook, os parâmetros mostrados pelo métodos são diferentes em variáveis numéricas e categóricas.

As variáveis ainda são observadas graficamente. Os principais tipos de gráficos usados na análise univariada exploratória de dados são:

-Variáveis numéricas: histogramas, box plots, dist plots, violin plots.

-Variáveis categóricas: count plots.

Para análises bivariadas, podemos usar mapas de correlação e pair plots.
