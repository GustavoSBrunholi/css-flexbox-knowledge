# **3. Propriedades do Contêiner Flexível**

## **3.1 `flex-direction`** – Direção dos elementos
![<Representação do flex-direction>](<../imgs/flex-direction-img.png>)
A propriedade flex-direction define a direção do eixo principal e pode ter quatro valores possíveis:
```
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```

`row (linha)` ou `row-reverse (linha reversa)`, seu eixo principal se moverá ao longo da linha, com direção inline.

`column (coluna)` ou `column-reverse (coluna reversa)` o eixo principal se moverá do topo até o fim da página, com direção block.

## **3.2 `flex-wrap`** – Quebra de linha dos itens
![<Representação do flex-wrap>](<../imgs/flex-wrap-img.png>)
Ele define se os itens flexíveis são forçados a ficarem na mesma linha ou se podem ser quebradas em varias linhas.
```
.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```
`nowrap:` Os itens flexíveis são agrupados em uma unica linha.
`wrap:` Os itens flexíveis são quebrados em multiplas linhas.
`wrap-reverse:` Se comporta da mesma maneira que o wrap mas a quebra de linhas ocorre na direção contrária, ou seja, de baixo para cima.

## **3.3 `flex-flow`** – Atalho para `flex-direction` e `flex-wrap`
```
.container {
  flex-flow: column wrap;
}
```
Ele é uma junção das propriedades flex-direction e flex-wrap, que juntas definem os eixos principal e cruzado do contêiner flex.

## **3.4 `justify-content`** – Alinhamento horizontal dos itens
![<Representação do justify-content>](<../imgs/justify-content-img.png>)
Define como o navegador distribui o espaço entre e ao redor dos itens de conteúdo ao longo do eixo principal de um contêiner flexível.
```
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;
}
```

`flex-start:` Os itens são compactados em direção à borda inicial do contêiner de alinhamento no lado inícial principal do contêiner flexível.

`flex-end:` Os itens são compactados e alinhados na borda final do contêiner.

`start:` Os itens são compactados e alinhados uns aos outros em direção à borda inicial do contêiner.

`end:` Os itens são compactados e alinhados uns com os outros em direção à borda final do contêiner.

`left:` Os itens são compactados e alinhados uns aos outros em direção à borda esquerda do contêiner.

`right:` Os itens são compactados e alinhados uns aos outros em direção à borda direita do contêiner.

`center:` Os itens são compactados e alinhados uns aos outros em direção ao centro do contêiner.

`space-between:` Os itens são distribuídos uniformemente dentro do contêiner. O primeiro item estará alinhado na borda inicial e o últim item alinhado no final do contêiner.

`space-arround:` Os itens são distribuídos uniformemente dentro do contêiner. Possui um espaço vazio antes do primeiro e depois do último item igual à metade do espaço entre cada par de itens.

`space-evenly:` Os itens são distribuídos uniformemente dentro do contêiner. Tendo um espaçamento entre cada item e o espaço vazio antes do primeiro e depois do último item, sendo exatamente os mesmos.


## **3.5 `align-items`** – Alinhamento vertical dos itens
![<Representação do align-items>](<../imgs/align-items-img.png>)
Define o comportamento padrão de como os itens flexíveis são dispostos ao longo do eixo cruzado na linha atual.

```
.container {
  align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe;
}
```

`stretch:` Os itens-flex são esticados de uma maneira que o tamanho da caixa de margem do item seja o mesmo da linha.

`flex-start / start / self-start:` Os itens são colocados no início do eixo cruzado.

`flex-end / end / self-end:` Os itens são colocados no final do eixo cruzado.

`center:` As caixas de margem dos itens flex são centralizados ao longo da linha do eixo.

`baseline:` Os itens são alinhados, assim como suas linhas de base se alinham

## **3.6 `align-content`** – Alinhamento em múltiplas linhas
![<Representação do align-content>](<../imgs/align-content-img.png>)
Define a distribuição entre e ao redor dos items do conteúdo do eixo transversal de uma flexbox ou do eixo de bloco de uma grid.

```
.container {
  align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end | baseline | first baseline | last baseline + ... safe | unsafe;
}
```

`normal:` Os itens são compactados em sua posição padrão como se nenhum valor tivesse sido definido.

`flex-start / start:` Os itens embalados até o início do contêiner.

`flex-end / end:` Os itens são embalados até o final do contêiner.

`center:` Os itens são centralizados no contêiner

`space-between:` Os itens são distribuídos uniformemente, a primeira linha está no início do contêiner, enquanto a última está no final

`space-around:` Os itens são distribuídos uniformemente com espaço igual ao redor de cada linha

`space-evenly:` Os itens são distribuídos uniformemente com espaço igual ao seu redor

`stretch:` As linhas se estendem para ocupar o espaço restante