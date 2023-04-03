# AnaliseExploratoria-DataWrangling-ECommerce
Projeto em 3 partes feito no curso Big Data Real-Time Analytics com Python e Spark da Data Science Academy, onde são feitos Análise Exploratória de Dados, Engenharia de Atributos e Pré-Processamento de Dados para um conjunto de dados de um e-commerce fictício utilizando linguagem Python e os pacotes NumPy, Pandas, SciKit Learn, Matplotlib e Seaborn.
## Análise Exploratória de Dados
Na Análise Exploratória de Dados, os dados são carregados e é feita, inicialmente, uma visão geral do conjunto de dados, como seu formato, além de informações sobre as colunas presentes. Após isso, as variáveis são divididas em dois grupos, as numéricas e as categóricas. Ao fazer esta separação, é importante considerarmos a informação presente, e não apenas o formato do dado. Por exemplo, temos uma variável "entregue_no_prazo", com valores 0 e 1, o que pode indicar, a princípio, que temos uma variável numérica. Porém, os valores 0 e 1 representam entregas no prazo e em atraso, respectivamente, ou seja, trata-se de uma variável categórica, mesmo que representada por números.

Variáveis numéricas e categóricas podem ser resumidas com o uso da função describe(), porém, como mostrado no notebook, os parâmetros mostrados pelo métodos são diferentes em variáveis numéricas e categóricas.

As variáveis ainda são observadas graficamente. Os principais tipos de gráficos usados na análise univariada exploratória de dados são:

-Variáveis numéricas: histogramas, box plots, dist plots, violin plots.

-Variáveis categóricas: count plots.

Para análises bivariadas, podemos usar mapas de correlação e pair plots.

Na segunda parte da análise, são dados exemplos de perguntas de negócio a serem respondidas utilizando somente análise exploratória de dados.

## Engenharia de Atributos

A Engenharia de Atributos consiste na trasnformação dos dados em atributos a serem utilizados no processo de aprendizado de máquina, de modo a tornar o modelo mais eficiente.

Antes da Engenharia de Atributos em si, é feita a análise de dados ausentes e dados extremos, ou outliers, de modo a garantir que estes dados não estejam presentes no conjunto final de dados. Além disso, é importante observarmos se as variáveis categóricas estão balanceadas, ou seja, com um número de observações similar. Isso é importante para garantir que os modelos de Machine Learning a serem utilizados aprendam igualmente todas as categorias, e não apresentem resultados tendenciosos.

Na Engenharia de Atributos, vemos duas técnicas, a Feature Selection e a Feature Extraction. 
