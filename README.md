# Random Forest com Scikit-Learn e Vega Datasets

Notebook de atividade de Inteligência Artificial e Aprendizagem de Máquina da graduação em Ciência da Computação. O material explora classificação com Random Forest e apresenta um exemplo usando o conjunto Iris da biblioteca `vega_datasets`.

## Autores

- **Nicolas Mariano da Silva** — GitHub: [@nickmds1](https://github.com/nickmds1) — RA: `0033311`
- **Pedro Henrique Isamu Fagundes de Souza Tsukahara Yoshissaro** — GitHub: [@knutzin](https://github.com/knutzin) — RA: `00330820`

## O que o notebook aborda

- Preparação dos dados Iris e inspeção de valores ausentes e distribuição das classes.
- Separação estratificada entre treino e teste.
- Treinamento de `RandomForestClassifier` do Scikit-Learn.
- Avaliação por acurácia, precisão, revocação, F1-score e matriz de confusão.
- Visualização da importância das variáveis.
- Contexto adicional de Random Forest, Titanic e métodos ensemble no material original da aula.

## Como executar

1. Abra `RandomForest_Vega_Datasets.ipynb` no Google Colab ou Jupyter Notebook.
2. Instale as dependências com `pip install -r requirements.txt`.
3. Execute as células em ordem.

A seção Iris usa `from vega_datasets import data` e `data.iris()`. As partes opcionais do Titanic que baixam dados do Kaggle exigem configuração de credenciais/API do Kaggle no ambiente do Colab.

## Dependências

As dependências listadas cobrem os imports usados no notebook completo. Para executar somente o exemplo Iris, bastam `vega_datasets`, `scikit-learn`, `pandas`, `numpy` e `matplotlib`.

## Observação

Os resultados de avaliação são gerados ao executar o notebook. A interpretação deve considerar as saídas da execução e a separação entre dados de treino e teste.
