# HTML Carousel Grid Layout

Este repositório contém um exemplo de um layout de grade combinado com um carrossel implementado em HTML e CSS.

## Visão Geral

O objetivo deste projeto é demonstrar como criar um layout de grade responsivo que também funcione como um carrossel de imagens. O layout é desenvolvido com HTML5 e CSS3, utilizando técnicas modernas para garantir compatibilidade e flexibilidade.

## Estrutura do Projeto

### HTML

O arquivo HTML define a estrutura básica do layout da grade e do carrossel. Aqui está uma visão geral da estrutura HTML:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carousel Grid Layout</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="carousel">
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img src="image1.jpg" alt="Image 1">
            </div>
            <div class="carousel-item">
                <img src="image2.jpg" alt="Image 2">
            </div>
            <div class="carousel-item">
                <img src="image3.jpg" alt="Image 3">
            </div>
        </div>
        <button class="carousel-control prev">Previous</button>
        <button class="carousel-control next">Next</button>
    </div>
</body>
</html>
```

### CSS

O arquivo CSS estiliza a grade e o carrossel para garantir que sejam responsivos e visualmente atraentes. Abaixo estão alguns trechos-chave do CSS:

```css
body {
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
}

.carousel {
    width: 80%;
    max-width: 600px;
    overflow: hidden;
    position: relative;
}

.carousel-inner {
    display: flex;
    transition: transform 0.5s ease-in-out;
}

.carousel-item {
    min-width: 100%;
    box-sizing: border-box;
}

.carousel img {
    width: 100%;
    display: block;
}

.carousel-control {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background-color: rgba(0, 0, 0, 0.5);
    color: white;
    border: none;
    padding: 10px;
    cursor: pointer;
}

.carousel-control.prev {
    left: 10px;
}

.carousel-control.next {
    right: 10px;
}
```

## Funcionamento do HTML

- **Estrutura Principal**: A estrutura HTML consiste em um `div` principal com a classe `carousel`, que contém os elementos do carrossel.
- **Itens do Carrossel**: Dentro do `div.carousel-inner`, cada `div.carousel-item` representa um item do carrossel. A primeira imagem possui a classe `active` para ser exibida inicialmente.
- **Controles do Carrossel**: Dois botões (`button.carousel-control prev` e `button.carousel-control next`) são adicionados para navegar entre os itens do carrossel.

## Funcionamento do CSS

- **Estilização Básica**: O `body` é estilizado para centralizar o carrossel na página.
- **Carrossel**: A `div.carousel` define a área visível do carrossel, com `overflow: hidden` para ocultar os itens que não estão ativos.
- **Itens do Carrossel**: `div.carousel-inner` usa `display: flex` para alinhar os itens horizontalmente. A transição suave é garantida por `transition: transform 0.5s ease-in-out`.
- **Controle de Navegação**: Os botões de navegação são posicionados absolutamente no centro vertical do carrossel e são estilizados para serem semi-transparentes.

## Instruções de Uso

1. Clone o repositório:
   ```sh
   git clone https://github.com/jhonieldorschulz/html-carousel-grid-layout.git
   ```
2. Navegue até o diretório do projeto:
   ```sh
   cd html-carousel-grid-layout
   ```
3. Abra o arquivo `index.html` em um navegador para ver o carrossel em ação.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e enviar pull requests.

---

Isso deve fornecer uma explicação clara e detalhada do funcionamento do HTML e CSS no projeto, ajudando os usuários a entenderem melhor como o layout foi implementado.