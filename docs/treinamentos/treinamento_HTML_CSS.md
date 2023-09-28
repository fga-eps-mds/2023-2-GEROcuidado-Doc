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




