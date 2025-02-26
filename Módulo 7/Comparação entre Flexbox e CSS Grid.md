# **7. Comparação entre Flexbox e CSS Grid**

## **7.1 Diferenças entre Flexbox e Grid Layout**

### Flex:
O foco do flex é organizar os itens em linhas OU colunas como blocos, um ao lado do outro, ou um sobre o outro. É adequado para organizar layouts em uma dimensão (uma linha ou uma coluna), permitindo manipular o tamanho, alinhamento e distribuição dos seus itens.

### Grid:
Serve para organizar seus itens em forma de grade, linhas e colunas, ou seja, em duas dimensões, possibilitando que cada item tenha um comportamento independente.

## **7.2 Quando usar Flexbox e quando usar Grid**

### Uso do Grid:
Devemos usar o grid para definir o template de uma página, delimitando áreas como header, main e footer, criando o layout onde os elementos vão se encaixar dentro deles, e não o contrário.

### Uso do Flex:
O flex é perfeito para enfileirar elementos de diversos tamanhos. Nele o container define a direção na qual os elementos vão se enfileirar e como eles devem se comportar ao atingir as beiradas do container. Também são definidos como os itens são alinhados independente do tamanho individual de cada item.

## **7.3 Combinação de Flexbox e Grid para layouts avançados**
 Grid Layout para o layout geral (e qualquer coisa que não fosse linear no design). Dentro das áreas de conteúdo da grade, o Flexbox foi usado para ordenar e ajustar o estilo dentro das áreas da grade.

## **7.4 Conversão de layouts Flexbox para Grid e vice-versa**
### De Flexbox para Grid
Flexbox é unidimensional (linha ou coluna), enquanto Grid é bidimensional (linha e coluna). Para converter um layout Flexbox para Grid:
- Mude display: flex para display: grid.
- Converta flex-wrap em grid-template-columns.
- Substitua justify-content e align-items por propriedades equivalentes do Grid.

### De Grid para Flexbox
Se o layout Grid for simples e não precisar de alinhamento complexo de células, ele pode ser convertido para Flexbox. Para converter um layout Grid para Flexbox:
- Troque display: grid por display: flex.
- Use flex-wrap e flex-basis para distribuir os itens.
- Substitua gap por margin nos itens, se necessário.