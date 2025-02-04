# RegressaoPrevisao_CasoDeEstudo_PrecoCasasBoston
Regressão linear: previsão de preços de casas em Boston

Bem-vindo(a) ao estudo de caso sobre regressão linear. Usaremos os dados de preços de casas em Boston para o exercício de construção de um modelo de regressão.

# Declaração do problema
O problema em questão é prever os preços das casas de uma cidade ou subúrbio com base nas características da localidade fornecidas. No processo, precisamos identificar os recursos mais importantes no conjunto de dados. Devemos empregar técnicas de pré-processamento de dados e construir um modelo de regressão linear que preveja os preços para nós.

# Informações dos dados
Cada registro no banco de dados descreve um subúrbio ou cidade de Boston. Os dados foram retirados da Standard Metropolitan Statistical Area (SMSA) de Boston em 1970. Informações detalhadas sobre os atributos podem ser encontradas abaixo.

# Informações dos atributos (em ordem):
CRIM: taxa de criminalidade per capita por cidade.

ZN: proporção de terras residenciais zoneadas para lotes com mais de 25.000 pés quadrados (sq.ft.).

INDUS: proporção de acres de negócios não varejistas por cidade.

CHAS: variável fictícia do rio Charles (se o lote faz fronteira com o rio, é igual a um; caso contrário, zero).

NOX: concentração de óxido nítrico (partes por 10 milhões).

RM: número médio de cômodos por residência.

AGE: proporção de unidades ocupadas pelo proprietário, construídas antes de 1940.

DIS: distâncias ponderadas em relação a cinco centros de emprego em Boston.

RAD: índice de acessibilidade às rodovias radiais.

TAX: valor total da taxa de imposto sobre a propriedade por 10.000 dólares.

PTRATIO: proporção entre alunos e professores por cidade.

LSTAT: porcentagem da população de mais baixo status.

MEDV: valor da mediana de casas ocupadas pelo proprietário em milhares de dólares.

# Definição de melhor modelo para Previsão do MEDV

Para definirmos o melhor modelo, nós exploramos o serviço de ML Automatizado no Azure Machine Learning.
Na ferramenta nós subimos o banco Boston.csv seguindo as orientações do site: https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html
Fizemos algumas alterações em relação as orientações do site da Microsoft, como usar todos os modelos disponíveis (duranção de 6 horas para treinamento dos modelos) e também não configuramos os limites.
Com isto, nesta configuração, o melhor modelo foi aquele que utilizou o algoritmo VotingEnsemble, com "Erro de quadrado de média de raiz normalizado" de 0.06007.
Anexamos os arquivos gerados neste laboratório (JSON, PYTHON) aqui neste repositório.
