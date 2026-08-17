# Introdução a Machine Learning

Material de aula introdutória de Machine Learning usando o dataset **Online Shoppers Intention**.

Professor: **Jaime Teixeira** - [@jaimejrs](https://github.com/jaimejrs)

## Objetivo

Este projeto apresenta, de forma didática, o fluxo básico de um experimento de Machine Learning:

1. carregar e conhecer um dataset real;
2. explorar variáveis e estatísticas descritivas;
3. identificar a variável-alvo;
4. preparar dados categóricos e numéricos;
5. criar um modelo baseline;
6. treinar uma Árvore de Decisão;
7. visualizar a árvore;
8. treinar um Random Forest;
9. comparar os modelos com métricas de classificação;
10. interpretar resultados e variáveis importantes.

## Dataset

O notebook utiliza o dataset **Online Shoppers Purchasing Intention**, disponível publicamente pela UCI Machine Learning Repository.

A pergunta norteadora do experimento é:

> Como podemos prever se uma sessão de e-commerce terminará em compra?

A variável-alvo do projeto é `Compra`, que indica se a sessão terminou ou não em compra.

## Estrutura do Repositório

```text
.
├── assets/
│   ├── fonts/
│   └── img/
├── notebooks/
│   └── 1_experimento_online_shoppers_colab.ipynb
├── slides/
│   └── apresentacao_aula.html
├── requirements.txt
└── README.md
```

## Como Usar

### Google Colab

A aula prática foi pensada para execução no Google Colab.

1. Abra o notebook `notebooks/1_experimento_online_shoppers_colab.ipynb`.
2. Faça upload para o Google Colab ou abra pelo GitHub.
3. Execute as células em ordem.

Link direto pelo Colab:

[Abrir notebook no Colab](https://colab.research.google.com/github/jaimejrs/intro-ml/blob/main/notebooks/1_experimento_online_shoppers_colab.ipynb)

### Ambiente Local

Crie e ative um ambiente virtual:

```bash
python -m venv .venv
```

No Windows:

```bash
.venv\Scripts\activate
```

Instale as dependências:

```bash
pip install -r requirements.txt
```

Abra o Jupyter:

```bash
jupyter lab
```

## Materiais

- Slides: `slides/apresentacao_aula.html`
- Notebook: `notebooks/1_experimento_online_shoppers_colab.ipynb`
- Assets visuais: `assets/img/`

## Modelos Utilizados

O notebook compara três abordagens:

- **Baseline**: `DummyClassifier`, prevendo a classe majoritária;
- **Árvore de Decisão**: modelo interpretável e visual;
- **Random Forest**: conjunto de várias árvores para maior estabilidade.

As métricas usadas na comparação são:

- acurácia;
- precisão da classe `comprou`;
- recall da classe `comprou`;
- F1-score da classe `comprou`;
- ROC AUC.

