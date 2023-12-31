# Box-Model
O Conceito do box-model, é todos os elementos no html são interpretados como caixas. <br> Como caixas de papelão, os elementos tem, conteúdo (Content), altura (Height), largura (Width), bordas (Border), preenchimento interno (Padding), espaços ao redor (Margin). 

**Display é uma propriedade.**
--------
## TIPOS DE DISPLAY'S:

### Display Block <br>
Tem algumas propriedades, e uma delas é sobre a largura. A largura de um elemento do tipo display block, esse elemento vai ocupar todo o espaço disponível. <br>
Fazendo com que um próximo elemento na página fique não ao lado dele mas, abaixo dele. Porque ele ocupa todo o espaço disponível dele, ou seja, cada elemento ocupar uma linha inteira, e ai ele vai outro elemento abaixo dele e assim sucessivamente com os demais elementos que tenham o display do tipo block.

        Por padrão, elementos como div, section, p, h1, h2, ul, li, article são display block. 
----
### Display Inline <br>
No display inline faz com que o tamanho dos elementos, seja de acordo com o tamanho do conteúdo desses elementos. E cada elemento fica um do lado do outro. <br> Os elementos não são jogado para baixo, isso é, um em baixo do outro, pois não ocupam a linha toda. <br>

    Por padrão, elementos como a, b, big, i, small, tt. abbr, acronym, cite, code, dfn, em, kbd, strong, samp, var. a, bdo, br, img, map, object, q, script, span, sub, sup. em são display inline.     
TANTO O DISPLAY: BLOCK E O DISPLAY: INLINE, ESSES TIPOS DE DISPLAY'S, TRATAM OS ELEMENTOS, ISSO É, AS CAIXAS QUE ESTÃO UMA DO LADO DA OUTRA, EM UM ESCOPO ABERTO.

    PODEMOS TER CAIXAS DENTRO DE OUTRAS CAIXAS.

    DISPLAY BLOCK E INLINE, TEM A VER COM A CAIXA EM SÍ E COMO ESTÁ O AMBIÊNTE AO REDOR DELA.

---
### Display Flex <br>
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


