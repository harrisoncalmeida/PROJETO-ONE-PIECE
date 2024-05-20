# PROJETO ONE PIECE

### ONE PIECE

Projeto One Piece, desenvolvido por meio de uma imersão no YouTube em parceria com o canal Dev em Dobro. Durante essa experiência, aprendemos conceitos fundamentais de HTML e CSS, além de explorarmos alguns princípios básicos de JavaScript.

![Página One Piece](/SRC/Img%20readme/Página%20ONE%20PIECE.jpeg)

Neste projeto, apresentamos descrições de alguns dos principais personagens do anime 'One Piece'. Cada personagem é destacado com uma imagem de fundo, acompanhada por sua descrição e nome.

Criamos também uma lista, com botões e ao clicar em um botão, o botão e o personagem correspondente sejam destacados. Com isso, apenas um botão e um personagem são selecionados por vez.

* Segue a explicação para a seleção dos botões

![Função 01](/SRC/Img%20readme/função%2001.jpeg)

***const botoes = document.querySelectorAll(‘.botao’);***
No código acima, estamos selecionando todos da classe ‘botao’ e armazenado em uma variável chamada ‘botoes’.


***const personagens = document.querySelectorAll(‘.personagem’);***
Esse código é a mesma função do código acima, com isso, vamos selecionar todos da classe ‘personagem’ e armazenar em uma variável chamada ‘personagens’. 
	
![Função 01](/SRC/Img%20readme/função%2002.jpeg)

***botoes.forEach((botao, indice) => { ... });***
Esse código vai percorre cada elemento na NodeList ‘botoes’ que criamos, passando o elemento atual ‘botao’ e seu índice para a função de callback. 

callback: São funções passadas como argumentos para outras funções.

***botao.addEventListener("click", () => { ... });***
Já aqui, estamos adicionando um evento de clique a cada botão. Quando um botão é clicado, a função de callback é executada.

***desselecionarBotao();***
Chama a função para remover a classe selecionada do botão que estiver atualmente selecionado.

***desselecionarPersonagem();***
Chama a função para remover a classe selecionada do personagem que estiver atualmente selecionado.

***botao.classList.add("selecionado");***
Adiciona a classe selecionada ao botão que foi clicado.

***personagens[indice].classList.add("selecionado");***
Adiciona a classe selecionada ao personagem correspondente ao índice do botão clicado.

![Função 01](/SRC/Img%20readme/função%2003.jpeg)

***function desselecionarPersonagem() { const personagemSelecionado = document.querySelector(".personagem.selecionado"); }***

Sua função é selecionar o elemento ‘personagem’ que atualmente tem a classe selecionado.personagemSelecionado.classList.remove("selecionado"); e remover a classe ‘selecionado’ desse elemento.


***function desselecionarBotao() { const botaoSelecionado = document.querySelector(".botao.selecionado");}***

Sua função é selecionar o elemento ‘botao’ que atualmente tem a classe selecionado.
botaoSelecionado.classList.remove("selecionado"); e remove a classe selecionado desse elemento.