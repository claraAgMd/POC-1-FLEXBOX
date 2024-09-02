<h1 align="center">POC 1 - Flexbox</h1>

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
## Justify-content
Define o alinhamento ao longo do eixo principal (horizontalmente). Ajuda a distribuir o espaço livre extra quando todos os itens flexíveis em uma linha são inflexíveis, ou já atingiram seu tamanho máximo. Também exerce algum controle sobre o alinhamento dos itens quando eles ultrapassam o limite da linha.

* **flex-start:** Itens se alinham à esquerda do container.

```css
.flex-start {
  display:flex;
  justify-content: flex-start;
}
```

![gato1](https://github.com/user-attachments/assets/09947054-3c9d-4c07-8a09-f22a1fdaff35)

* **flex-end:** Itens se alinham à direita do container.

```css
.flex-end {
  display:flex;
  justify-content: end;
}
```

![gato2](https://github.com/user-attachments/assets/79fc5388-d830-4c6b-a389-2632521767b2)


* **center:** Itens se alinham no centro do container.

```css
.center {
   display:flex;
    justify-content: center;
}
```

![gato3](https://github.com/user-attachments/assets/0da67385-e982-4128-ac6f-3d981dbfe61c)



* **space-between:** Itens se alinham com distância igual entre eles.
```css
.space-between {
   display:flex;
    justify-content: space-between;
}
```

![gato4](https://github.com/user-attachments/assets/bc45f22b-7ccb-4658-919a-b6bcadc888dd)


* **space-around:** Itens se alinham com distância igual em torno deles.
```css
.space-around {
   display:flex;
   justify-content: space-around;
}
```

![gato5](https://github.com/user-attachments/assets/b19826c1-5d99-4438-bb17-82ecd041b9d0)



* **space-evenly:** Distribui o espaço igualmente entre os itens e nas extremidades.
```css
.space-evenly {
   display:flex;
   justify-content: space-evenly;
}
```

![gato6](https://github.com/user-attachments/assets/30c15c33-09ca-485c-afe4-5c246225b79f)




## Align-items
Define o alinhamento dos itens ao longo do eixo vertical. Isso permite distribuir espaço livre adicional entre os itens de diferentes maneiras:

* **flex-start:** Alinha os itens no início do contêiner verticalmente.

```css
.align-flex-start {
  display:flex;
  align-items: flex-start;
}
```

![gato7](https://github.com/user-attachments/assets/a51fe32f-0bf0-4d51-817a-c5fbbc849bec)


* **flex-end:** Alinha os itens no fim do contêiner verticalmente.

```css
.align-flex-end {
  display:flex;
  align-items: flex-end;
}
```

![gato8](https://github.com/user-attachments/assets/7fcd6e77-badd-4a0f-b8b4-3cf90eba3b2d)


* **center:** Alinha os itens no centro do contêiner verticalmente.

```css
.align-flex-center {
  display:flex;
  align-items: center;
}
```

![gato9](https://github.com/user-attachments/assets/1376d3b0-7fbe-4d08-858c-3c1b29d81bb5)


