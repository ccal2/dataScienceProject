# Projeto de Ciência de Dados

Projeto desenvolvido para a disciplina `IF697 - Tópicos Avançados em Gerenciamento de Dados e Informação` do curso de Engenharia da Computação do CIn - UFPE no período letivo de 2020.2.


# Dataset utilizado

Esse projeto foi desenvolvido utilizando um _dataset_ que contém dados relacionados à série de livros _A Song of Ice and Fire_ (As Crônicas de Gelo e Fogo), mais conhecida pelo título do seu primeiro livro: _A Game of Thrones_ (A Guerra dos Tronos).

O arquivo `battles.csv` foi baixado diretamente de um [dataset do kaggle](https://www.kaggle.com/mylesoneill/game-of-thrones) e possui informações de várias batalhas que ocorrem durante a história.


# Parte I

[project.ipynb](./project.ipynb)

A primeira parte do projeto consiste em:
- Pré-processamento dos dados
  - Definição de tipos
  - Tratamento de dados ausentes
  - Detecção de outliers
  - Discretização
- Análise descritiva dos dados
- Testes de Hipóteses


# Parte II

A segunda parte do projeto utiliza o dataset processado na parte I para criar um classificador a partir de algoritmos de _Machine Learning_. A coluna escolhida para a classificação foi a `attacker_outcome`, que indica se o atacante venceu ou não a batalha.

Os algoritmos utilizados foram:
- Gaussian Naive Bayes
- KNN
- Decision Tree
- Random Forest

O [optuna](https://optuna.org/) foi utilizado para selecionar hiper-parâmetros para cada um desses algoritmos e depois um deles foi escolhido para ser diagnosticado e melhorado.
