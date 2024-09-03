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

## Align-content

A propriedade `align-content` é usada para alinhar linhas de itens dentro de um contêiner flexível. Mas, ela só funciona quando há várias linhas de itens. Isso acontece quando os itens "quebram" e vão para a linha de baixo. A propriedade `align-content` ajuda a decidir como essas linhas devem ser organizadas dentro do container. Você pode empurrá-las para cima, para baixo, colocá-las no meio, espalhá-las.


* **flex-start:** Coloca todas as linhas no início do contêiner, como se você empurrasse tudo para cima.*
```css
.container1 {
    align-content: flex-start;
}
```

![gato10](https://github.com/user-attachments/assets/eb3a0873-a9df-4363-b228-0b08624e8fe6)

* **center:** Centraliza as linhas no meio do contêiner, como se você as colocasse no centro.*

```css
.container2 {
    align-content: center;
}
```

![gato11](https://github.com/user-attachments/assets/59dec6f3-ad1d-4b3f-aadf-c96131c0df5c)

* **flex-end:** Coloca todas as linhas no final do contêiner, como se você empurrasse tudo para baixo.*
```css
.container3 {
    align-content: flex-end;
}
```

![gato12](https://github.com/user-attachments/assets/894ad59b-1134-40a4-86d6-afbc3fc95dc3)

* **stretch:** Estica as linhas para preencher todo o espaço disponível do contêiner. Isso faz com que cada linha se ajuste para ocupar o máximo de espaço.*
```css
.container4 {
    align-content: stretch;
}
```

![gato13](https://github.com/user-attachments/assets/f57418a3-b8a3-4d5f-a199-2b4304005c4c)

* **space-between:** Espalha as linhas com o primeiro item no início e o último item no final, deixando espaço igual entre eles.*
```css
.container5 {
    align-content: space-between;
}
```

![gato14](https://github.com/user-attachments/assets/bf756b91-bd44-4ab2-986c-b400aec19df6)

* **space-around:** Coloca espaço igual ao redor de cada linha, como se houvesse uma pequena margem ao redor de cada linha.*
```css
.container6 {
    align-content: space-around;
}
```

![gato15](https://github.com/user-attachments/assets/a65eb9df-3f80-4444-9da0-676ac6d673bc)

## Propriedade order
A propriedade `order` define a ordem em que os itens aparecem dentro do contêiner, não importando a ordem em que foram escritos no código. Isso é útil quando você quer reorganizar os itens de uma forma específica, como colocar algumas imagens em ordens diferentes sem alterar o HTML.
#Como Funciona:
- Primeira Linha: Mostra a ordem padrão dos itens, que é a mesma ordem em que eles aparecem no HTML.
- Segunda Linha: Mostra a ordem dos itens após a aplicação da propriedade order.

```css
/* primeira linha*/
.item1, .item2, .item3, .item4 {
    order: 1;
}

/* segunda linha */
.item5 {
    order: 4; 
}
.item6 {
    order: 1;
}
.item7 {
    order: 2;
}
.item8 {
    order: 3;
}
```
![gato16](https://github.com/user-attachments/assets/02b37f40-2cf8-402f-b343-da70b7fac19f)







