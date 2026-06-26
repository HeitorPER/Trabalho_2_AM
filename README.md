# Aprendizado Nao Supervisionado aplicado a Exoplanetas Confirmados

Projeto 02 da disciplina Aprendizado de Maquina I. O objetivo e explorar o catalogo de exoplanetas confirmados da NASA usando exclusivamente tecnicas nao supervisionadas para descobrir tipos de planeta, detectar anomalias e extrair regras de associacao entre parametros fisicos e orbitais.

## Tecnicas aplicadas

- Reducao de dimensionalidade via PCA
- Agrupamento com K-Means e DBSCAN
- Deteccao de anomalias com Isolation Forest e Local Outlier Factor
- Extracao de regras com Apriori
- Regressao linear descritiva sobre os componentes principais

## Requisitos

- Python 3.9 ou superior
- Jupyter Notebook ou JupyterLab

## Instalacao das dependencias

```
pip install numpy pandas matplotlib seaborn scikit-learn mlxtend jupyter
```

## Como rodar

1. Clone ou baixe o repositorio e entre na pasta do projeto.

2. Certifique-se de que o arquivo `confirmed_exoplanents_2024_December.csv` esta na mesma pasta que o notebook.

3. Inicie o Jupyter:

```
jupyter notebook
```

4. No navegador, abra o arquivo `Analise_exoplanetas.ipynb`.

5. Execute todas as celulas em ordem: no menu superior clique em **Kernel > Restart & Run All**.

## Dataset

O arquivo `confirmed_exoplanents_2024_December.csv` contem dados do NASA Exoplanet Archive referentes a dezembro de 2024, obtidos via Kaggle. O notebook espera encontrar esse arquivo no mesmo diretorio em que e executado.

Apos a limpeza de valores ausentes, o pipeline trabalha com aproximadamente 3.686 planetas e 12 variaveis numericas (periodo orbital, raio, massa, semieixo maior, excentricidade, temperatura de equilibrio, fluxo de insolacao, temperatura estelar, raio estelar, massa estelar, metalicidade e distancia).
