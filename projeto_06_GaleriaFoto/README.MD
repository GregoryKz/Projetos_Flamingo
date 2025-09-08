Olá, time!

Até agora, aprendemos a alinhar itens com Flexbox. Hoje, vamos explorar algo ainda mais poderoso: o CSS Grid Layout. Este módulo nos permite criar grades e layouts complexos de forma simples e flexível, ajustando automaticamente o número de colunas conforme o tamanho da tela.

O objetivo deste projeto é construir uma galeria de fotos responsiva, onde as imagens se organizam sozinhas em colunas e linhas sem precisar de @media queries. Além disso, aplicaremos object-fit e efeitos de hover para tornar a experiência mais elegante.

Estrutura de Arquivos
projeto-06-grid-gallery/
├── assets/
│   ├── foto-1.jpg
│   ├── foto-2.jpg
│   ├── foto-3.jpg
│   ├── foto-4.jpg
│   ├── foto-5.jpg
│   └── foto-6.jpg
├── index.html
└── style.css

HTML da Galeria

As imagens são envolvidas por <div class="gallery-item"> dentro de um container com class gallery-grid. Cada imagem possui um atributo alt, que descreve o conteúdo da foto para acessibilidade e SEO.

Lista de descrições usadas nas imagens:

"Pôr do sol sobre um campo de flores amarelas"

"Montanhas cobertas de neve sob céu azul claro"

"Cachoeira caindo entre pedras e vegetação verdejante"

"Café da manhã em uma mesa de madeira com frutas e café"

"Praia deserta com areia branca e mar turquesa ao fundo"

"Cidade à noite com luzes brilhantes e arranha-céus iluminados"

CSS – O foco no Grid

Container da Galeria

.gallery-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}


repeat(auto-fit, minmax(250px, 1fr)): cria automaticamente colunas que têm no mínimo 250px e ocupam igualmente o espaço disponível.

gap: 20px: espaçamento uniforme entre linhas e colunas.

Itens da Galeria

.gallery-item {
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 5px 10px rgba(0,0,0,0.15);
}
.gallery-item img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
    transition: transform 0.4s ease;
}
.gallery-item img:hover {
    transform: scale(1.05);
}


object-fit: cover: garante que a imagem preencha seu container sem distorcer.

overflow: hidden e border-radius: mantém os cantos arredondados sem que a imagem "vaze".

transition e hover: efeito de zoom suave ao passar o mouse.

Desafios para praticar

Adicionar um Campo de Mensagem

Crie um <textarea> dentro de um .form-group para permitir que o usuário escreva uma mensagem.

Use padding, borda e estilo consistente com o resto da galeria.

Checkbox de Termos

Adicione um checkbox para "Eu aceito os termos e condições".

Use display: flex e align-items: center para alinhar o quadradinho ao texto da label.

Responsividade Avançada

Experimente alterar minmax(250px, 1fr) para ver como o número de colunas se adapta.

Tente adicionar mais fotos e veja o grid se ajustar automaticamente.

Observações

Este projeto ensina CSS Grid Layout responsivo, object-fit, hover effects, e boas práticas de HTML semântico e acessibilidade.

É um ótimo passo para criar layouts complexos sem precisar de frameworks ou float.