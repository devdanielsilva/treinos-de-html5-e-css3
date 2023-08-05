# Box-Model
O Conceito do box-model, é todos os elementos no html são interpretados como caixas. <br> Como caixas de papelão, os elementos tem, conteúdo (Content), altura (Height), largura (Width), bordas (Border), preenchimento interno (Padding), espaços ao redor (Margin). 

**Display é uma propriedade.**
--------
**TIPOS DE DISPLAY'S:**

**Display Block** <br>
Tem algumas propriedades, e uma delas é sobre a largura. A largura de um elemento do tipo display block, esse elemento vai ocupar todo o espaço disponível. <br>
Fazendo com que um próximo elemento na página fique não ao lado dele mas, abaixo dele. Porque ele ocupa todo o espaço disponível dele, ou seja, cada elemento ocupar uma linha inteira, e ai ele vai outro elemento abaixo dele e assim sucessivamente com os demais elementos que tenham o display do tipo block.

        Por padrão, elementos como div, section, p, h1, h2, ul, li, article são display block. 
----
**Display Inline** <br>
No display inline faz com que o tamanho dos elementos, seja de acordo com o tamanho do conteúdo desses elementos. E cada elemento fica um do lado do outro. <br> Os elementos não são jogado para baixo, isso é, um em baixo do outro, pois não ocupam a linha toda. <br>

    Por padrão, elementos como a, b, big, i, small, tt. abbr, acronym, cite, code, dfn, em, kbd, strong, samp, var. a, bdo, br, img, map, object, q, script, span, sub, sup. em são display inline.     
TANTO O DISPLAY: BLOCK E O DISPLAY: INLINE, ESSES TIPOS DE DISPLAY'S, TRATAM OS ELEMENTOS, ISSO É, AS CAIXAS QUE ESTÃO UMA DO LADO DA OUTRA, EM UM ESCOPO ABERTO.

    PODEMOS TER CAIXAS DENTRO DE OUTRAS CAIXAS.

    DISPLAY BLOCK E INLINE, TEM A VER COM A CAIXA EM SÍ E COMO ESTÁ O AMBIÊNTE AO REDOR DELA.

---
**Display Flex** <br>
O Display flex, tem a ver com as caixas dentro de outras caixas.
Através dessa propriedade flex, pode se dizer que temos o "Destrave" de algumas propriedades. <br>
POR EXEMPLO: 
        JUSTIFY-CONTENT
        A propriedade justify-content define o alinhamento dos itens ao longo do eixo principal do container. A sintaxe e os valores possíveis para essa propriedade são apresentados a seguir:

    justify-content: [center, flex-start / flex-end / space-between / space-around / space-evenly] 

    flex-start (padrão): Os itens são alinhados a partir do início do eixo principal;

    flex-end: Os itens são alinhados a partir do fim do eixo principal;

    center: Os itens são alinhados ao centro do eixo principal;

     space-between: O primeiro item é deslocado para o início do eixo principal, o último é deslocado para o final do eixo principal e os demais são distribuídos uniformemente entre eles;

     space-around: Os itens são uniformemente distribuídos ao longo do eixo principal. Aqui, porém, são atribuídas margens iguais à esquerda e à direita (ou acima e abaixo, dependendo da direção do eixo principal). Por isso o primeiro e o último item não ficam “colados” nas bordas do container.

     space-evenly: Espaços constante, espaços entre e ao redor dos elementos. E esse espaços são proporcionais do mesmo tamanho.


**EXPLICAÇÃO DE CADA PROPRIEDADE QUE O DISPLAY FLEX TEM** <br>





