# POC 1 - Flexbox

Flexbox é um modelo de layout introduzido no CSS3 que simplifica a criação de estruturas de layout complexas e responsivas. Ele permite que os elementos filhos de um contêiner se ajustem automaticamente com base no espaço disponível.O Flexbox facilita o controle sobre o alinhamento, espaçamento e dimensionamento dos itens, tornando o desenvolvimento de layouts mais rápido e eficiente. É especialmente útil para garantir que interfaces funcionem bem em diferentes tamanhos de tela, de desktops a dispositivos móveis.

Flex container é o elemento pai que define o contexto flexível. Ele estabelece o eixo principal e o eixo transversal, ao longo dos quais os elementos filhos são alinhados e distribuídos. O contêiner flexível controla o alinhamento, o espaçamento entre os itens e como eles devem se comportar em relação ao espaço disponível. As propriedades aplicadas ao contêiner, como justify-content, align-items , flex-direction, align-content determinam como os elementos filhos serão organizados.

**Características do Flexbox**

**Display:** 
   O Flexbox é ativado em um contêiner ao aplicar a propriedade `display` com os valores “flex” ou “inline-flex”. Quando o valor “flex” é utilizado, o contêiner se torna um bloco flexível (flex container), enquanto o valor “inline-flex” cria um contêiner flexível em linha. Esse contêiner flexível define um contexto no qual todos os elementos filhos diretos, chamados de “flex items”, são organizados de acordo com as regras do modelo Flexbox.
   
   ```css
   .container {
       display: flex;
   }
   ```
**Justify-content**
Define o alinhamento ao longo do eixo principal (horizontalmente). Ajuda a distribuir o espaço livre extra quando todos os itens flexíveis em uma linha são inflexíveis, ou já atingiram seu tamanho máximo. Também exerce algum controle sobre o alinhamento dos itens quando eles ultrapassam o limite da linha.

* **flex-start:** Itens se alinham à esquerda do container.

```css
.flex-start {
  display:flex;
  justify-content: flex-start;
}
```

![gato1](https://github.com/user-attachments/assets/44d35122-e9d7-473a-837d-ce8a65832322)

* **flex-end:** Itens se alinham à direita do container.

```css
.flex-end {
  display:flex;
  justify-content: end;
}
```
*imagem gatos flex-end*

* **center:** Itens se alinham no centro do container.

```css
.center {
   display:flex;
    justify-content: center;
}
```
*imagem gatos flex-end*


* **space-between:** Itens se alinham com distância igual entre eles.
```
.space-between {
   display:flex;
    justify-content: space-between;
}
```
*imagem gatos center*

* **space-around:** Itens se alinham com distância igual em torno deles.
```
.space-around {
   display:flex;
   justify-content: space-around;
}
```
*imagem gatos space-around*


* **space-evenly:** Distribui o espaço igualmente entre os itens e nas extremidades.
```
.space-evenly {
   display:flex;
   justify-content: space-evenly;
}
```
*imagem gatos space-evenly*


**Align-items**
Define o alinhamento dos itens ao longo do eixo vertical. Isso permite distribuir espaço livre adicional entre os itens de diferentes maneiras:

* **flex-start:** Alinha os itens no início do contêiner verticalmente.

```css
.align-flex-start {
  display:flex;
  align-items: flex-start;
}
```
*imagem gatos flex-start*

* **flex-end:** Alinha os itens no fim do contêiner verticalmente.

```css
.align-flex-end {
  display:flex;
  align-items: flex-end;
}
```
*imagem gatos flex-end*

* **center:** Alinha os itens no centro do contêiner verticalmente.

```css
.align-flex-center {
  display:flex;
  align-items: center;
}
```
*imagem gatos center*


