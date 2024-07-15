# Análise de Preços de Maçãs ao Longo do Tempo
Este projeto tem como objetivo analisar os preços de maçãs em diferentes regiões ao longo de um período de tempo, utilizando a biblioteca `numpy` para manipulação dos dados e `matplotlib` para visualização.

## Requisitos
- Python 3.6 ou superior
- Bibliotecas: `numpy`, `matplotlib`

## Dados Utilizados
Os dados são provenientes de um arquivo CSV disponível em uma URL pública: "https://raw.githubusercontent.com/alura-cursos/numpy/dados/apples_ts.csv"

## Fluxo do Projeto
1- Carregamento e Transformação dos Dados:

 - Carregamento dos dados utilizando `numpy`.
 - Transposição dos dados para facilitar a manipulação.

2- Análise dos Dados:

 - Extração das colunas de interesse (datas e preços).
 - Criação de variáveis para os preços de diferentes regiões: Moscow, Kaliningrad, Petersurg, Krasnodar e Ekaterinburg.
 - Segmentação dos dados de Moscow em diferentes anos para análise.

3- Visualização dos Dados:

 - Plotagem dos preços de Moscow ao longo dos anos.
 - Comparação dos preços de diferentes anos utilizando gráficos de linha.

4- Análise de Similaridade:

 - Utilização da função `np.allclose` para verificar a similaridade entre os preços de diferentes anos com um teto absoluto e relativo.

5- Preenchimento de Dados Faltantes:

 - Substituição de valores faltantes no conjunto de dados de Kaliningrad pela média dos valores adjacentes.

6- Regressão Linear:

 - Cálculo dos coeficientes da regressão linear para os preços de Moscow.
 - Plotagem da linha de regressão e cálculo da norma.

7- Análise de Coeficientes Aleatórios:

 - Geração de coeficientes aleatórios e cálculo da norma para cada coeficiente.
 - Salvamento dos dados gerados em um arquivo CSV.

## Execução
Para executar o projeto, siga as etapas descritas no fluxo do projeto. Certifique-se de que o arquivo `apples_ts.csv` esteja acessível na URL fornecida.