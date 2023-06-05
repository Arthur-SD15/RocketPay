<h1 align="center">
  RocketPay
</h1>

<p align="center">
  <a href="#-Projeto">Projeto</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-Layout">Layout&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-Aprendizado">Aprendizado&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-Pré-requesitos">Pré-requesitos</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-Executar Projeto">Executar</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-Creditos">Créditos</a>
</p>
  
<p align="center">
  <img alt="rocketpay" src=".github/project.png" width="100%">
</p>

## 💻 Projeto

Desenvolvi uma aplicação chamada RocketPay durante um evento da Rocketseat, focado no ensino de tecnologias web. O RocketPay é um componente que simula o preenchimento de formulários de cartões de crédito, durante o desenvolvimento utilizamos máscaras(mask) visando padronizar dados, como, os números dos cartões de crédito e também trabalhamos as atualizações dinâmicas de elementos HTML via DOM. A aplicação reconhece automaticamente a bandeira do cartão com base no número digitado e exibe a logo correspondente. Atualmente, suportamos as bandeiras Mastercard, Elo e Visa.

O RocketPay é uma aplicação inovadora que simplifica o preenchimento de formulários de cartões de crédito. Com suas máscaras de input e reconhecimento automático da bandeira, ele melhora a experiência do usuário. Experimente o RocketPay em seus projetos web e otimize o processo de inserção de informações de cartão de crédito.

## 🔖 Layout

Você pode visualizar o layout do projeto através [desse link](https://www.figma.com/file/gpqavL469k0pPUGOmAQEM9/Explorer-Lab-%2301/duplicate). É necessário ter conta no [Figma](https://figma.com) para acessá-lo.

## 🧠 Aprendizado
    
Na primeira aula, consegui aprender algumas ideias novas e aperfeiçoar alguns conceitos. Durante a aula, obtive entendimento sobre alguns conceitos de DOM, que é a representação do nosso documento HTML como um objeto JavaScript. Todos os objetos JavaScript possuem propriedades (atributos) e funcionalidades (métodos). Utilizamos o DOM para manipular o HTML com JavaScript.
    
Durante a primeira aula, também consegui relembrar alguns conceitos, como o de selecionar um elemento HTML específico usando JavaScript, que é feito por meio do método document.querySelector(). Veja:

```bash
// Seleciona o primeiro elemento path dentro de um svg, o primeiro path dentro do segundo g dentro do primeiro g que possui a classe .cc-bg
const ccBgColor01 = document.querySelector(".cc-bg svg > g g:nth-child(1) path")
    
// Seleciona o primeiro elemento path dentro de um svg, o segundo path dentro do segundo g dentro do primeiro g que possui a classe .cc-bg
const ccBgColor02 = document.querySelector(".cc-bg svg > g g:nth-child(2) path")
```
 
Utilizamos a função setCardType(type) que é definida com um parâmetro type. Essa função é usada para definir o tipo de cartão de crédito e ajustar a aparência correspondente. Em seguida, é declarado um objeto colors que mapeia diferentes tipos de cartão de crédito a cores específicas.  Dentro da função setCardType(type), o método setAttribute() é usado para alterar o atributo fill dos elementos selecionados. setAttribute("fill", colors[type][0]) define a cor de preenchimento do primeiro elemento selecionado (ccBgColor01), e setAttribute("fill", colors[type][1]) define a cor de preenchimento do segundo elemento selecionado (ccBgColor02).
    
Na segunda aula, aprendi sobre o IMask, uma ferramenta utilizada para padronizar dados. Também explorei o uso de expressões regulares, que permitem buscar padrões dentro de um texto. Nesse contexto, utilizei regex para definir padrões relacionados a números de cartões e suas respectivas bandeiras. A seguir, são apresentados exemplos de expressões regulares:

```bash
// Bandeira Visa
/^4\d{0,15}/
//Inicia com '4' seguido de um dígito que pode se repetir de 0 até 15 ocorrências
4234234423432344
    
// Bandeira MasterCard
/(^5[1-5]\d{0,2}|^22[2-9]\d|^2[3-7]\d{0,2}\d{0,12})/
//Inicia com 5, seguido de um dígito entre 1 e 5, seguido de 0 ou mais 2 dígitos. Ou, inicia com 22, seguido de um dígito entre 2 e 9, seguido de 0 ou mais 1 dígito. Ou, inicia com 2, seguido de um dígito entre 3 e 7, seguido de 0 ou mais 2 dígitos. Todos seguidos por 12 dígitos.
5353535353535353
2323232323232323
2237235728362235
```
Dei uma grande resumida neste pequeno texto, em relação ao meu aprendizado durante o desenvolvimento dessa aplicação. No entanto, acabei deixando de fora algumas ideias novas, como a propriedade dispatch.
    
## 📝 Pré-requesitos

Antes de baixar o projeto você vai precisar ter instalado na sua máquina as seguintes ferramentas:

- [Git](https://git-scm.com)
- [NodeJS](https://nodejs.org/en/)
- [NPM](https://www.npmjs.com/)

## 🗂 Executar Projeto

```bash
# Clonar Projeto.
$ https://github.com/Arthur-SD15/RocketPay.git

# Baixar as dependencias.
$ npm install

# Executar.
$ npm run dev

 ```
 
 ## 💳 Créditos 

Os verdadeiros créditos vão para a plataforma <a href="https://www.googleadservices.com/pagead/aclk?sa=L&ai=DChcSEwjD07f3k6v_AhUaQEgAHagFC_sYABAAGgJjZQ&ohost=www.google.com&cid=CAESauD2mS-qgpZJNt9tjZPCmAM6Z7x7wR4ED4k8AJdPmR4yoVOEGMTl0dEl5fHkZ6KVLG6UtjE9CEzJ72ZXL10C6z0ZyIwwuPZmtQcQp5ZUe0oRsV37dUrEhN-fUYxb-kFhLWon6je3SPcPDAE&sig=AOD64_1qSoRglAv6JJdCm9_r5hunRSY1fQ&q&adurl&ved=2ahUKEwiTo7L3k6v_AhUEILkGHZrcDkQQ0Qx6BAgIEAE">Rocketseat</a> e seus professores, que transmitiram o conhecimento com excelência.