## EXPLICAÇÃO DE CADA PROPRIEDADE QUE O DISPLAY FLEX TEM <br>
FLEX-DIRECTION
        A propriedade flex-direction deve ser aplicada ao container e define o eixo/fluxo de exibição em que os elementos serão organizados. A sintaxe e os valores possíveis para essa propriedade são apresentados a seguir:

        flex-direction: [row / row-universe / column / column-reverse] 

        row (padrão): Os itens são organizados em forma de linha da esquerda para a direita;
        row-reverse: Os itens são organizados em forma exibição em linha da direita para a esquerda;
        column: Os itens são organizados em forma de colunas iniciando de cima para baixo;
        column-reverse: Os itens são organizados em forma de colunas iniciando de baixo para cima.
        ..............................................................................................................
        FLEX-WRAP
        Por padrão os itens do container tentarão se ajustar em uma única linha dentro do container, mas para isso a sua largura original pode ser ajustada para que todos caibam na largura do elemento pai. Com a propriedade flex-wrap aplicada ao container podemos alterar esse comportamento, fazendo com que ocorra a “quebra de linha” nos itens.

        A sintaxe e os valores possíveis para essa propriedade são apresentados a seguir:   

        flex-wrap:[nowrap / wrap / wrap-reverse]

        nowrap (padrão): Todos os itens serão dispostos em uma linha;
        wrap: Ocorrerá a quebra de linha e os itens mais à direita serão deslocados para a linha de baixo;
        wrap-reverse: Ocorrerá a quebra de linha e os itens mais à direita serão deslocados para a linha de cima;
        ..............................................................................................................

        FLEX-FLOW
        Esta propriedade é uma forma abreviada para a escrita das propriedades flex-direction e flex-wrap, nesta ordem. Portanto, ela se aplica ao container.

        Normalmente essas propriedades são definidas uma a uma, da seguinte forma:

        flex-flow:[column wrap], 
        
        Já com o flex-flow podemos escrever as duas de forma simplificada:
        ..............................................................................................................
        ALIGN-CONTENT
        Essa propriedade define como as linhas são distribuídas ao longo do eixo transversal do container. Ela só terá efeito se o elemento tiver mais de uma linha, ou seja, se ele tiver elementos suficientes para quebrar a linha e a propriedade flex-wrap:wrap tiver sido definida. A sintaxe e os valores possíveis para essa propriedade são apresentados a seguir:

        align-content:[stretch / flex-start / flex-end / center / space-between / space-around] 

        stretch (padrão): As linhas são distribuídas uniformemente ao longo do eixo transversal, ocupando todo o espaço disponível;
        flex-start: As linhas são distribuídas a partir do início do eixo transversal;
        flex-end: As linhas são distribuídas a partir do fim do eixo transversal;
        center: As linhas são mantidas no centro do eixo transversal;
        space-between: A primeira linha é deslocada para o início do eixo transversal, a última é deslocada para o final do eixo transversal e as demais são distribuídas uniformemente entre eles;
        space-around: As linhas são uniformemente distribuídas ao longo do eixo transversal. Aqui, porém, são atribuídas margens iguais à esquerda e à direita (ou acima e abaixo, dependendo da direção do eixo transversal). Por isso a primeira e a última linha não ficam “coladas” nas bordas do container.
        ..............................................................................................................
        ALIGN-ITEMS
        Essa propriedade define como os itens são distribuídos ao longo do eixo transversal do container. A sintaxe e os valores possíveis para essa propriedade são apresentados a seguir:

        align-items:[stretch / flex-start / flex-end / center / baseline]

        stretch (padrão): Os itens serão esticados para preencher toda a dimensão do eixo transversal (altura ou largura);
        flex-start: Os itens são deslocadas para o início do eixo transversal;
        flex-end: Os itens são deslocadas para o final do eixo transversal;
        center: Os itens são centralizados no eixo transversal;
        baseline: Os itens são alinhados a partir da base da primeira linha de texto de cada um.
        ..............................................................................................................
        ORDER
        Por padrão, os itens são distribuídos no container na ordem em que são inseridos no HTML. No entanto, essa ordem pode ser alterada por meio da propriedade order, cuja sintaxe vemos abaixo:

        order:[número], flex:[flex-grow:[número], flex-shrink:[número]

        O valor numérico atribuído a essa propriedade define a ordem do item. Por exemplo, o valor 2 faz com que o item seja o segundo item ao longo do eixo principal, enquanto o valor -1 faz com que ele apareça antes do primeiro.
        ..............................................................................................................
        FLEX-GROW
        Esta propriedade define a proporção com que um item deve crescer caso seja necessário. Por padrão seu valor é 0, o que indica que o item não deve crescer, e são aceitos apenas valores numéricos positivos.

        A sintaxe dessa propriedade é a seguinte:
        
        flex-grow: [número]
        ..............................................................................................................
        FLEX-SHRINK
        Esta propriedade define a proporção com que um item deve encolher caso seja necessário. Essa propriedade aceita apenas valores positivos, e seu valor padrão é 1.

        A sintaxe dessa propriedade é a seguinte:

        flex-shrink: [número];
        ..............................................................................................................
        FLEX-BASIS
        O flex-basis define o tamanho inicial que um item deve ter antes que o espaço ao seu redor seja distribuído. Ou seja, dependendo da direção do eixo principal (horizontal ou vertical), essa propriedade define a largura ou altura mínima do elemento antes que ele seja redimensionado por outras propriedades.

        A sintaxe dessa propriedade é a seguinte:

        flex-basis:[número];

        O valor atribuído a essa propriedade pode ser em percentual, em pixels, ou a palavra auto, que é o valor padrão (considera as dimensões do item - width e height).
        ..............................................................................................................
        ALIGN-SELF
        Esta propriedade permite sobrescrever no item o comportamento que foi definido pela propriedade align-items.

        A sintaxe e os valores possíveis para essa propriedade são apresentados a seguir:

        align-self:[auto / stretch / flex-start / flex-end / centerr / baseline].
        
        auto (padrão): Respeita o comportamento definido no container por meio do align-items;
        stretch: O item será esticado para preencher toda a dimensão do eixo transversal (altura ou largura);
        flex-start: O item é deslocado para o início do eixo transversal;
        flex-end: O item é deslocado para o final do eixo transversal;
        center: O item é centralizado no eixo transversal;
        baseline: O item é alinhado a partir da base da primeira linha de texto dos demais.
        ..............................................................................................................
        FLEX
        Esta propriedade é uma forma abreviada para a escrita das propriedades flex-grow, flex-shrink e flex-basis, nesta ordem.

        A sintaxe dessa propriedade é a seguinte:

        flex: [flex-grow] [flex-shrink] [flex-basis];

---


