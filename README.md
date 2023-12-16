# Projeto: Boosting para Classificação no Jogo da Velha

## Introdução

Este projeto tem como objetivo implementar o algoritmo de Boosting, mais especificamente o AdaBoost, para aprimorar a classificação no jogo da velha. Utilizaremos um conjunto de classificadores de árvore de decisão para combinar modelos fracos e reduzir o viés do conjunto.

## Conjunto de Dados

O conjunto de dados utilizado neste trabalho é o "tic-tac-toe" que contém informações sobre partidas de jogo da velha. O objetivo é prever a classificação final do jogo (vitória ou derrota). Os atributos são categóricos, representando as posições do tabuleiro e a jogada do primeiro jogador. O dataset pode ser encontrado em [Tic-Tac-Toe End Game Dataset UCI - Kaggle](https://www.kaggle.com/datasets/aungpyaeap/tictactoe-endgame-dataset-uci?datasetId=207741&searchQuery=bag).

## Implementação

O código está disponível no arquivo [notebook.ipynb](notebook.ipynb) e inclui:

- Importação de bibliotecas necessárias.
- Visualização dos dados, incluindo histogramas comparativos.
- Preparação dos dados, substituindo valores categóricos e dividindo em conjuntos de treinamento e teste.
- Treinamento de um modelo simples de Árvore de Decisão e otimização dos hiperparâmetros usando Grid Search.
- Implementação do algoritmo de Boosting (AdaBoost) utilizando um conjunto de classificadores de árvore de decisão.
- Avaliação dos modelos por meio de validação cruzada (5 partições) e métricas de desempenho.
- Visualização de matrizes de confusão, curva ROC e taxa de aprendizado ao longo das iterações.

## Avaliação dos Modelos

Os resultados foram analisados considerando métricas como acurácia, precisão, revocação e F1-Score. O modelo com Boosting mostrou um desempenho superior, reduzindo falsos positivos e falsos negativos em comparação com o modelo simples de Árvore de Decisão.

## Conclusão

A implementação do algoritmo de Boosting demonstrou ser eficaz para aprimorar a classificação no jogo da velha em comparação com um modelo simples de Árvore de Decisão. A técnica de Boosting oferece uma abordagem eficiente para combinar modelos fracos e melhorar a precisão do classificador.

## Referências

- [Scikit-learn Documentation](https://scikit-learn.org/)
- [UC Irvine Machine Learning Repository - Tic-Tac-Toe Endgame](https://archive.ics.uci.edu/dataset/101/tic+tac+toe+endgame)
- [Tic-Tac-Toe End Game Dataset UCI - Kaggle](https://www.kaggle.com/datasets/aungpyaeap/tictactoe-endgame-dataset-uci?datasetId=207741&searchQuery=bag)
