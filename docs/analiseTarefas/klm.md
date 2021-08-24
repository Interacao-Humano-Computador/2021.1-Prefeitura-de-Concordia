## Versionamento
|Data|Versão|Descrição|Autor(es)
|--|--|--|--|
|23/08|1.0|Inicialização do documento|Natanael Filho|

## 1. Introdução

<p align = "justify"> &emsp;&emsp;  Incluso nos modelos da família GOMS, o KLM é uma técnica simples, onde visa analisar o tempo médio em que o usuário leva para executar tarefas durante navegação. A análise é feita a partir da definição da tarefa analisada, a utilização de operadores primitivos já definidos pela técnica, os quais auxiliam na diferenciação das ações, a descrições das ações e a demora de execução em segundos (BARBOSA, 2021, pág. 198)[1].</p>

<p align = "justify"> &emsp;&emsp; Além disso, é comum que sistemas possuam mais de uma maneira para executar uma tarefa, sendo assim, a análise de tarefas KLM é capaz de evidenciar a diferença de eficiência entre as diversas formas de realização da tarefa  (BARBOSA, 2021, pág. 198-199)[1]. Um exemplo seria em aplicativos de edição de imagem o botão de salvar e a utilização das teclas "CTRL+S", que efetuam a mesma coisa, porém, uma diferença de rapidez considerável.[1]</p>

## 2. Operadores primitivos

<p align = "justify"> &emsp;&emsp; Para a execução dessa tarefa utilizaremos a definição de Keira(1993), onde são definidos 6 operações primitivas principais, segue na tabela 1.</p>
|Operação|Duração Média(em segundos)|
|--|--|
|**K**: pressionar e soltar uma tecla do teclado||
|&emsp;&emsp;exímio digitador(135ppm)|<center>0,08</center>|
|&emsp;&emsp;bom digitador(90ppm)|<center>0,12</center>|
|&emsp;&emsp;digitador mediano (55 ppm)|<center>0,20</center>|
|&emsp;&emsp;digitador inexperiente (40 ppm)|<center>0,28</center>|
|&emsp;&emsp;digitação de letras aleatórias|<center>0,50</center>|
|&emsp;&emsp;digitação de códigos complexos|<center>0,75</center>|
|&emsp;&emsp;digitador não familiarizado com o teclado|<center>1,20</center>|
|**P**: apontar o cursor do mouse num objeto da tela |<center>1,10</center>|
|**B**: pressionar ou soltar o botão do mouse|<center>0,10</center>|
|**H**: levar a mão do teclado ao mouse ou vice-versa|<center>0,40</center>|
|**M**: preparação mental|<center>1,20</center>|
|**T(n)**: digitação de cadeia de caracteres|<center>n x K</center>|
|**W(t)**: espera pela resposta do sistema|<center>depende do sistema</center>|
<h6 align = "center">Tabela 1: Opreções primitivas do KLM-GOMS e seu tempo médio. </h6>
<h6 align = "center">Fonte: Kieras(apud BARBOSA, 2021, p.198)[1]</h6>

## 3. Resultados

### 3.1 KLM acesso a documento de acessibilidade

|Método|Operador|Descrição|Tempo(em s)|
|--|--|--|--|
|**Acessibilidade**|**M**|preparação|<center>1,20</center>|
||**H**|levar a mão do teclado ao mouse|<center>0,40</center>|
||**P**|levar cursor até menu Acesso Portal do cidadão|<center>1,10</center>|
||**B**|pressionar botão do mouse|<center>0,10</center>|
||**B**|soltar botão do mouse|<center>0,10</center>|
||**P**|levar cursor até menu Plano e Políticas Municipais|<center>1,10</center>|
||**P**|levar cursor até opção Plano Diretor Urbano|<center>1,10</center>|
||**P**|levar cursor até opção Acessibilidade|<center>1,10</center>|
||**B**|pressionar botão do mouse|<center>0,10</center>|
||**B**|soltar botão do mouse|<center>0,10</center>|
|||**TOTAL**|<center>**6,40**</center>|

<h6 align = "center">Tabela 2: Análise KLM-GOMS da tarefa Acessibilidade. </h6>
<h6 align = "center">Fonte: Autor</h6>

### 3.2 KLM acesso a Defesa Civil

|Método|Operador|Descrição|Tempo(em s)|
|--|--|--|--|
|**barra de menu opção Estrutura de Governo> Defesa Civil**|**M**|preparação|<center><center>1,20</center></center>|
||**H**|levar a mão do teclado ao mouse|<center>0,40</center>|
||**P**|levar cursor até menu Acesso Portal do cidadão|<center>1,10</center>|
||**B**|pressionar botão do mouse|<center>0,10</center>|
||**B**|soltar botão do mouse|<center>0,10</center>|
||**P**|levar cursor até menu Estrutura de Governo|<center>1,10</center>|
||**P**|levar cursor até opção Defesa Civil|<center>1,10</center>|
||**B**|pressionar botão do mouse|<center>0,10</center>|
||**B**|soltar botão do mouse|<center>0,10</center>|
|||**TOTAL**|<center>**5,30**</center>|
|**menu rotativo  Defesa Civil**|**M**|preparação|<center><center>1,20</center></center>|
||**H**|levar a mão do teclado ao mouse|<center>0,40</center>|
||**P**|levar cursor até menu Acesso Portal do cidadão|<center>1,10</center>|
||**B**|pressionar botão do mouse|<center>0,10</center>|
||**B**|soltar botão do mouse|<center>0,10</center>|
||**P**|levar cursor até a opção  Defesa Civil do menu rotativo|<center>1,10</center>|
||**B**|pressionar botão do mouse|<center>0,10</center>|
||**B**|soltar botão do mouse|<center>0,10</center>|
|||**TOTAL**|<center>**4,20**</center>|

<h6 align = "center">Tabela 3: Análise KLM-GOMS das formas de acesso a Defesa Civil. </h6>
<h6 align = "center">Fonte: Autor</h6>

## 4. Referências

<p style="text-align: justify; text-indent: 20px">[1] BARBOSA et al.<b>Interação Humano-Computador e Experiência do usuário</b>. Autopublicação. 2021.</p>