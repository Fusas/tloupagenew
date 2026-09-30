# The Last of Us Parte II — Landing Page

Landing page de estudo inspirada em The Last of Us Parte II, feita só com **HTML e CSS**.

## Animações
- **Entrada do hero:** a imagem surge do escuro com zoom lento e o título aparece letra por letra com fade e desfoque.
- **Neblina:** camada de névoa animada passando pela cena.
- **Profundidade no título:** uma cópia da imagem recortada no tronco da árvore (`clip-path`) fica na frente do título, então as letras parecem estar atrás da árvore.
- **Cards:** ao passar o mouse, o card sobe, a foto sai do preto e branco para colorida, aproxima e a descrição aparece. Ao rolar, eles entram um depois do outro.
- **Faixa infinita:** "ENDURE AND SURVIVE" correndo sem parar e, embaixo, os nomes das cidades no sentido contrário. Pausa ao passar o mouse.
- **Vaga-lumes:** segunda cena presa na tela, com o texto embaixo à direita (`cena-direita cena-baixo`) para não cobrir o símbolo na parede.
- **Infectados:** os 4 estágios da infecção em cards, ligados por uma linha que cresce ao rolar. As fotos saem do preto e branco para coloridas no hover. Card sem foto: troque o `<div class="card-vazio">` por um `<img>`.
- **Chamada final:** imagem em tela cheia que se afasta ao entrar, título "Sobreviva." e botões para a loja e o trailer.
- **Números:** contam de 0 até o valor final conforme entram na tela (`@property` + `counter()`), e a linha de cima cresce junto.
- **Rodapé:** assinatura "fusas." com o ponto piscando no hover e selo giratório em SVG.
- **Rolagem:** o título sobe e some ao rolar. Nas cenas seguintes, o conteúdo fica fixo na tela (`position: sticky`) enquanto a imagem sai do escuro e os textos entram um de cada vez (`animation-timeline`).
- Respeita `prefers-reduced-motion` para quem desativa animações no sistema.

> As animações ligadas à rolagem funcionam no Chrome, no Edge e no Safari mais recente. Nos outros navegadores o conteúdo aparece normalmente, sem o efeito.

## Prévia ao compartilhar o link
As tags `og:` no `<head>` fazem o link mostrar a imagem `img/preview.jpg` (1200×630), o título e a descrição no WhatsApp, Discord etc. Elas apontam para `https://fusas.github.io/tloupagenew/`, então só funcionam com o site publicado nesse endereço. Para testar depois de publicar: [opengraph.xyz](https://www.opengraph.xyz).

## Adicionar uma nova cena
Copie um bloco `<section class="cena">` no `index.html`, troque a imagem e os textos. Para o texto ficar do lado direito, use `class="cena cena-direita"`.

## Estrutura
```
index.html
style.css
img/     imagens
fonts/   fonte The Last Of Us Rough (títulos)
```

## Créditos
Projeto de estudo, sem fins comerciais. The Last of Us e imagens © Naughty Dog / Sony Interactive Entertainment.
Fonte "The Last Of Us Rough" © MedRida.
