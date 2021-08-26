## Versionamento
|Data|Versão|Descrição|Autor(es)
|--|--|--|--|
|22/08|1.0|Criação de documento|Abraão Alves|

## 1. Introdução
<p align = "justify"> &emsp;&emsp; O CMN-GOMS é um dos modelos utilizados para a analise de tarefas que faz referencia a proposta original GOMS, onde os operadores são executados estritamente em ordem sequencial, e os métodos são representados numa notação semelhante a um pseudocódigo, que inclui submétodos e condicionais, portanto, a análise é geral e executável. Qualquer instância de classe de tarefas descrita pode ser realizada ou simulada seguindo os passos do modelo que podem passar por caminhos diferentes dependendo da situação específica da tarefa [1].</p>

## 2. Elaboração
<p align = "justify"> &emsp;&emsp; Ao elaborar um modelo GOMS, devemos definir cuidadosamente o que representar e o que não representar. Tarefas mentais podem ser complexas, o nível de detalhes utilizado deve atender aos objetivos da análise. Em etapas iniciais, costumamos representar as estratégias alternativas que o usuário poderá seguir para atingir seus objetivos [1].</p>

<center><img src="../../images/analiseTarefas/cmn-goms-modelo.png"></center>
<h6 align = "center">Imagem 1: Exemplo de modelo CMN-GOMS sem detalhes.</h6>
<h6 align = "center">Figura retirada do livro Interação Humano-Computador de BARBOSA et al. (2021, pag.170) [1]</h6>

<p align = "justify">  &emsp;&emsp;  os modelos CMN-GOMS permitem prever a sequência de operadores e o tempo de execução. Qualitativamente, eles focam métodos para alcançar objetivos: métodos semelhantes são facilmente identificados, métodos atipicamente curtos ou longos se destacam e podem disparar ideias de design, como, por exemplo, a inclusão de teclas de atalho para comandos frequentes e pontos de feedback para o usuário.</p>

## 3 Legenda
|Termo|Tradução|Descrição|
|--|--|--|
|Goal|Objetivo|O que o usuário quer realizar utilizando o sistema|
|OP|Operador|Ações concretas que o site permite que o usuário faça|
|METHOD|Método|Sequência de subobjetivos e operadores para atingir um objetivo maior|
|SEL.RULE|Regra de seleção|Tomada de decisão sobre qual método utilizar|

## 4 Análise
<p align = "justify">  &emsp;&emsp; A análise em questão busca realizar o mapeamento dos objetivos, métodos e operações utilizadas para serem realizadas algumas tarefas comums dentro do site. Lembrando que  o ponto de partida do usuario para executar a tarefa analisada é a home do site.</p>

### 4.1 Copiar Telefone de atendimento
~~~
Goal 0: Copiar Telefone de atendimento
    Goal 1: Encontrar Informações de contato
        METHOD 1.A: Encontrar através do menu secundário
        (SEL.RULE: preferência do usuário)
            OP: Levar cursor até o menu
            OP: Levar o cursor a opção com nome acesso à informação
            OP: Clicar com o botão esquerdo do mouse
            OP: Rolar tela para baixo até a área com nome Atendimento Telefone
        METHOD 1.B: Encontrar através da área de pesquisa do menu
        (SEL.RULE: preferência do usuário)
            OP: Levar cursor até o menu secundário
            OP: Levar o cursor a opção de pesquisa 
            OP: Clicar com o botão esquerdo do mouse
            OP: Digitar a palavra "ouvidoria"
            OP: Levar cursor até a coluna central com nome serviços
            OP: Levar cursor até a opção com nome ouvidoria municipal
            OP: Clicar com o botão esquerdo do mouse
    Goal 2: Copiar telefone
        OP: Levar Cursor até o numero de telefone desejado
        OP: selecionar todo o numero de telefone com o botão esquerdo do mouse
        OP: Clicar com botão direito do mouse
        OP: Levar cursor até a opção menu "Copiar"
        OP: Clicar com botão esquerdo do mouse
~~~

### 4.2 Solicitar Reclamação da falta de água na região
~~~
Goal 0: Solicitar Reclamação da falta de água na região


    Goal 1: Encontrar formulário de reclamação
        METHOD 1.A: Encontrar através do cabeçalho
        (SEL.RULE: preferência do usuário)
            OP: Levar cursor até o cabeçalho
            OP: Levar cursor até a opção Serviços
            OP: Levar cursor até a opção com nome falta de água
            OP: clicar com o botão esquerdo do mouse
         METHOD 1.B: Encontrar através da área de pesquisa do menu
        (SEL.RULE: preferência do usuário)
            OP: Levar cursor até o menu secundário
            OP: Levar o cursor a opção de pesquisa 
            OP: Clicar com o botão esquerdo do mouse
            OP: Digitar a palavra "falta de água"
            OP: Levar cursor até a coluna com nome páginas 
            OP: Levar cursor até a opção com nome Falta de água
            OP: Clicar com o botão esquerdo do mouse
    Goal 2: Preencher do formulário de reclamação      
        METHOD 2: inserir dados corretos nos campos do formulário
            OP: Levar cursor até o campo de nome
            OP: Clicar com o botão esquerdo do mouse
            OP: inserir através do teclado o nome
            OP: Levar cursor até o campo de Telefone
            OP: Clicar com o botão esquerdo do mouse
            OP: inserir numero de telefone através do teclado
            OP: Levar cursor até o campo de mensagem
            OP: Clicar com o botão esquerdo do mouse
            OP: inserir mensagem através do teclado
           
    Goal 3: Enviar Formulário de reclamação
    (SEL.RULE: Formulário deve estar com todas informações obrigatórias)
       METHOD 3: Usar botão de confirmação
            OP: levar cursor até o botão com nome "confirmar"
            OP: clicar com o botão esquerdo do mouse
~~~


## 5. Referências

<p style="text-align: justify; text-indent: 20px">[1] BARBOSA et al.<b>Interação Humano-Computador e Experiência do usuário</b>. Autopublicação. 2021.</p>
