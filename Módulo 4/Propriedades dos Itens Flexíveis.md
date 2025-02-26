# **4. Propriedades dos Itens Flexíveis**

## **4.1 `order`** – Definição de ordem de exibição
![<Representação do order>](<../imgs/order-img.png>)
Define a ordem para dispor um item em um contêiner flexível ou de grid.
```
.item {
  order: 5; /* default is 0 */
}
```

## **4.2 `flex-grow`** – Crescimento proporcional dos itens
![<Representação do flex-grow>](<../imgs/flex-grow-img.png>)
Define o fator de crescimento flex, que especifica quanto do espaço livre positivo do contêiner flex, se houver, deve ser atribuído ao tamanho principal do item flex.

```
.item {
  flex-grow: 4; /* default 0 */
}
```

## **4.3 `flex-shrink`** – Redução proporcional dos itens
Especifica o fator de redução flex, que determina o quanto o item flex será reduzido em relação ao restante dos itens flex no contêiner flex quando o espaço livre negativo for distribuído.

```
.item {
  flex-shrink: 3; /* default 1 */
}
```

## **4.4 `flex-basis`** – Tamanho inicial do item
Especifica o tamanho inicial de um item flex antes que ocorra qualquer distribuição do espaço livre positivo ou negativo.

```
.item {
  flex-basis:  | auto; /* default auto */
}
```

## **4.5 `flex`** – Atalho para `flex-grow`, `flex-shrink` e `flex-basis`
É uma forma abreviada para definir o `flex-grow`, `flex-shrink` e `flex-basis`

```
.item {
  flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
}
```

## **4.6 `align-self`** – Alinhamento individual dos itens
![<Representação do align-self>](<../imgs/align-self-img.png>)
Alinha os itens-flex da linha flex alvo, sobreescrevendo o valor align-items.

```
.item {
  align-self: auto | flex-start | flex-end | center | baseline | stretch;
}
```