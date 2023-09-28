# Índice

## HTML (HyperText Markup Language)

1. [Introdução ao HTML](#1-introdução-ao-html)

* O que é HTML?
* Estrutura básica de um documento HTML
* Tags, elementos e atributos

2. [Estrutura de um Documento HTML](#2-estrutura-de-um-documento-html)

* Doctype
* Elemento ```<html>```
* Elemento ```<head>``` (meta tags, título)
* Elemento ```<body>```

3. [Texto e Formatação](#3-texto-e-formatação)

* Parágrafos (```<p>```)
* Títulos (```<h1>``` a ```<h6>```)
* Texto em negrito (```<strong>```) e itálico (```<em>```)
* Quebras de linha (```<br>```)
* Comentários (```<!-- -->```)

4. [Listas](#4-listas)

* Listas ordenadas (```<ol>```)
* Listas não ordenadas (```<ul>```)
* Listas de definição (```<dl>```)

5. [Links](#5-links)

* Hiperlinks (```<a>```)
* Âncoras e URLs
* Links internos e externos

6. [Imagens](#6-imagens)

* Inserindo imagens (```<img>```)
* Atributos alt e src
* Imagens responsivas

7. [Formulários](#7-formulários)

* Elemento ```<form>```
* Campos de entrada de texto (```<input>```)
* Botões (```<button>```)
* Caixas de seleção (```<select>```)
* Botões de opção (```<radio>```) e caixas de verificação (```<checkbox>```)
* Envio de formulário

8. Documentação: https://www.w3schools.com/TAGS/default.asp

##  CSS (Cascading Style Sheets)

1. [Introdução ao CSS](#1-introdução-ao-css-cascading-style-sheets)

* O que é CSS?
* Vantagens de usar CSS

2. [Seletores e Propriedades](#2-seletores-e-propriedades-css)

* Seletores de elemento, classe e ID
* Definindo propriedades de estilo
* Comentários em CSS

3. [Estilos Inline, Incorporados e Externos](#3-estilos-inline-incorporados-e-externos-em-css)

* Uso de estilos inline
* Incorporando estilos com a tag ```<style>```
* Vinculando um arquivo CSS externo

4.[Formatação de Texto](#4-formatação-de-texto-em-css)

* Tamanho de fonte
* Cor de texto e de fundo
* Espaçamento entre linhas e margens

5. [Box Model](#5-modelos-de-caixas-box-model-em-css)

* Margem, borda, preenchimento (margin, border, padding)
* Tamanho e modelo de caixa (box-sizing)

6. [Layout e Posicionamento](#6-posicionamento-e-layout-em-css)

* Posicionamento estático, relativo, absoluto e fixo
* Display (block, inline, inline-block)
* Modelos de layout (flexbox e grid)

7. [Cores e Fundos](#7-cores-e-fundos-em-css)

* Definindo cores (hexadecimal, RGB, nomes)
* Imagens de fundo (background-image)
* Gradientes

8. [Pseudo-classes e Pseudo-elementos](#8-pseudo-classes-e-pseudo-elementos-em-css)

* Uso de :hover, :active, :focus
* ::before e ::after

9. [Media Queries](#9-media-queries-em-css)

* Criando layouts responsivos
* Conceito de breakpoints

10. [Animações e Transições (opcional)](#10-animações-e-transições-em-css-opcional)

* Criando animações com keyframes
* Aplicando transições suaves


## Site Modelo treinamento

https://melohenrique-room.netlify.app/

# HTML (HyperText Markup Language)

## 1. Introdução ao HTML

### O que é HTML?

HTML, sigla para HyperText Markup Language, é uma linguagem de marcação usada para criar páginas da web. Ele permite estruturar o conteúdo de uma página, incluindo textos, imagens, links e outros elementos, de forma organizada e semântica.

### Estrutura básica de um documento HTML

Um documento HTML é composto por uma estrutura básica que inclui elementos essenciais:

```html
<!DOCTYPE html> <!-- Define o tipo de documento HTML5 -->
<html>
<head>
    <meta charset="UTF-8"> <!-- Define a codificação de caracteres -->
    <title>Título da Página</title> <!-- Define o título da página exibido na aba do navegador -->
</head>
<body>
    <!-- Conteúdo da página vai aqui -->
</body>
</html>
```

### Tags, elementos e atributos

* Tags: São elementos fundamentais em HTML e são usados para marcar partes específicas do conteúdo, como títulos, parágrafos, imagens, etc. Exemplo: ```<h1>```Meu Título```</h1>```

* Elementos: São combinações de tags que englobam o conteúdo relacionado. Por exemplo, o elemento de lista não ordenada ```<ul>``` engloba várias tags de item de lista ```<li>```.

* Atributos: São informações adicionais fornecidas às tags para modificar seu comportamento ou aparência. Exemplo: ```<img src="imagem.jpg" alt="Descrição da Imagem">```.

Lembre-se de que HTML é uma linguagem de marcação estrutural, não de estilo. Para estilizar elementos, você usaria CSS (Cascading Style Sheets).

## 2. Estrutura de um Documento HTML

A estrutura básica de um documento HTML é composta pelo Doctype, o elemento ```<html>```, o elemento ```<head>```, e o elemento ```<body>```. Isso estabelece a base para a criação de uma página da web.

* Doctype: O Doctype é a primeira linha de um documento HTML e define o tipo de documento que está sendo usado. Para documentos HTML5, usamos o seguinte Doctype:

```html
<!DOCTYPE html>
```

* Elemento ```<html>```: O elemento ```<html>``` é o contêiner raiz de todo documento HTML. Ele engloba todo o conteúdo da página e define o idioma padrão da página usando o atributo lang.

```html
<html lang="pt-BR">
    <!-- Conteúdo da página vai aqui -->
</html>
```

* Elemento ```<head>```: O elemento ```<head>``` contém informações sobre o documento, como meta tags, links para folhas de estilo CSS e o título da página.

```html
<head>
    <meta charset="UTF-8">
    <title>Título da Página</title>
    <!-- Outros elementos do cabeçalho podem ser incluídos aqui -->
</head>
```

* Elemento ```<body>```: O elemento ```<body>``` contém o conteúdo visível da página, incluindo textos, imagens, links e outros elementos.

```html
<body>
    <h1>Meu Título</h1>
    <p>Este é um parágrafo de exemplo.</p>
    <!-- Outros elementos do corpo da página vão aqui -->
</body>
```

## 3. Texto e Formatação

* Parágrafos (```<p>```): Os parágrafos são usados para estruturar o texto em blocos coesos.

```html
<p>Este é um parágrafo de exemplo.</p>
```

* Títulos (```<h1>``` a ```<h6>```): Os títulos são usados para definir a hierarquia de cabeçalhos, do ```<h1>``` (mais importante) ao ```<h6>``` (menos importante).

```html
<h1>Título Principal</h1>
<h2>Subtítulo</h2>
```

* Texto em Negrito (```<strong>```) e Itálico (```<em>```): As tags ```<strong>``` e ```<em>``` são usadas para enfatizar o texto.

```html
<p>Este é um texto <strong>em negrito</strong> e este é um texto <em>itálico</em>.</p>
```

* Quebras de Linha (```<br>```): A tag ```<br>``` é usada para inserir uma quebra de linha dentro do texto.

```html
<p>Esta é a primeira linha.<br>Esta é a segunda linha.</p>
```

* Comentários (```<!-- -->```): Os comentários são usados para adicionar notas ou descrições no código HTML que não são visíveis na página.

```html
<!-- Este é um comentário de exemplo -->
```

## 4. Listas

* Listas Ordenadas (```<ol>```): As listas ordenadas são usadas para criar listas numeradas, onde cada item é automaticamente numerado.

```html
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ol>
```

* Listas Não Ordenadas (```<ul>```): As listas não ordenadas são usadas para criar listas com marcadores, onde cada item é precedido por um marcador.

```html
<ul>
    <li>Item A</li>
    <li>Item B</li>
    <li>Item C</li>
</ul>
```

* Listas Aninhadas: Você também pode criar listas aninhadas, colocando uma lista dentro de um item de lista.

```html
<ul>
    <li>Item 1</li>
    <li>Item 2
        <ul>
            <li>Subitem 1</li>
            <li>Subitem 2</li>
        </ul>
    </li>
    <li>Item 3</li>
</ul>
```

## 5. Links

* Hiperlinks (```<a>```): A tag ```<a>``` é usada para criar hiperlinks, permitindo que os visitantes da página cliquem em um texto ou imagem para navegar para outra página da web ou recurso.

```html
<a href="https://www.exemplo.com">Visitar Exemplo.com</a>
```

* Âncoras e URLs: O atributo href dentro da tag ```<a>``` especifica o URL de destino para o link.

* Links Internos: Além de URLs externos, você pode criar links internos dentro da mesma página usando âncoras.

```html
<a href="#secao2">Ir para Seção 2</a>
...
<h2 id="secao2">Seção 2</h2>
```

* Links de Email: Você também pode usar a tag ```<a>``` para criar links de email.

```html
<a href="mailto:exemplo@email.com">Enviar um Email</a>
```

* Links para Downloads: Para permitir o download de arquivos, você pode usar a tag ```<a>``` com o atributo download.

```html
<a href="documento.pdf" download>Baixar Documento PDF</a>
```

## 6. Imagens

* Inserindo Imagens (```<img>```): A tag ```<img>``` é usada para inserir imagens em uma página da web. Ela não possui uma tag de fechamento e requer o atributo src, que especifica o caminho para a imagem.

```html
<img src="imagem.jpg" alt="Descrição da Imagem">
```

* Atributos alt e src: O atributo alt fornece uma descrição alternativa da imagem, importante para acessibilidade e SEO. O atributo src especifica o caminho da imagem.

```html
<img src="gato.jpg" alt="Foto de um gato fofo">
```

* Imagens Responsivas: Para garantir que as imagens se ajustem ao tamanho da tela, você pode adicionar a classe class="img-responsive" (no contexto do framework Bootstrap) ou usar CSS para tornar as imagens responsivas.

```html
<img src="imagem.jpg" alt="Descrição da Imagem" class="img-responsive">
```

## 7. Formulários

* Elemento ```<form>```: O elemento ```<form>``` é usado para criar formulários interativos em uma página da web. Ele envolve vários elementos de entrada e define como os dados serão enviados ao servidor.

```html
<form action="/processar-formulario" method="post">
    <!-- Elementos de entrada do formulário vão aqui -->
    <input type="text" name="nome" placeholder="Seu Nome">
    <input type="email" name="email" placeholder="Seu Email">
    <button type="submit">Enviar</button>
</form>
```

* Campos de Entrada (```<input>```): A tag ```<input>``` é usada para criar campos de entrada de texto, como campos de texto, caixas de seleção, botões de rádio e caixas de verificação.

```html
<input type="text" name="usuario" placeholder="Nome de Usuário">
<input type="password" name="senha" placeholder="Senha">
<input type="checkbox" name="lembre-me" id="lembre-me">
<label for="lembre-me">Lembre-me</label>
```

* Botões (```<button>```): A tag ```<button>``` é usada para criar botões em formulários. Você pode usá-los para enviar formulários ou realizar outras ações específicas.

```html
<button type="submit">Enviar</button>
<button type="reset">Limpar</button>
```

* Caixas de Seleção (```<select>```) e Opções (```<option>```): Você pode usar o elemento ```<select>``` para criar listas suspensas e o elemento ```<option>``` para definir as opções dentro dessas listas.

```html
<select name="cidade">
    <option value="ny">Nova York</option>
    <option value="la">Los Angeles</option>
    <option value="sf">São Francisco</option>
</select>
```

* Envio de Formulário: Ao clicar em um botão de envio dentro de um formulário, os dados inseridos nos campos de entrada são enviados ao servidor especificado no atributo action do elemento ```<form>```.

```html
<form action="/processar-formulario" method="post">
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome" placeholder="Seu Nome" required>
    
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" placeholder="Seu Email" required>
    
    <button type="submit">Enviar</button>
</form>
```




# CSS (Cascading Style Sheets)

## 1. Introdução ao CSS (Cascading Style Sheets)

* O que é CSS: CSS é a sigla para "Cascading Style Sheets" (Folhas de Estilo em Cascata). É uma linguagem de estilo usada para controlar a apresentação e o layout de elementos em uma página da web.

* Separação de Conteúdo e Estilo: Uma das principais vantagens do CSS é a separação de conteúdo e estilo. Isso significa que você pode manter o conteúdo HTML de uma página separado do seu estilo CSS. Isso torna o código mais limpo, organizado e mais fácil de manter.

* Seletor e Propriedades: No CSS, você seleciona os elementos HTML aos quais deseja aplicar estilos usando seletores e, em seguida, define as propriedades de estilo para esses elementos.

```css
/* Seletor */
p {
    /* Propriedades de Estilo */
    color: blue;
    font-size: 16px;
}
```

* Cascata: A palavra "cascata" em CSS significa que as regras de estilo podem ser sobrepostas e herdar características. Isso permite que você defina estilos de forma hierárquica, aplicando estilos gerais e, em seguida, refinando-os para elementos específicos.

* Herança: Os estilos aplicados a um elemento podem ser herdados por elementos filhos, a menos que sejam substituídos por estilos mais específicos.

* Folhas de Estilo Externas: Além de inserir estilos diretamente no HTML usando a tag ```<style>```, você pode criar folhas de estilo externas em arquivos separados com a extensão .css e vinculá-los a várias páginas HTML usando a tag ```<link>```.

```html
<link rel="stylesheet" type="text/css" href="estilos.css">
```

## 2. Seletores e Propriedades CSS

* Seletores: Os seletores CSS são padrões que definem quais elementos HTML receberão os estilos. Existem vários tipos de seletores, incluindo seletores de elemento, seletores de classe, seletores de ID e seletores de atributo.

- Exemplo de seletores de elemento:

```css
p {
    /* Estilos aplicados a todos os parágrafos */
}

h1, h2 {
    /* Estilos aplicados a todos os cabeçalhos h1 e h2 */
}
```

- Exemplo de seletores de classe:

```css
.destaque {
    /* Estilos aplicados a elementos com a classe "destaque" */
}
```

- Exemplo de seletores de ID:

```css
#cabecalho {
    /* Estilos aplicados a um elemento com o ID "cabecalho" */
}
```

* Propriedades CSS: As propriedades CSS são atributos que você pode definir para os elementos selecionados. Cada propriedade define um aspecto diferente do estilo, como cor, tamanho, margens, etc.

- Exemplo de propriedades CSS:

```css
p {
    color: blue; /* Define a cor do texto para azul */
    font-size: 16px; /* Define o tamanho da fonte como 16 pixels */
    margin-top: 10px; /* Define a margem superior como 10 pixels */
    background-color: #f0f0f0; /* Define a cor de fundo como cinza claro */
}
```

* Regras CSS: As regras CSS são formadas por seletores e propriedades, e são usadas para definir estilos. Elas são definidas dentro de um bloco de código entre chaves {}.

- Exemplo de regra CSS:

```css
p {
    color: blue;
    font-size: 16px;
}
```

* Comentários CSS: Você pode adicionar comentários em seu código CSS para documentar seu trabalho. Os comentários são precedidos por /* e terminados com */.

- Exemplo de comentário CSS:

```css
/* Este é um comentário de exemplo */
```

## 3. Estilos Inline, Incorporados e Externos em CSS

* Estilos Inline: Os estilos inline são aplicados diretamente a elementos HTML usando o atributo style. Esses estilos têm a maior especificidade e substituirão qualquer estilo definido externamente.

- Exemplo de estilo inline:

```html
<p style="color: red;">Este texto é vermelho.</p>
```

* Estilos Incorporados (Internal Styles): Os estilos incorporados são definidos dentro do próprio documento HTML, entre as tags ```<style>```. Esses estilos se aplicam a todas as ocorrências dos elementos selecionados no documento.

- Exemplo de estilo incorporado:

```html
<head>
    <style>
        p {
            color: blue;
            font-size: 16px;
        }
    </style>
</head>
<body>
    <p>Este é um parágrafo com estilo incorporado.</p>
</body>
```

* Estilos Externos (External Styles): Os estilos externos são definidos em arquivos CSS separados e vinculados ao documento HTML usando a tag ```<link>```. Esses estilos podem ser reutilizados em várias páginas HTML.

- Exemplo de estilo externo (em um arquivo "estilos.css"):

```css
p {
    color: green;
    font-size: 18px;
}
```

- Vinculação do arquivo CSS ao HTML:

```html
<link rel="stylesheet" type="text/css" href="estilos.css">
```

## 4. Formatação de Texto em CSS

* Fontes (font-family): A propriedade font-family permite definir a família de fontes para um elemento de texto. Você pode especificar várias fontes em ordem de preferência, para que o navegador escolha a primeira disponível.

- Exemplo:

```css
p {
    font-family: Arial, Helvetica, sans-serif;
}
```

* Tamanho de Fonte (font-size): A propriedade font-size define o tamanho da fonte do texto.

- Exemplo:

```css
h1 {
    font-size: 24px;
}
```

* Estilo de Fonte (font-style): A propriedade font-style permite definir o estilo da fonte, como itálico.

- Exemplo:

```css
em {
    font-style: italic;
}
```

* Peso da Fonte (font-weight): A propriedade font-weight define a espessura da fonte, como negrito.

- Exemplo:

```css
strong {
    font-weight: bold;
}
```

* Cor do Texto (color): A propriedade color define a cor do texto.

- Exemplo:

```css
p {
    color: #333; /* Cor cinza escuro */
}
```

* Espaçamento entre Linhas (line-height): A propriedade line-height controla o espaçamento entre as linhas de texto.

- Exemplo:

```css
p {
    line-height: 1.5; /* Espaçamento 1,5 vezes a altura da fonte */
}
```

* Alinhamento de Texto (text-align): A propriedade text-align define como o texto é alinhado dentro de um elemento, como à esquerda, à direita, centralizado ou justificado.

- Exemplo:

```css
h2 {
    text-align: center;
}
```

* Decoração de Texto (text-decoration): A propriedade text-decoration controla a decoração do texto, como sublinhado.

- Exemplo:

```css
a {
    text-decoration: none; /* Remove sublinhado de links */
}
```

## 5. Modelos de Caixas (Box Model) em CSS

* Modelo de Caixa (Box Model): O modelo de caixa é um conceito fundamental em CSS que descreve como os elementos HTML são representados visualmente. Cada elemento HTML é considerado uma caixa retangular que consiste em quatro áreas principais: conteúdo, preenchimento, borda e margem.

* Conteúdo (content): É a área interna da caixa que contém o conteúdo real, como texto ou imagens.

* Preenchimento (padding): É uma área opcional ao redor do conteúdo, separando-o da borda. O preenchimento é controlado pelas propriedades padding-top, padding-right, padding-bottom e padding-left.

* Borda (border): A borda é uma linha que circunda o conteúdo e o preenchimento. Você pode personalizar a aparência da borda usando propriedades como border-width, border-style e border-color.

* Margem (margin): A margem é uma área opcional fora da borda que separa um elemento de outros elementos vizinhos. As margens podem ser definidas com as propriedades margin-top, margin-right, margin-bottom e margin-left.

* Box Sizing (box-sizing): A propriedade box-sizing permite controlar como as dimensões totais da caixa são calculadas. O valor padrão é content-box, que leva em consideração apenas o conteúdo e o preenchimento ao calcular a largura e altura total. Você também pode usar border-box, que inclui o conteúdo, o preenchimento e a borda nas dimensões totais da caixa.

- Exemplo:

```css
div {
    width: 200px;
    height: 100px;
    padding: 20px;
    border: 2px solid #000;
    margin: 10px;
    box-sizing: border-box; /* Inclui preenchimento e borda nas dimensões */
}
```

* Espaçamento Negativo (negative margin): Margens negativas permitem que os elementos se sobreponham a seus vizinhos. Isso pode ser útil para criar layouts complexos, mas deve ser usado com cuidado.

## 6. Posicionamento e Layout em CSS

* Posicionamento (position): A propriedade position permite controlar como um elemento é posicionado em relação ao seu contexto. Os valores mais comuns são:
 - static (padrão): O elemento é posicionado normalmente no fluxo do documento.
 - relative: O elemento é posicionado em relação à sua posição original.
 - absolute: O elemento é posicionado em relação ao seu ancestral mais próximo com position diferente de static.
 - fixed: O elemento é posicionado em relação à janela do navegador, permanecendo fixo enquanto você rola a página.

* Deslocamento (top, right, bottom, left): Essas propriedades são usadas com elementos posicionados (relative, absolute, ou fixed) para ajustar sua posição a partir de sua localização original.
- Exemplo:
```css
.caixa {
    position: relative;
    top: 20px;
    left: 30px;
}
```

* Layout de Exibição (display): A propriedade display controla o comportamento de exibição de um elemento. Alguns valores comuns incluem:

- block: O elemento ocupa toda a largura disponível e inicia em uma nova linha.
- inline: O elemento ocupa apenas o espaço necessário e não inicia uma nova linha.
- inline-block: Combina características de elementos block e inline.
- none: O elemento não é exibido.

* Flutuação (float): A propriedade float é usada para fazer com que um elemento flutue à esquerda ou à direita de seu contêiner pai. É comumente usado para criar layouts de coluna.

- Exemplo:

```css
.coluna {
    float: left;
    width: 50%;
}
```

* Clear (clear): A propriedade clear é usada para garantir que um elemento não flutue ao lado de elementos anteriores que estão flutuando.

- Exemplo:

```css
.limpar {
    clear: both;
}
```

* Flexbox e Grid: CSS também oferece recursos avançados de layout, como Flexbox e Grid Layout, que permitem criar layouts complexos de forma eficiente.

- Exemplo de uso de Flexbox:

```css
.container {
    display: flex;
    justify-content: space-between;
}
```

- Exemplo de uso de Grid Layout:

```css
.grid-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
}
```

## 7. Cores e Fundos em CSS

* Cor do Texto (color): A propriedade color define a cor do texto dentro de um elemento.

- Exemplo:

```css
p {
    color: #FF5733; /* Cor em formato hexadecimal */
}
```

* Cor de Fundo (background-color): A propriedade background-color define a cor de fundo de um elemento.

- Exemplo:

```css
div {
    background-color: #EFEFEF; /* Cor de fundo em formato hexadecimal */
}
```

* Imagem de Fundo (background-image): Você pode definir uma imagem como fundo de um elemento usando a propriedade background-image.

- Exemplo:

```css
body {
    background-image: url('fundo.jpg');
    background-size: cover; /* Redimensiona a imagem para cobrir todo o fundo */
}
```

* Repetição de Fundo (background-repeat): A propriedade background-repeat controla como uma imagem de fundo é repetida.

- Exemplo:

```css
div {
    background-image: url('padrao.png');
    background-repeat: repeat-x; /* Repete horizontalmente */
}
```

* Posicionamento de Fundo (background-position): A propriedade background-position permite definir a posição inicial de uma imagem de fundo.

- Exemplo:

```css
header {
    background-image: url('cabecalho.jpg');
    background-position: center top; /* Posiciona no centro superior */
}
```

* Gradientes de Fundo (background-gradient): Além de cores sólidas e imagens, você pode criar fundos gradientes usando a propriedade background-image.

- Exemplo:

```css
button {
    background-image: linear-gradient(to right, #FF5733, #FFC300); /* Gradiente linear */
}
```

* Sombra Textual (text-shadow) e Sombra de Caixa (box-shadow): Você pode adicionar sombras tanto a texto quanto a caixas usando as propriedades text-shadow e box-shadow, respectivamente.

- Exemplo:

```css
h1 {
    text-shadow: 2px 2px 4px #333; /* Sombra de texto */
}

.caixa {
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Sombra de caixa */
}
```

## 8. Pseudo-classes e Pseudo-elementos em CSS

### Pseudo-classes

As pseudo-classes são usadas para selecionar elementos com base em estados ou interações do usuário.

* :hover: Seleciona um elemento quando o cursor do mouse está sobre ele.

- Exemplo:

```css
a:hover {
    color: red; /* Altera a cor do texto quando o mouse passa sobre o link */
}
```

* :active: Seleciona um elemento quando ele está ativo, geralmente quando é clicado.

* :focus: Seleciona um elemento quando ele está com foco, como quando um campo de entrada de formulário é selecionado.

- Exemplo:

```css
input:focus {
    border-color: blue; /* Define a cor da borda quando o campo de entrada está em foco */
}
```

* :nth-child(): Seleciona elementos com base em sua posição em relação aos irmãos. Isso permite estilizar elementos em listas ou tabelas de forma específica.

- Exemplo:

```css
li:nth-child(even) {
    background-color: #f2f2f2; /* Define a cor de fundo para linhas pares em uma lista */
}
```

### Pseudo-elementos

Os pseudo-elementos permitem estilizar partes específicas de um elemento, como o primeiro caractere de um parágrafo (::first-letter) ou o último elemento de uma lista (::last-child).

* ::before e ::after: Permitem adicionar conteúdo gerado antes ou após o conteúdo de um elemento.

- Exemplo:

```css
p::before {
    content: "» "; /* Adiciona um caractere antes de cada parágrafo */
}
```

* ::first-line e ::first-letter: Permitem estilizar a primeira linha ou o primeiro caractere de um elemento de texto.

- Exemplo:

```css
p::first-line {
    font-weight: bold; /* Deixa a primeira linha do parágrafo em negrito */
}

p::first-letter {
    font-size: 24px; /* Aumenta o tamanho da primeira letra do parágrafo */
}
```

* ::selection: Permite estilizar o texto selecionado pelo usuário.

- Exemplo:

```css
::selection {
    background-color: yellow; /* Define a cor de fundo para texto selecionado */
    color: black; /* Define a cor do texto selecionado */
}
```


## 9. Media Queries em CSS

As media queries são uma parte essencial do design responsivo em CSS. Elas permitem que você adapte o layout e o estilo de uma página da web com base nas características do dispositivo ou na largura da tela.

* Sintaxe Básica: Uma media query começa com a palavra-chave @media, seguida de uma condição que descreve as características do dispositivo que você deseja direcionar. As media queries são definidas entre chaves {} e contêm as regras CSS que serão aplicadas quando a condição for atendida.

- Exemplo de uma media query que direciona dispositivos com largura de tela menor que 600 pixels:

```css
@media (max-width: 600px) {
    /* Regras CSS a serem aplicadas a dispositivos com largura menor que 600px */
    body {
        font-size: 14px;
    }
    .menu {
        display: none;
    }
}
```

* Condições Comuns: Existem várias condições que você pode usar em media queries para direcionar diferentes características do dispositivo, incluindo:

- max-width e min-width: Define faixas de largura de tela.
- max-height e min-height: Define faixas de altura de tela.
- orientation: Direciona a orientação da tela, como retrato ou paisagem.
- device-pixel-ratio: Direciona dispositivos de alta resolução (Retina, por exemplo).
- hover: Direciona dispositivos que suportam interações com o mouse.

* Múltiplas Condições: Você pode combinar várias condições usando operadores and (and) e or (or) para criar media queries mais complexas.

- Exemplo de uma media query com várias condições:

```css
@media (max-width: 600px) and (orientation: portrait) {
    /* Regras CSS para dispositivos com largura menor que 600px em modo retrato */
    /* ... */
}
```

* Design Responsivo: O uso eficaz de media queries é fundamental para criar um design responsivo que se adapte a uma variedade de dispositivos e tamanhos de tela. Você pode reorganizar o layout, ajustar tamanhos de fonte, ocultar ou exibir elementos e muito mais, dependendo das necessidades do seu design.

* Exemplos Práticos: Algumas aplicações comuns de media queries incluem ajustar a navegação para telas pequenas, reorganizar colunas em layouts de grade e alterar o tamanho da fonte para melhor legibilidade em dispositivos móveis.

## 10. Animações e Transições em CSS (Opcional)

As animações e transições em CSS permitem adicionar movimento e interatividade a elementos em uma página da web.

* Transições (transition): As transições permitem suavizar a mudança de um estado para outro. Você pode definir propriedades CSS que mudam gradualmente quando um evento, como um hover ou foco, ocorre. As transições são configuradas com a propriedade transition.

- Exemplo:

```css
.botao {
    background-color: #3498db;
    transition: background-color 0.3s ease; /* Altera a cor de fundo suavemente em 0,3 segundos */
}

.botao:hover {
    background-color: #2980b9; /* Nova cor de fundo no hover */
}
```

* Animações (@keyframes): As animações permitem criar sequências de movimentos ou mudanças de estilo em elementos. Você define as etapas da animação usando a regra @keyframes e, em seguida, aplica essa animação a um elemento usando a propriedade animation.

- Exemplo:

```css
@keyframes balanco {
    0% {
        transform: rotate(0deg); /* Começa sem rotação */
    }
    50% {
        transform: rotate(10deg); /* Rotação intermediária */
    }
    100% {
        transform: rotate(-10deg); /* Rotação final */
    }
}

.caixa {
    animation: balanco 2s infinite; /* Aplica a animação de balanço de forma contínua */
}
```

* Propriedades de Animação (animation): A propriedade animation é usada para aplicar animações a elementos e controlar sua duração, iteração e outros aspectos.

* Easing Functions: Você pode usar funções de "easing" para controlar como uma animação acelera ou desacelera ao longo do tempo. Alguns exemplos incluem ease, ease-in, ease-out e ease-in-out.

* Frameworks de Animação: Para animações mais complexas, você pode considerar o uso de frameworks de animação em CSS, como o Animate.css ou bibliotecas JavaScript como o GreenSock (GSAP).
