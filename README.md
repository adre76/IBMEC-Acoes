### PROJETO APLICADO: ANÁLISE PREDITIVA E VANTAGEM COMPETITIVA
**Professor:** Sergio Monteiro

------------

### Trabalho 2 (70%) - Análise preditiva e otimização de escolha de ações
------------

**Aluno:** André Luís dos Reis Pereira   **Matrícula:** 202205179109

**Curso:** MBA em BI & Data Science   **Campus e Turno:** Barra/Noite

------------

#### **Descrição:**
Este trabalho tem como objetivo construir uma aplicação Python utilizando recursos de aprendizado de máquina para prever valores de 10 ações (livre escolha) e utilizar os valores preditos em uma data futura específica em uma função de otimização que escolherá apenas 3 ações para investimento de forma a minimizar os riscos de perda.

$$ \max \ z= R_{1}\ x_{1} + R_{2}\ x_{2} + R_{3}\ x_{3} + R_{4}\ x_{4} + R_{5}\ x_{5} + R_{6}\ x_{6} + R_{7}\ x_{7} + R_{8}\ x_{8} + R_{9}\ x_{9} + R_{10}\ x_{10}  \\ $$

$$ \mbox{sujeito a:}  \\ \\ \\ \\ \ x_{1} + \ x_{2} + \ x_{3} + \ x_{4} + \ x_{5} + \ x_{6} + \ x_{7} + \ x_{8} + \ x_{9} + \ x_{10} = 3 $$

$$ \ x_{i} \in ( 0,1 ), i = 1,...,10 $$

O aprendizado de máqiuna utilizado foi baseado na arquitetura LSTM. Trata-se de um modelo de rede neural recorrente (RNN) especializada em classificar, processar e prever séries temporais.
Para cada ativo observado, são geradas três informações específicas para analisar a eficácia do modelo treinado:
- Performance do modelo: Foi utilizada a métrica MSE (erro quadrático médio). Para o valor obtido, quanto mais próximo de zero, melhor é o desempenho do modelo treinado.
- Gráfico de cálculo de erro ao longo do treinamento.
- Gráfico comparando os valores reais da base de treinamento com os valores obtidos através do modelo treinado utilizando as datas da base de treinamento.

Para calcular a maximização dos resultados, que envolve um problema de otimização combinatória entre os valores das ações de forma a escolher as melhores opções, foi utilizada a função [maximize] do pacote MIP.

As datas de amostragem dos dados das ações foi definida em:
Início: 01/01/2021
Fim: 01/03/2023

A data de previsão foi configurada em 30/06/2023

Todas as datas estão fixas na elaboração do programa, mas nada impede que outras datas sejam configuradas pelo usuário, bastando alterá-las na célula 5 do notebook Projeto.ipynb

#### **Considerações:**
Apesar de ser um trabalho cujo objetivo é apenas demonstrar a funcionalidade de predição e otimização, criei uma interface visual para a escolha das ações, para tornar mais fácil o processo de entrada de dados.

#### **Arquivos:**
- Projeto.ipynb: Notebook com o programa descrito acima.
- README.md: Arquivo Markdown com a descrição do trabalho.
- requests.txt: Arquivo com os pacotes (nas suas versões utilizadas para a elaboração deste trabalho), a fim de garantir sua execução mesmo com a evolução das bibliotecas utilizadas no Projeto.ipynb. A preparação do ambioente deve ser feita executando o comando [pip3 install -r requests.txt] no prompt de comando.
