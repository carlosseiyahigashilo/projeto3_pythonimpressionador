# projeto3_pythonimpressionador
Projeto de Ciência de Dados desenvolvido no Curso Python Impressionador, ministrado pela Hashtag Treinamentos.


## 1. Objetivo
O objetivo deste projeto é prever o preço de aluguel de um imóvel no Rio de Janeiro, de acordo com a plataforma Airbnb.

## 2. Arquivos
A pasta contém os seguintes arquivos:
1. <b>Projeto 3 - AirBnb Rio de Janeiro.ipynb</b> -> arquivo Jupyter em que foi realizado praticamente todo o projeto, desde a etapa de importação dos dados, data cleaning, Análise Exploratória, feature engineering e treino dos modelos, até o preparo para o Deploy. Nele, está documentado também todas as lógicas e conceitos que foram adotados para a elaboração do projeto.
2. <b>DeployProjetoAirbnb.py</b> -> é o arquivo que aproveita e utilizado modelo gerado no arquivo "Projeto 3 - AirBnb Rio de Janeiro.ipynb" para realizar a previsão. Ele deve ser rodado no Prompt do Anaconda utilizando-se o comando "streamlit run DeployProjetoAirbnb.py", em que se abrirá uma janela no navegador padrão do usuário para realizar os inputs necessários para o modelo fazer a sua previsão.
3. [ARQUIVO NÃO FOI COLOCADO DEVIDO A LIMITE DE ESPAÇO NO GITHUB] <b>modelo.joblib</b> -> é o modelo "vencedor" após os treinos realizados (ExtraTrees), e que é utilizado no arquivo "DeployProjetoAirbnb.py"
4. [ARQUIVO NÃO FOI COLOCADO DEVIDO A LIMITE DE ESPAÇO NO GITHUB] <b>dataset</b> -> é uma subpasta que contém dados desde abril/19 até maio/20, com informações de imóveis do Airbnb (a base foi extraída do Kaggle)
5. [ARQUIVO NÃO FOI COLOCADO DEVIDO A LIMITE DE ESPAÇO NO GITHUB] <b>dados.csv</b> -> é o arquivo csv resultado da exportação da base depois que é realizado todo o data cleaning/feature engineering, para que não seja necessário repetir todo o processo totalmente do zero caso seja necessário.
6. <b>primeiros_registros.csv</b> -> arquivo csv auxiliar para verificar os 1000 primeiros registros, e realizar uma análise qualitativa de todas as colunas da tabela original (caso queira ver com maiores detalhes, é explicado de forma clara e didática dentro do próprio arquivo Jupyter "Projeto 3 - AirBnb Rio de Janeiro.ipynb".

## 3. Observações importantes:
1. Ele é excelente para prever o preço de imóveis "na média", mas não é preciso quando se trata de exceções e outliers (ex: se um imóvel na praia do Leblon, que na prática é bem caro, mas o modelo previria como não tão caro quanto um imóvel com uma latitude similar, ou seja, relativamente perto, porém mais afastado da praia). 
2. O modelo final pode ser utilizado abrindo o Prompt do Anaconda, entrando na pasta do arquivo "DeployProjetoAirbnb.py", e rodando o comando "streamlit run DeployProjetoAirbnb.py". Será aberta uma interface gráfica no navegador padrão, e é possível preencher os valores para que o modelo consiga realizar as previsões. Ele retorna, no final, o preço sugerido pelo modelo de previsão.
