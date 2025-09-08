Componente de Post com Flexbox – Projeto Front-End
Descrição

Este projeto apresenta um componente de post de blog com imagem à esquerda e bloco de texto à direita, construído usando CSS Flexbox.

O objetivo é aprender como alinhar itens horizontalmente dentro de um contêiner, dominar o uso de display: flex, gap, align-items e aplicar técnicas de responsividade básica.

O layout também inclui boas práticas de acessibilidade, com atributos alt em imagens e textos semanticamente corretos.

Visual do Projeto

Card centralizado na tela.

Imagem quadrada à esquerda e texto à direita.

Título e resumo do post com padding interno.

Layout responsivo: em telas pequenas, os itens se empilham verticalmente.

Estrutura de Arquivos
projeto-03-flexbox-post/
├── assets/
│   └── laptop-codigo.jpg    # Imagem representativa do post
├── index.html
└── style.css

Como Abrir o Projeto

Baixe ou clone o projeto.

Abra o arquivo index.html em qualquer navegador moderno.

Observe o card de post com imagem e texto alinhados horizontalmente.

Reduza a largura da janela para testar a responsividade.

Explicação do Código
index.html

<article>: elemento semântico para posts de blog.

<img src="..." alt="...">: insere a imagem com descrição para acessibilidade.

<div class="post-content">: agrupa título e resumo do post, facilitando padding e layout.

<h2> e <p>: estrutura semântica de título e resumo do conteúdo.