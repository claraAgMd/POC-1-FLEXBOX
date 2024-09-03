<h1 align="center">POC 1 - Flexbox</h1>

## Tabela de Conteúdos
1. [Objetivo](#objetivo)
2. [O que é?](#oque)
3. [Características do Flexbox](#caracteristicas)
   - [Display](#display)
   - [Justify-content](#justify-content)
   - [Align-items](#align-items)
   - [Flex-direction](#flex-direction)
   - [Align-content](#align-content)
4. [Características dos Flex Items](#características-dos-flex-items)
   - [Propriedade order](#propriedade-order)
   - [Align-self](#align-self)
   - [Propriedade flex-grow](#propriedade-flex-grow)
5. [Autoras](#autoras)

## Autoras:
* Carolina Sun Ramos Nantes de Castilho 
* Clara Beatriz Aguiar 
* Erica Gonçalves de Oliveira
* Laura Carolina Balbachan dos Santos 

<div id='objetivo'/> 
   
## Objetivo  

<p> O objetivo deste projeto é detalhar as características do modelo de layout Flexbox no CSS3, explicando como ele simplifica a criação de layouts responsivos. Abordaremos as propriedades essenciais para o controle do fluxo e posicionamento de elementos, proporcionando uma base sólida para o desenvolvimento de interfaces adaptáveis.</p>

<div id='oque'/> 
   
## O que é? 
Flexbox é um modelo de layout introduzido no CSS3 que simplifica a criação de estruturas de layout complexas e responsivas. Ele permite que os elementos filhos de um contêiner se ajustem automaticamente com base no espaço disponível.O Flexbox facilita o controle sobre o alinhamento, espaçamento e dimensionamento dos itens, tornando o desenvolvimento de layouts mais rápido e eficiente. É especialmente útil para garantir que interfaces funcionem bem em diferentes tamanhos de tela, de desktops a dispositivos móveis.

Flex container é o elemento pai que define o contexto flexível. Ele estabelece o eixo principal e o eixo transversal, ao longo dos quais os elementos filhos são alinhados e distribuídos. O contêiner flexível controla o alinhamento, o espaçamento entre os itens e como eles devem se comportar em relação ao espaço disponível. As propriedades aplicadas ao contêiner, como justify-content, align-items , flex-direction, align-content determinam como os elementos filhos serão organizados.

<div id='caracteristicas'/>

**Características do Flexbox**

<div id='display'/>
**Display:** 
   O Flexbox é ativado em um contêiner ao aplicar a propriedade `display` com os valores “flex” ou “inline-flex”. Quando o valor “flex” é utilizado, o contêiner se torna um bloco flexível (flex container), enquanto o valor “inline-flex” cria um contêiner flexível em linha. Esse contêiner flexível define um contexto no qual todos os elementos filhos diretos, chamados de “flex items”, são organizados de acordo com as regras do modelo Flexbox.
   
   ```css
   .container {
       display: flex;
   }
   ```

<div id='justify-content'/>
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





## Flex-direction 

A propriedade `flex-direction` no Flexbox define a direção na qual os itens flexíveis são organizados dentro de um contêiner. Ela pode alinhar os itens em uma linha horizontal (`row`), em uma coluna vertical (`column`), ou inverter essas direções (`row-reverse` e `column-reverse`). Essa característica permite que os desenvolvedores controlem como os itens são distribuídos no eixo principal, influenciando a ordem visual e o fluxo dos elementos, o que é essencial para criar layouts dinâmicos e responsivos.






## Align-content

A propriedade `align-content` é usada para alinhar linhas de itens dentro de um contêiner flexível. Mas, ela só funciona quando há várias linhas de itens. Isso acontece quando os itens "quebram" e vão para a linha de baixo. A propriedade `align-content` ajuda a decidir como essas linhas devem ser organizadas dentro do container. Você pode empurrá-las para cima, para baixo, colocá-las no meio, espalhá-las.


* **flex-start:** Coloca todas as linhas no início do contêiner, como se você empurrasse tudo para cima.*
```css
.container1 {
    align-content: flex-start;
}
```

![gato10](https://github.com/user-attachments/assets/eb95b21b-db70-46e8-b021-b4688db22166)

* **center:** Centraliza as linhas no meio do contêiner, como se você as colocasse no centro.*

```css
.container2 {
    align-content: center;
}
```

![gato11](https://github.com/user-attachments/assets/d79c8f1f-ea01-4f38-aac2-a48ba1b10c97)

* **flex-end:** Coloca todas as linhas no final do contêiner, como se você empurrasse tudo para baixo.*
```css
.container3 {
    align-content: flex-end;
}
```

![gato12](https://github.com/user-attachments/assets/bccfc720-0b21-445a-8700-4b4fe52d86e8)

* **stretch:** Estica as linhas para preencher todo o espaço disponível do contêiner. Isso faz com que cada linha se ajuste para ocupar o máximo de espaço.*
```css
.container4 {
    align-content: stretch;
}
```

![gato13](https://github.com/user-attachments/assets/8107eb25-0759-4c40-ae46-8ec1d59fd5b4)

* **space-between:** Espalha as linhas com o primeiro item no início e o último item no final, deixando espaço igual entre eles.*
```css
.container5 {
    align-content: space-between;
}
```

![gato14](https://github.com/user-attachments/assets/6e57a67d-5f86-482d-9fcb-b7634a198a1e)

* **space-around:** Coloca espaço igual ao redor de cada linha, como se houvesse uma pequena margem ao redor de cada linha.*
```css
.container6 {
    align-content: space-around;
}
```

![gato15](https://github.com/user-attachments/assets/c69ff4bb-4364-4b1e-99b7-7daff4d6535f)


## Características do Flex Items
Os itens flexíveis são os elementos filhos diretos de um contêiner flexível. Embora eles herdem as características do contêiner, podem ser ajustados individualmente usando propriedades como flex-grow, flex-shrink e flex-basis. Essas propriedades determinam como cada item cresce, encolhe e ocupa espaço dentro do contêiner. A flexibilidade dos itens permite um layout mais dinâmico e adaptável, assegurando que os elementos sejam distribuídos de forma eficiente, independentemente do conteúdo ou do tamanho da tela.

## Propriedade order
A propriedade `order` no Flexbox permite reorganizar a ordem visual dos itens flexíveis dentro de um contêiner, sem alterar a estrutura HTML. Ao atribuir valores positivos ou negativos, é possível mover os itens, com menores valores de `order` aparecendo antes dos maiores. Isso facilita a criação de layouts dinâmicos e responsivos.
* **Original:**
  
![image](https://github.com/user-attachments/assets/31e2b2ee-f0c8-4fdb-8b87-1fc00ff69145)


* **Utilizando Order:**

![image](https://github.com/user-attachments/assets/feeb75cf-722b-4373-bceb-b834c0a1dbe1)
```css
.mudar_ordem{
    display: flex;
}

.ordem0{
    order:0
}
.ordem1 {
    order: 1;
}

.ordem2 {
    order: 2;
}

.ordem3 {
    order: 3;
}

.ordem4 {
    order: 4;
}
```

## Align-self
A propriedade align-self em CSS é usada para ajustar o alinhamento de um item flexível dentro de um contêiner flexível, permitindo que você sobreponha o alinhamento padrão definido pelo contêiner pai. Esta propriedade aceita os mesmos valores que align-items e seus valores são usados para o item específico. </p>

* **Flex-Start:** Alinha o item ao início do contêiner.
  ```css
   .item{
      display:flex;
     }
   .align-self-start {
       align-self: flex-start;
   }
  ```
![image](https://github.com/user-attachments/assets/88163009-3063-4549-9c25-168a366f866e)


  
* **Center:** Alinha o item ao centro do contêiner. (gato cinza)
```css
   .item{
      display:flex;
   }
   .align-self-center {
       align-self: center;
   }
```
![image](https://github.com/user-attachments/assets/2d7e1650-ba99-4f4d-ad9b-f369ac3e138e)



* **Flex-end:** Alinha o item ao final do contêiner. (gato laranja)
```css
   .item{
      display:flex;
}
   .align-self-end {
       align-self: flex-end;
}

```
![image](https://github.com/user-attachments/assets/54414a2a-439e-40e8-8123-cdf59bb5dbaf)

## Propriedade flex-grow
A propriedade `flex-grow` determina a capacidade de um item flexível de se expandir para preencher o espaço disponível dentro de um contêiner flexível. O valor atribuído a essa propriedade é um número sem unidade, utilizado para calcular a proporção de crescimento. Esse valor define a quantidade de espaço livre no contêiner que o item deve ocupar.

Se todos os itens tiverem flex-grow definido como 1, o espaço extra no contêiner será distribuído igualmente entre eles. Caso um item tenha o valor 2 (gato branco), ele tentará ocupar o dobro do espaço disponível em comparação aos itens com valor 1.

```css
   .item{
      display:flex;
}
   .item-flex-grow{
    flex-grow: 1;
}
   .item-flex-grow2{
    flex-grow: 2;
}
}

```

![gato-grow](https://github.com/user-attachments/assets/40834f4d-322a-4c51-a585-509925d4dd81)








