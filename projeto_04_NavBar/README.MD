Barra de Navegação com Flexbox – Projeto Front-End
Descrição

Este projeto apresenta uma barra de navegação (Navbar) moderna construída com CSS Flexbox.

O cabeçalho contém:

Logo à esquerda

Links de navegação centralizados ao lado do logo

Feedback visual ao passar o mouse nos links (:hover)

Indicação do link ativo para mostrar a página atual

O objetivo é aprofundar o conhecimento em Flexbox, especialmente justify-content, align-items, gap e pseudo-classes como :hover.

Visual do Projeto

Header limpo e centralizado

Logo e menu lado a lado, centralizados

Links com efeito hover e borda inferior animada

Link “Home” ativo destacando a página atual

Estrutura de Arquivos
projeto-04-navbar/
├── index.html
└── style.css

Como Abrir o Projeto

Clone ou baixe o projeto.

Abra index.html em qualquer navegador moderno.

Observe o cabeçalho com logo e links centralizados.

Passe o mouse sobre os links para ver o efeito hover.

Explicação do Código
index.html

<header>: semântico para cabeçalhos.

<div class="header-container">: agrupa logo e navegação para centralização.

<nav> e <ul>: estrutura da navegação, com <li> e <a>.

<a class="active">: indica o link da página atual.

style.css
Flexbox
.header-container {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 50px;
}


display: flex: transforma o container em Flex Container.

justify-content: center: centraliza logo + nav.

align-items: center: alinha verticalmente logo e links.

gap: espaço uniforme entre logo e menu.

Links
.main-nav a:hover {
    color: #007bff;
    border-bottom: 2px solid #007bff;
}

.main-nav a.active {
    color: #007bff;
    border-bottom: 2px solid #007bff;
}


Hover: muda cor e adiciona borda inferior.

Active: indica visualmente a página atual.

Desafios Implementados

Link ativo:

O link “Home” possui a classe .active.

Centralização do layout:

Logo e menu estão dentro de .header-container centralizado com Flexbox.