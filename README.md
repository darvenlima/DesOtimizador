# Otimizador open-source para simulação de eventos discretos


O objetivo desse trabalho foi desenvolver uma ferramenta open-source de  Otimização para simulação de eventos discretos. Para auxiliar projetos na área de otimização via simulação, tanto para empresas que não possuem softwares comerciais e para pesquisadores da área. 

# Visão geral do projeto

O funcionamento do otimizador se utiliza de um algoritmo genético como meta-heurística, uma rede neural para criar o metamodelo, assim acelerando o tempo de execução do código. A forma de conectar o modelo de simulação com o código de otimização ocorre via arquivos externos (.txt), para disponibilizar maior flexibilidade na linguagem que podem ser usadas para a modelagem computacional, atualmente pode ser utlizado python, R, C e C++ 


![fluxo_software](https://user-images.githubusercontent.com/48968629/153720015-0f57b7f3-c947-41c5-bcd4-0c8528dd0e0a.jpg)  


# Como utilizar o projeto 

Antes de iniciar o uso do otimizador, deve-se adaptar o código da simulação com a leitura e escrita dos arquivos .txt.
O formato dos arquivos de entrada e de saída precisão seguir essa estrutura. Primeira linha com os nomes das variáveis separadas por vírgula e, na linha de baixo os valores de cada uma das variáveis em ordem, também separada por vírgula.


Para acessar otimizador:

Pré-requisitos: python 3.9 

clonar repositório em uma pasta vazia:
git clone https://github.com/darvenlima/DesOtimizador

Após a clonagem do repositório e com o python 3.9 instalado, é necessário fazer a instalação das bibliotecas usadas no código antes da primeira utilização. Todas as instalações necessárias estão no arquivo bibliotecas.txt. Com a instalação completa, pode realizar a execução do código com o comando:

python .\interface.py

Executando o código abrira a sua interface gráfica, onde no canto esquerdo fica os botões de cada uma das telas. A primeira tela a ser usada deve ser a tela de endereço da simulação, para inserir o endereço do código de simulação e os arquivos .txt de entrada e de saída. Caso o usuário desenvolve a simulação nas linguagens python e R, deve passar o endereço dos arquivos .py e .R respectivamente, já se for utilizado as linguagens C e C++, precisa ser passado o arquivo .exe que é gerado após a compilação do código. Após inserir os três arquivos, clique no botão aplicar para salvar os endereços.

![fig_interface_simu](https://user-images.githubusercontent.com/48968629/153720578-a153a893-2607-4689-bc27-f945d085fcf2.jpg)

A segunda tela, mostra as variáveis de entrada do problema, que o usuário pode selecionar quais são os limites inferior e superior de cada variável (a marquem onde o valor dessa variável pode variar), e definir se a variável é contínua ou inteira.   

![fig_interface_variaveis](https://user-images.githubusercontent.com/48968629/153722035-aeff59de-4d56-471f-9ba8-118bb982535e.jpg)

As últimas duas telas são para inserir as restrições do problema e sua função objetivo, onde na parte superior mostra a lista das variáveis de entrada e saída para construir as restrições e a função objetivo.

![fig_interface_restricoes](https://user-images.githubusercontent.com/48968629/153722668-ea4f0f97-b1ed-4281-b0fa-274030d4b80d.jpg)



Com todas as informações inseridas, o usuário pode clicar no botão "resolver" para iniciar a simulação.


