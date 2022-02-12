# Otimizador ope-source para simulação de eventos discretos


O objetivo desse trabalho foi desenvolver uma ferramenta open-source de  Otimização para simulação de eventos discretos. Para auxiliar projetos na área de otimização via simulação, tanto para empresas que não possuem softwares comerciais e para pesquisadores da área. 

# Visão geral do projeto

O funcionamento do otimizador se utiliza de um algoritmo genético como meta-heurística, uma rede neural para criar o metamodelo, assim acelerando o tempo de execução do código. A forma de conectar o modelo de siulação com o código de otimização ocorre via arquivos externos (.txt), para disponibilizar maior flexibilidade na linguagens que podem ser usadas para a modelagem computacional, atualmente pode ser utlizado python, R, C e C++ 


![fluxo_software](https://user-images.githubusercontent.com/48968629/153720015-0f57b7f3-c947-41c5-bcd4-0c8528dd0e0a.jpg)  


# Como utilizar o projeto 

Antes de iniciar o uso do otimizador, deve-se adaptar o código da simulação com a leitura e escrita dos arquivos .txt.
o formato dos arquivos de entrada e de saída precisão seguir essa estrutura. Primeira linha com os nomes das variavéis separadas por vírgula e, na linha de baixo os valores de cada uma das variáveis em ordem, também separada por vírgula.


Para acessar otimizador:

Pré-requisitos: python 3.9 

clonar repositório em uma pasta vazia:
git clone https://github.com/darvenlima/OtimizadorDES

Após a clonagem do do repositório e com o python 3.9 installado, é necessario fazer a instalação das bibliotecas usadas no código antes da primeira utilização. Todas as instalações necessárias estão no arquivo bibliotecas.txt. Com a instalação completa, pode realizar a execução do código com o comando:

python .\interface.py

