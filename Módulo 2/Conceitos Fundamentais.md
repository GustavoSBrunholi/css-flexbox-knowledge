# **2. Conceitos Fundamentais**

## **2.1** O Modelo de Caixa Flexível
No Modelo de Caixa Flexível cada elemento é envolto em uma "caixa flexível" que permite o ajuste dinâmico de tamanho e posicionamento.

## **2.2** Elemento Pai (Flex Container) vs. Elementos Filhos (Flex Items)

### **Flex Container:** 
#### Ele é o elemento que possui a propriedade display: flex.
![<Representação do container>](<../imgs/container-image.png>)

### **Flex Items:** 
#### São os elementos internos do flex contêiner, que herdam as propriedades flexíveis.
![<Representação dos items>](<../imgs/items-image.png>)

## **2.3** Propriedade `display: flex` e seus efeitos
É utilizado para definir um recipiente flexível, em linha ou bloco, dependendo do valor dado. Ele permite um contexto flexível para todos os filhos do container diretas.

```
.container {
  display: flex;
}
```