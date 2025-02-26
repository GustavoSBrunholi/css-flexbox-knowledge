# **6. Flexbox e Responsividade**

## **6.1 Uso de `flex-wrap` para adaptação em telas menores**
O `flex-wrap` permite que os elementos quebrem para uma nova linha conforme necessário, evitando a sobreposição e melhora a organização em telas pequenas.

## **6.2 Combinando Flexbox com Media Queries**
Utilize `@media` para modificar propriedades do Flexbox conforme a largura da tela.
- Exemplo: mudar `flex-direction` de `row` para `column` em telas menores.
```css
@media (max-width: 600px) {
    .container {
        flex-direction: column;
    }
}
```

## **6.3 Melhorando a usabilidade em dispositivos móveis**
Como programadores devemos garantir espaçamentos adequados entre os elementos em diferentes telas.

### Alguns modos de melhorar essa usabilidade é:
- Aplicar `min-width` e `max-width` para evitar layouts quebrados.
- Utilizar `align-items: center;` para melhorar a organização dos componentes.

## **6.4 Criando layouts flexíveis sem necessidade de Media Queries**
Para criarmos layouts flexíveis sem Media Queries precisamos definir `flex-grow` e `flex-shrink` para permitir adaptação automática do layout e Utilizar `min-width` e `max-width` para controle de expansão dos itens.
```css
.item {
    flex-grow: 1;
    flex-shrink: 1;
    min-width: 150px;
}
```

## **6.5 Testando responsividade com ferramentas do navegador**
### Para testarmos essa responsividade, temos algumas formas:
- Podemos utilizar o DevTools (apertando `F12` Chrome) para testar diferentes resoluções.
- Ativando a opção de simulação de dispositivos móveis no navegador.
- Ajustar `flex-wrap`, `justify-content` e `align-items` conforme necessário.