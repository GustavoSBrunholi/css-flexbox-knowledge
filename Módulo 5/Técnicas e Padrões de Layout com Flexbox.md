# **5. Técnicas e Padrões de Layout com Flexbox**

## **5.1 Criando um layout de coluna responsivo*
- Utilize `flex-direction: column;` para organizar os elementos verticalmente.
- E Defina `flex-wrap: wrap;` para que os elementos se ajustem a diferente tamanhos de tela.

```css
.container {
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
}
```

## **5.2 Criando um layout de linha responsivo**
- Use o `flex-direction: row;` para distribuir os elementos horizontalmente.
- Aplique `justify-content: space-between;` para melhor espaçamento entre os itens.

```css
.container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}
```

## **5.3 Centralizando elementos com Flexbox**
- Utilize o `justify-content: center;` para centralizar horizontalmente.
- Aplique `align-items: center;` para centralizar verticalmente.
- E para alinhamento total, use o `display: flex; justify-content: center; align-items: center; height: 100vh;`.

```css
.container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
```
## **5.4 Criando um menu de navegação flexível**
- Defina `display: flex;` no contêiner do menu.
- Use `justify-content: space-around;` ou `justify-content: space-between;` para os espaçamentos dos itens.
- E utilize o `flex-wrap: wrap;` para garantir adaptação em telas menores.

```css
.menu {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
}
```

## **5.5 Criando um grid de cards com Flexbox**
- Utilize `display: flex; flex-wrap: wrap;` para organizar os cards em várias linhas.
- Utilize o `justify-content: space-evenly;` para distribuir os elementos uniformemente.
- E Defina `flex: 1 1 300px;` para garantir tamanhos proporcionais.

```css
.grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-evenly;
}

.card {
    flex: 1 1 300px;
}
```
