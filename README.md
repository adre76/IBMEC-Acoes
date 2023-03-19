### PROJETO APLICADO: ANÁLISE PREDITIVA E VANTAGEM COMPETITIVA
**Professor:** Sergio Monteiro

------------

### Trabalho 2 - Análise preditiva e otimização de escolha de ações
------------

**Aluno:** André Luís dos Reis Pereira   **Matrícula:** 202205179109

**Curso:** MBA em BI & Data Science   **Campus e Turno:** Barra/Noite

------------

#### **Descrição:**
Este trabalho tem como objetivo construir uma aplicação Python utilizando recursos de aprendizado de máquina para prever valores de 10 ações (livre escolha) e utilizar os valores preditos em uma data futura específica em uma função de otimização que escolherá apenas 3 ações para investimento de forma a minimizar os riscos de perda.

O aprendizado de máqiuna utilizado foi baseado na arquitetura LSTM. Trata-se de um modelo de rede neural recorrente (RNN) especializada em classificar, processar e prever séries temporais.

Para calcular a maximização dos resultados, que envolve um problema de otimização combinatória entre os valores das ações de forma a escolher as melhores opções, foi utilizada a função [maximize] do pacote MIP.

As datas de amostragem dos dados das ações foi definida em:
Início: 01/01/2021
Fim: 01/03/2023

A data de previsão foi configurada em 30/06/2023

Todas as datas estão fixas na elaboração do programa, mas nada impede que outras datas sejam configuradas pelo usuário, bastando alterá-las na célula 5 do notebook Projeto.ipynb

#### **Considerações:**
Apesar de ser um trabalho cujo objetivo é apenas demonstrar a funcionalidade de predição e otimização, criei uma interface visual para a escolha das ações, para tornar mais fácil o processo de entrada de dados.