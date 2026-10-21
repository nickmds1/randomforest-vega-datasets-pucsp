# Random Forest com Scikit-Learn e Vega Datasets: Stocks

Atividade de Inteligência Artificial e Aprendizagem de Máquina da graduação em Ciência da Computação. O notebook explora **regressão com `RandomForestRegressor`** usando o conjunto **Stocks** do pacote `vega_datasets`.

O conjunto contém 560 observações mensais de cinco empresas, entre 2000 e 2010, com as colunas `symbol` (ticker), `date` (data) e `price` (preço). A tarefa didática é estimar o preço mensal a partir do ticker, da data e de preços observados em meses anteriores.

## Autores

- **Nicolas Mariano da Silva** — GitHub: [@nickmds1](https://github.com/nickmds1) — RA: `0033311`
- **Pedro Henrique Isamu Fagundes de Souza Tsukahara Yoshissaro** — GitHub: [@knutzin](https://github.com/knutzin) — RA: `00330820`

## O que o notebook aborda

- Carregamento de `data.stocks()` e inspeção dos dados.
- Visualização da série histórica de preços por empresa.
- Criação de atributos temporais e defasagens (`lag_1`, `lag_3` e média móvel dos três meses anteriores).
- Separação cronológica entre treino e teste para evitar usar dados futuros no treinamento.
- Treinamento de `RandomForestRegressor` e comparação com uma previsão de referência que repete o preço do mês anterior.
- Avaliação por MAE, RMSE e R², gráficos de valores observados e previstos e importância das variáveis.
- Discussão das limitações de um exercício didático de previsão com dados históricos.

## Como executar

1. Abra `RandomForest_Vega_Datasets.ipynb` no [Google Colab](https://colab.research.google.com/) ou no Jupyter Notebook.
2. Instale as dependências com `pip install -r requirements.txt`.
3. Execute as células na ordem. O notebook carrega os dados com `from vega_datasets import data` e `data.stocks()`.

## Dependências

Veja `requirements.txt`. São usadas `vega_datasets`, `scikit-learn`, `pandas`, `numpy` e `matplotlib`.

## Observação

O conjunto Stocks cobre apenas dados históricos de 2000 a 2010 e é usado para fins educacionais. A avaliação é um experimento de previsão temporal e **não deve ser interpretada como recomendação de investimento**. Os resultados são produzidos ao executar o notebook.

## Fonte dos dados

- [Vega Datasets — Stocks](https://vega.github.io/vega-datasets/datasets/stocks/)
