## Versionamento
|Data|Versão|Descrição|Autor(es)
|--|--|--|--|
|23/08|1.0|Inicialização do documento|Natanael Filho|

## 1. Introdução

<p align = "justify"> &emsp;&emsp;  Incluso nos modelos da família GOMS, o KLM é uma técnica simples, onde visa analisar o tempo médio em que o usuário leva para executar tarefas durante navegação. A análise e feita a partir da definição da tarefa analisada, a utilização de operadores primitivos já definidos pela técnica, os quais auxiliam na diferenciação das ações, a descrições das ações e a demora de execução em segundos.</p>

<p align = "justify"> &emsp;&emsp; Além disso, é comum que sistemas possuam mais de uma maneira para executar uma tarefa, sendo assim, a análise de tarefas KLM pode evidenciar a diferença de eficiência entre as diversas formas de execução da tarefa. Um exemplo seria em aplicativos de edição de imagem o botão de salvar e a utilização das teclas "CTRL+S", que efetuam a mesma coisa, porém, uma diferença de rapidez considerável.</p>

## 2. Operadores primitivos

<p align = "justify"> &emsp;&emsp; Para a execução dessa tarefa utilizaremos a definição de Keira(1993), onde são definidos 6 operações primitivas principais, segue na tabela 1.</p>
|Operação|Duração Média(em segundos)|
|--|--|
|K: pressionar e soltar uma tecla do teclado||
|&emsp;&emsp;exímio digitador(135ppm|0,08|
|&emsp;&emsp;bom digitador(90ppm)|0,12|
|&emsp;&emsp;digitador mediano (55 ppm)|0,20|
|&emsp;&emsp;digitador inexperiente (40 ppm)|0,28|
|&emsp;&emsp;digitação de letras aleatórias|0,50|
|&emsp;&emsp;digitação de códigos complexos|0,75|
|&emsp;&emsp;digitador não familiarizado com o teclado|1,20|
|P: apontar o cursor do mouse num objeto da tela |1,10|
|B: pressionar ou soltar o botão do mouse|0,10|
|H: levar a mão do teclado ao mouse ou vice-versa|0,40|
|M: preparação mental|1,20|
|T (n): digitação de cadeia de caracteres|n x K|
|W(t): espera pela resposta do sistema|depende do sistema|
<h6 align = "center">Tabela 1: Opreções primitivas do KLM-GOMS e seu tempo médio. </h6>
<h6 align = "center">Fonte: Kieras(apud BARBOSA, 2021, p.198)[1]</h6>

## 3. Resultados

### 3.1 KLM Acesso a notícias

|Método|Operador|Descrição|Tempo(em s)|
|--|--|--|--|
|**Notícias**|M|preparação|1,20|
||H|levar a mão do teclado ao mouse|0,40|
||P|levar cursor até menu Acesso Portal do cidadão|1,10|
||B|pressionar botão do mouse|0,10|
||B|soltar botão do mouse|0,10|
||P|levar cursor até menu Notícia|1,10|
||B|pressionar botão do mouse|0,10|
||B|soltar botão do mouse|0,10|
||P|levar cursor até rolagem da página|1,10|
||B|pressionar botão do mouse|0,10|
||P|levar cursor até posição onde está à notícia|1,10|
||B|soltar botão do mouse|0,10|
|||**TOTAL**|**6,60**|

<h6 align = "center">Tabela 2: Análise KLM-GOMS da tarefa Notícias. </h6>
<h6 align = "center">Fonte: Autor</h6>

### 3.2 KLM Defesa Civil

|Método|Operador|Descrição|Tempo(em s)|
|--|--|--|--|
|**Menu Estrutura de Governo> Defesa Civil**|M|preparação|1,20|
||H|levar a mão do teclado ao mouse|0,40|
||P|levar cursor até menu Acesso Portal do cidadão|1,10|
||B|pressionar botão do mouse|0,10|
||B|soltar botão do mouse|0,10|
||P|levar cursor até menu Estrutura de Governo|1,10|
||P|levar cursor até menu Defesa Civil|1,10|
||B|pressionar botão do mouse|0,10|
||B|soltar botão do mouse|0,10|
|||**TOTAL**|**5,30**|
|**Defesa Civil**|M|preparação|1,20|
||H|levar a mão do teclado ao mouse|0,40|
||P|levar cursor até menu Acesso Portal do cidadão|1,10|
||B|pressionar botão do mouse|0,10|
||B|soltar botão do mouse|0,10|
||P|levar cursor até menu Defesa Civil|1,10|
||B|pressionar botão do mouse|0,10|
||B|soltar botão do mouse|0,10|
|||**TOTAL**|**4,20**|

<h6 align = "center">Tabela 2: Análise KLM-GOMS das formas de acesso a Defesa Civil. </h6>
<h6 align = "center">Fonte: Autor</h6>

## 4. Referências

<p style="text-align: justify; text-indent: 20px">[1] BARBOSA et al.<b>Interação Humano-Computador e Experiência do usuário</b>. Autopublicação. 2021.</p>