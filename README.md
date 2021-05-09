
# Análise Descritiva e Preditiva dos Mecanismos de Ação Celulares

<img src='https://github.com/maicon-reis/imersao-dados-desafio-final/blob/main/Capa%20para%20o%20Readme.jpg' height=600 width=900></img>

**Projeto:** Projeto de conclusão da 3ª Edição da Imersão Dados  da Alura  busca desenvolver um estudo de Data Science com análise exploratória e desenvolvimento de um modelo de machine learning para auxiliar na descoberta de novos medicamentos.

**Dados:** A base de dados está dividida em dois Datasets, o primeiro contém as informações referentes ao experimento, forma de tratamento, tempo, dose e composto utilizado além da assinatura celular. Já o segundo conjunto de dados contém os mecanismos de ação decorrentes da assinatura celular.

**Objetivo/Tarefas:** O projeto foi dividido em quatro objetivos, sendo três descritivos e um decorrente da utilização de um modelo de machine learning:

1. Qual mecanismo de ação foi mais ativado?
2. Os tipos de tratamento “com_controle” ativaram algum mecanismo de ação?
3. Algum tipo de tratamento “com_droga” não ativou nenhum mecanismo de ação?
4. Caso não seja identificado se a utilização do composto se derivou da dose D1 ou D2, qual a probabilidade de realizar a identificação do tipo da dose através do conjunto de dados? 

**Aspectos dos dados:** 

Nesse projeto serão utilizados dois datasets, sendo o primeiro é dividido em três grupos de dados:

1. **Quatro colunas com informações categóricas:** Além do 'id' temos [1] **tratamento**, se a amostra foi submetida ao composto ou é uma amostra de controle; [2] **droga** que descreveve o tipo de tratamento que cada amostra foi submetida; [3] **tempo**, que cada amostra foi submetida ao tratamento e [4] **dose**, que indica a dosagem utilizada no tratamento;
2. **As expressões gênicas (genes)** que são nomeadas como "g-" seguido de um número sequencial;
3. **As de viabilidades celulares (células)** nomeadas como "c-" seguido de um número sequencial.

Tanto as expessões gênicas quanto as viabilidade celulares contém resposta simultânea de diferentes linhagens celulares à utilização de determinado composto. Cada linha, contendo essas respostas é chamado de **assinatura celular**.

Os valores numéricos contidos nas colunas g_ correspondem ao resultado do caminho da informação biológica com destino à proteína, pela ativação ou não de um mecanismo de ação. Já o valor das colunas c_ é a viabilidade celular, ou seja, o quanto as células sobreviveram ou não à exposição do composto.

Dessa forma cada linhagem celular, seja expressões gênicas ou de viabilidade celular, foi exposta a um determinado a um composto ou situando-se como amostra de controle, por um período de tempo, a uma determinada dosagem.

Já o segundo dataset é composto por **mecanismos de ação** do composto, onde cada linha é resultado de um experimento na primeira base de dados. Em resumo, como cada linha da base de dados é o resultado de um experimento na base dedados, quando o mecanismo de ação é ativado ele recebe o valor 1.

>"Em farmacologia, a expressão mecanismo de ação refere-se à intereção bioquímica através da daqual uma droga produz um efeito farmacológico.Um mecanismo de ação usualmente inclui menção de um "alvo" molecular específico no qual a droga liga-se, tal como uma enzima ou receptor."

Nas colunas, além do **id**, são compostas por elementos que potencializam ou bloqueiam o receptor ou inibidores, utilizados para enzimas.

Verifica-se que as colunas são compostas por nomes terminados com "_inhibitor" (suprimem ou inibem a ação sobre uma enzima), bem como por "_agonist" e "_antagonist" (estes bloqueiam o receptor, enquanto aqueles ativam ou potencializam o receptor).

**Conclusões:**
1. O mecanismo de ação mais ativado foi o 'nfkb_inhibitor' com 832 ativações;
2. Como esperado o tipo de tratamento marcado 'com_controle', que é um valor de referência, não ativou nenhum mecanismo de ação;
3. Houve 7501 amostras com tipo de tratamento marcadas "com_droga" que não ativaram nenhum mecanismo de controle;
4. Caso haja a necessidade de identificar o tipo de dose a partir da base de dados, há uma taxa de acurácia acima de 90% de chances de identificação.

**Leitura Complementar**

1. [Conceito de Mecanismo de Ação](https://pt.wikipedia.org/wiki/Mecanismo_de_a%C3%A7%C3%A3o)
2. [Fluoroquilononas: Mecanismos de Ação e Resistência](https://www.youtube.com/watch?v=hyjKWF7yvrE)
3. [Drug discovery: passado, presente e futuro](https://docs.google.com/document/d/10EhrQBChlyYIcff3to7PrCQi5HcNk2r-zd2ZCKPtcz8/edit)
4. [Expressão gênica: o caminho da informação biológica](https://drive.google.com/file/d/1VNP08ffCiGD8cqaBkdHATWSX8Yxfm3dj/view)


