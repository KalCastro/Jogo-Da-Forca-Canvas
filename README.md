# Jogo-Da-Forca-Canvas

Este é um jogo da forca feito em HTML, CSS e JavaScript. O objetivo é adivinhar a palavra secreta antes que o boneco seja enforcado.

## Funcionalidades

- O jogo escolhe uma palavra aleatória de uma lista de palavras pré-definidas.
- 
- O jogador pode digitar qualquer letra do teclado para tentar acertar a palavra.
- 
- O jogo mostra as letras acertadas e as tentativas erradas na tela.
- 
- O jogo desenha o boneco conforme o número de erros.
- 
- O jogo termina quando o jogador acerta a palavra ou quando o boneco é enforcado.
- 
- O jogo mostra uma mensagem de vitória ou derrota na tela.

## Demonstração

https://github.com/KalCastro/Jogo-Da-Forca-Canvas/assets/129300311/e23bdda7-dfac-4085-b21d-dee0b8920fce

## Colaboradores

- Kauã de Castro(KalCastro)
- Vincenzo Monaco(VincenMonaco)

## Tecnologias utilizadas

- HTML
- CSS
- JavaScript

## HTML Iniciar(Iniciar.html)
## Estrutura Básica

O código começa com a declaração do tipo de documento (`<!DOCTYPE html>`), que é HTML5. Em seguida, temos a tag `<html>` com o atributo `lang` definido como "pt-br", indicando que o idioma do documento é o português do Brasil.

### `<head>`

Dentro da tag `<head>`, temos:

- A tag `<meta charset="UTF-8">`, que define a codificação de caracteres do documento como UTF-8.
- A tag `<title>` que define o título do documento como "Jogo da Forca".

### `<style>`

Os estilos CSS são definidos dentro da tag `<style>`. Eles incluem:

- Um plano de fundo para o corpo do documento que usa uma imagem de uma floresta.
- Estilos para o botão `"Iniciar Jogo"`, incluindo largura, altura, raio da borda e margem superior.

### `<body>`

Dentro da tag `<body>`, temos:

- Um cabeçalho `<h1>` e um subcabeçalho `<h2>` que dão as boas-vindas ao usuário e instruem sobre como iniciar o jogo.
- Um botão com o id `"inicioButton"` que o usuário pode clicar para iniciar o jogo.

### `<script>`

Por fim, temos a tag `<script>` que vincula a um arquivo JavaScript externo chamado "Iniciar.js".

## Script Iniciar(Iniciar.js)
## Descrição

Este script adiciona um evento de clique a o botão com o id `"inicioButton"` na página HTML Iniciar. 

## Estrutura

- `const iniciarButton = document.getElementById("inicioButton");`: Esta linha de código seleciona o elemento HTML com o ID "inicioButton" e o armazena na constante `iniciarButton`.

- `iniciarButton.addEventListener("click", () => {...});`: Esta linha de código adiciona um ouvinte de eventos ao botão. O ouvinte "escuta" por um evento de clique.

- `window.location.href = "forca.html";`: Quando o botão é clicado, o usuário é redirecionado para a página "forca.html".

## HTML Forca("forca.html")
## Descrição

O código começa com a declaração do tipo de documento (`<!DOCTYPE html>`), que é HTML5. Em seguida, temos a tag `<html>` com o atributo `lang` definido como "pt-br", indicando que o idioma do documento é o português do Brasil.

## Estrutura

### `<head>`

Esta seção define o título da página e o estilo CSS. O título da página é "Jogo da Forca". O estilo CSS define a imagem de fundo, o tamanho da imagem de fundo, a repetição da imagem de fundo, o anexo de fundo e o alinhamento dos itens.

### `<body>`

Esta seção contém o conteúdo principal da página. Inclui um título `<h2>` que solicita ao usuário para digitar qualquer letra, um elemento `<canvas>` onde o jogo da forca é desenhado, e um botão que recarrega a página quando clicado, permitindo ao usuário passar a palavra.

### `<script>`

Esta seção vincula um arquivo JavaScript externo chamado "script.js". Este arquivo contém a lógica do jogo.

## Script Forca(script.js)
## Descrição

O código inclui funções para desenhar o boneco da forca e verificar as tentativas do usuário.

### Variáveis

- `palavras`: Uma lista de palavras que podem ser escolhidas para o jogo.

- `quantiErros`: Contador de erros do usuário.

- `acertos`: Contador de acertos do usuário.

- `tentativas`: String que armazena as tentativas do usuário.

- `palavraSecreta`: A palavra que o usuário deve adivinhar, escolhida aleatoriamente da lista de palavras.

### Funções

- `teclaPressionada()`: Esta função é chamada sempre que uma tecla é pressionada. Ela verifica se a tecla pressionada está na palavra secreta e atualiza os contadores de acertos e erros.

- `adiTentativa()`: Adiciona a tecla pressionada à string de tentativas.

- `verificaFimJogo()`: Verifica se o jogo terminou, seja porque o usuário adivinhou a palavra ou porque o número máximo de erros foi atingido.

- `dePoste()`, `deBarraSuperior()`, `deApoio()`, `deTracos()`: Estas funções desenham a forca.

- `deBoneco(quantiErros)`: Desenha o boneco da forca, adicionando partes do corpo com base no número de erros.

- `deCabeca()`, `deTronco()`, `deBracoEs()`, `deBracoDi()`, `dePernaEs()`, `dePernaDi()`: Estas funções desenham as partes do corpo do boneco da forca.

## Como jogar
O usuário deve pressionar as teclas correspondentes às letras que acredita estarem na palavra secreta. Se a letra estiver na palavra, ela será revelada. Se não estiver, uma parte do corpo será adicionada ao boneco da forca. O jogo termina quando o usuário adivinha a palavra ou quando o boneco da forca está completo.




