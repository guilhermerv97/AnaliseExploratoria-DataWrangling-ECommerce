# AnaliseExploratoria-DataWrangling-ECommerce


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

Na Engenharia de Atributos, vemos duas técnicas, a Feature Selection e a Feature Extraction. Na Feature Selection, observamos as variáveis de entrada em busca de entender quais são as mais relevantes para o cálculo da variável alvo, e, com isso, retirar as variáveis menos importantes. Com isso, podemos reduzir o custo computacional e, muitas vezes, melhorar a performance dos modelos. Na Feature Extraction, criamos atributos novos a partir de atributos já existentes, para, com isso, diminuir o número total de variáveis. No notebook, são explorados alguns exemplos.

A partir do uso destas técnicas, criamos um novo dataset, que será utilizado na etapa de pré-processamento de dados.

## Pré-Processamento de Dados
No pré-processamento de dados, realizamos a preparação dos dados para modelos de aprendizado de máquina. Neste notebook, há um enfoque na codificação dos dados, convertendo dados categóricos e em formato de texto para dados numéricos, que podem, assim, serem utilizados para modelagem matemática. Para isso, são utlizadas netste notebook técnicas como Label Encoding, One-Hot Encoding e Feature Scaling.

O Label Encoding é uma técnica, normalmente utilizada para variáveis categóricas ordinais, que envolve a troca das categorias por valores numéricos correspondentes, podendo ser feito manualmente através de dicionários em Python, ou através do método LabelEncoder, do pacote preprocessing do SciKit Learn.

O One Hot-Encoding, por sua vez, é normalmente utilizado para variáveis categóricas nominais, e consiste na quebra de uma variável em variáveis dummy para cada categoria, com valores de 0 ou 1. Com isso, o número de variáveis aumenta, o que pode tornar esta técnica inviável no caso de variáveis com um número muito elevado de categorias.

Por fim, o Feature Scaling é o tratamento de variáveis numéricas, para garantir que todas possuam valores em faixas semelhantes, uma vez que valores em escalas muito diferentes podem tornar o modelo preditivo tendencioso. Para isso, são feitas a Normalização, em que o valor mínimo da variável é convertido para 0 e o máximo é 1, ou a Padronização, que converte os valores para um conjunto com média 0 e desvio padrão 1. A Normalização permite observar a diferença dos valores para o máximo e mínimo, porém a Padronização permite, por exemplo, a observação de valores discrepantes, uma vez que não estabelece limites para os dados. Ambos são feitos usando o pacote preprocessing do SciKit Learn, e as funções MinMaxScaler() e StandardScaler(), respectivamente.




