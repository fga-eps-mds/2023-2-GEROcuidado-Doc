# Módulo 1: Introdução ao JavaScript
## O que é JavaScript?
### História e evolução

JavaScript é uma linguagem de programação de alto nível criada por Brendan Eich em 1995. Foi originalmente desenvolvida para ser executada no navegador Netscape Navigator e tinha o nome inicial de "LiveScript". Mais tarde, foi renomeada para JavaScript para aproveitar o sucesso da linguagem Java. JavaScript evoluiu significativamente ao longo dos anos, tornando-se uma das linguagens de programação mais populares e versáteis do mundo.

### O papel do JavaScript no desenvolvimento web

JavaScript desempenha um papel fundamental no desenvolvimento web moderno. Ele permite que você adicione interatividade e dinamismo às páginas da web, tornando-as mais envolventes para os usuários. Por exemplo, você pode usar JavaScript para:

* Validar formulários em tempo real.
* Criar carrosséis de imagens interativos.
* Atualizar conteúdo de páginas sem recarregar a página inteira (AJAX).
* Manipular o Document Object Model (DOM) para alterar elementos HTML dinamicamente.
* Criar jogos e aplicativos web complexos.

## Configuração do ambiente
### Instalação do Node.js

Para trabalhar com JavaScript no servidor (back-end), é comum usar o Node.js. Para instalá-lo, siga os passos apropriados para o seu sistema operacional no site oficial do Node.js: [Node.js Download](https://nodejs.org/).

```bash
node -v
npm -v
```

# Módulo 2: Conceitos Básicos
## Variáveis e Tipos de Dados
### Variáveis e constantes

Em JavaScript, você pode declarar variáveis usando as palavras-chave var, let e const. A diferença entre var, let e const está no escopo e na mutabilidade das variáveis.

```js
var nome = "João"; // Declaração de variável usando var
let idade = 30;    // Declaração de variável usando let
const PI = 3.1415;  // Declaração de constante usando const
```

### Tipos de dados primitivos

```js
 let numero = 42; // Números
 let nome = "Alice";  // String
 let estaAtivo = true;  // Booleanos
 let valor; // Undefined (quando uma variável é declarada, mas nenhum valor é atribuído a ela)
 let nulo = null;  // Nulo  (representa a ausência intencional de qualquer valor ou objeto)
```

## Operadores
### Operadores aritméticos

```js
let a = 10;
let b = 5;

// *** ATENÇÃO PARA O TIPO DE DADO
let soma = a + b;     // Soma: 15
let subtracao = a - b; // Subtração: 5
let multiplicacao = a * b; // Multiplicação: 50
let divisao = a / b; // Divisão: 2
```

### Operadores de comparação
```js
let x = 10;
let y = 5;

let igual = x === y;   // Igual: false
let diferente = x !== y; // Diferente: true
let maior = x > y;      // Maior que: true
let menor = x < y;      // Menor que: false
```

### Operadores lógicos
```js
let estaChovendo = true;
let estaFrio = false;

let ficarEmCasa = estaChovendo && estaFrio; // Ambos verdadeiros: true
let sairParaPassear = estaChovendo || estaFrio; // Pelo menos um verdadeiro: true
let naoSair = !sairParaPassear; // Invertendo o valor: false
```
## Controle de Fluxo

### Estruturas condicionais (if, else, switch, operador ternário)

* Estruturas condicionais permitem que você execute código com base em condições. O if é usado para executar um bloco de código se a condição for verdadeira, enquanto o else é usado para executar um bloco de código alternativo se a condição for falsa.

 ```js
let idade = 18;

if (idade >= 18) {
  console.log("Você é maior de idade.");
} else {
  console.log("Você é menor de idade.");
}
 ```

* O switch é usado quando você precisa lidar com múltiplas condições.

```js
let diaDaSemana = 3;
let nomeDoDia;

switch (diaDaSemana) {
  case 1:
    nomeDoDia = "Segunda-feira";
    break;
  case 2:
    nomeDoDia = "Terça-feira";
    break;
  case 3:
    nomeDoDia = "Quarta-feira";
    break;
  case 4:
    nomeDoDia = "Quinta-feira";
    break;
  case 5:
    nomeDoDia = "Sexta-feira";
    break;
  case 6:
    nomeDoDia = "Sábado";
    break;
  case 7:
    nomeDoDia = "Domingo";
    break;
  default:
    nomeDoDia = "Dia inválido";
}

console.log("Hoje é " + nomeDoDia);
```

* O operador ternário ? é uma forma concisa de escrever uma instrução if...else em uma única linha.

```js
let idade = 20;
let status = (idade >= 18) ? "Maior de idade" : "Menor de idade";
console.log(status);
```

### Estruturas de repetição (for, while, do-while)

Estruturas de repetição permitem que você execute código repetidamente.

* O for é útil quando você sabe quantas vezes deseja repetir.

```js
for (let i = 0; i < 5; i++) {
  console.log("Número: " + i);
}
```

* O while executa o loop enquanto a condição for verdadeira.

```js
let contador = 0;

while (contador < 5) {
  console.log("Contador: " + contador);
  contador++;
}
```

* O do While executa o loop primeiro e depois verifica a condição.
```js
let contador = 0;

do {
  console.log('Contador: ' + contador)
  contador++;
} while(contador <= 10)
```

# Módulo 3: Funções e Escopo
## Funções
### Definindo Funções

Funções são blocos de código reutilizáveis que podem ser chamados em vários lugares do programa. Em JavaScript, você pode definir funções de várias maneiras, incluindo declarações de função e expressões de função.

```js
// Função tradicional
// ** Parâmetros são variáveis listadas entre os parênteses na definição de uma função. Eles servem como variáveis locais na função.
function saudacao(nome) {
  console.log(`Olá, ${nome}!`);
}

// Expressão de função (function expression)
const saudacao = function(nome) {
  console.log(`Olá, ${nome}!`);
};

saudacao("Maria"); // Chamando a função e passando o argumento "Maria"
```

###  Retornando Valores

Funções podem retornar valores usando a palavra-chave return. Isso permite que você obtenha um resultado calculado ou processado pela função.

```js
function soma(a, b) {
  return a + b;
}

let resultado = soma(5, 3); // Chamando a função e armazenando o resultado
console.log(resultado); // Exibe 8
```

### Arrow Functions

* Arrow functions são uma sintaxe mais curta e concisa para definir funções em JavaScript.
* Elas têm um escopo léxico, o que significa que herdam o valor this do contexto em que foram criadas.

```js
const soma = (a, b) => a + b;
```

## Escopo
### Escopo Global e Local

Em JavaScript, existem dois principais níveis de escopo: escopo global e escopo local. Variáveis declaradas fora de uma função têm escopo global, enquanto variáveis declaradas dentro de uma função têm escopo local.

```js
let globalVar = "Isso é uma variável global";

function exemploEscopo() {
  let localVar = "Isso é uma variável local";
  console.log(globalVar); // Variável global acessível dentro da função
  console.log(localVar);  // Variável local acessível dentro da função
}

exemploEscopo();
console.log(globalVar); // Variável global acessível fora da função
// console.log(localVar);  // Isso resultará em um erro, a variável local não é acessível fora da função
```

### Escopo de Bloco (let e const)

Variáveis declaradas com let e const também têm escopo de bloco. Isso significa que elas estão limitadas ao bloco de código em que são declaradas.

```js
if (true) {
  let nome = "João";
  console.log(nome); // Variável "nome" é acessível apenas neste bloco
}
// console.log(nome);  // Isso resultará em um erro, a variável "nome" não é acessível aqui
```

### Closure

Um closure é uma função que "lembra" do ambiente em que foi criada, incluindo as variáveis fora de seu próprio escopo.

```js
function contador() {
  let count = 0;

  function increment() {
    count++;
    console.log(count);
  }

  return increment;
}

let contador1 = contador();
contador1(); // Exibe 1
contador1(); // Exibe 2
```

Neste exemplo, contador retorna a função increment, que ainda tem acesso à variável count mesmo após contador ter sido executada.


# Módulo 4: Arrays e Objetos
## Arrays
### Introdução a Arrays

Arrays são estruturas de dados em JavaScript que permitem armazenar e organizar coleções de valores. Eles são especialmente úteis para lidar com listas de itens relacionados.

```js
let frutas = ["Maçã", "Banana", "Morango"];
```

### Acessando e Modificando Elementos de um Array

Você pode acessar e modificar elementos em um array usando índices.

```js
let primeiraFruta = frutas[0]; // Acessa o primeiro elemento (índice 0)
console.log(primeiraFruta); // Exibe "Maçã"

frutas[1] = "Pera"; // Modifica o segundo elemento (índice 1)
console.log(frutas); // Exibe ["Maçã", "Pera", "Morango"]
```

### Métodos de Arrays

Arrays possuem métodos que permitem realizar operações comuns, como adicionar, remover, filtrar e transformar elementos.

```js
frutas.push("Uva", "Abacaxi"); // Adiciona elementos ao final do array
console.log(frutas); // Exibe ["Maçã", "Pera", "Morango", "Uva", "Abacaxi"]

frutas.unshift("Manga"); // Adiciona elementos ao início do array
console.log(frutas); // Exibe ["Manga", "Maçã", "Pera", "Morango", "Uva", "Abacaxi"]

frutas.pop(); // Remove o elemento do final do array
console.log(frutas); // Exibe ["Manga", "Maçã", "Pera", "Morango", "Uva"]

frutas.shift(); // Remove o elemento do início do array
console.log(frutas); // Exibe ["Maçã", "Pera", "Morango", "Uva"]
```

### Iteração com Loops em Arrays

Loops como for e for...of são usados para iterar pelos elementos de um array.

```js
for (let fruta of frutas) {
  console.log(fruta); // "Maçã" -> "Pera" -> "Morango" -> "Uva"
}
```

## Objetos
### Introdução a Objetos

Objetos são estruturas de dados que permitem armazenar informações organizadas em pares de chave e valor. Eles são ideais para representar entidades complexas com propriedades específicas.

```js
let pessoa = {
  nome: "Maria",
  idade: 30,
  cidade: "São Paulo"
};
```

### Acessando e Modificando Propriedades de um Objeto

Você pode acessar e modificar as propriedades de um objeto usando a notação de ponto ou a notação de colchetes.

```js
let nomeDaPessoa = pessoa.nome; // Acessa a propriedade "nome"
console.log(nomeDaPessoa); // Exibe "Maria"

pessoa.idade = 31; // Modifica a propriedade "idade"
console.log(pessoa); // Exibe { nome: "Maria", idade: 31, cidade: "São Paulo" }
```

### Métodos e Funções em Objetos

Objetos podem conter métodos, que são funções definidas dentro do objeto.

```js
let carro = {
  marca: "Toyota",
  modelo: "Camry",
  ligar: function() {
    console.log("O carro está ligado.");
  }
};

carro.ligar(); // Chama o método "ligar" do objeto
```

###  Iteração com Loops em Objetos

Você pode iterar pelas propriedades de um objeto usando loops como for...in.

```js
for (let chave in pessoa) {
  console.log(chave + ": " + pessoa[chave]); // "nome: Maria" -> "idade: 30" -> "Cidade: São Paulo"
}
```

## Desestruturação

* A desestruturação permite que você extraia valores de objetos e arrays de forma mais conveniente.
* É útil para atribuir variáveis a partir de propriedades de objetos ou elementos de arrays.

```js
const pessoa = { nome: "Maria", idade: 30 };
const { nome, idade } = pessoa;

const array = ["Maçã", "Pera"];
const [fruta1, fruta2] = array;
```

## Spread e Rest Operator

* O operador spread (...) permite espalhar elementos de um array ou propriedades de um objeto em outro.
* O operador rest (...) é usado para coletar argumentos em uma função em um único array.

```js
// spread
const frutas = ["Maçã", "Banana"];
const maisFrutas = [...frutas, "Morango"];
console.log(maisFrutas) // ["Maçã", "Banana", "Morango"]

// rest
const pessoa = { nome: "Maria", idade: 30 }
const professora = { ...pessoa, materia: "Biologia" }
console.log(professora) // { nome: "Maria", idade: 30, materia: "Biologia" }
```

# Módulo 5: Manipulação do DOM e Eventos
## Introdução ao DOM (Document Object Model)
### O que é o DOM?

O DOM (Document Object Model) é uma representação hierárquica em árvore de um documento HTML ou XML. Ele permite que os programadores acessem e manipulem os elementos e conteúdos de uma página web por meio de scripts.

```js
let elemento = document.getElementById("meu-elemento");
```

## Manipulação do DOM
### Selecionando Elementos

Você pode selecionar elementos do DOM usando métodos como getElementById, querySelector, getElementsByClassName e getElementsByTagName.

```js
let meuElemento = document.getElementById("meu-elemento");
let botoes = document.getElementsByClassName("botao");
let paragrafos = document.querySelectorAll("p");
```

### Manipulando Conteúdo

Você pode alterar o conteúdo de elementos HTML, como textos e atributos, usando propriedades do DOM.

```js
let meuElemento = document.getElementById("meu-elemento");
meuElemento.textContent = "Novo texto";
meuElemento.setAttribute("href", "https://www.example.com");
```

### Criando e Inserindo Elementos

Você pode criar novos elementos HTML e inseri-los no DOM.

```js
let novaDiv = document.createElement("div");
document.body.appendChild(novaDiv); // Insere a nova div como filho do body
```

## Eventos
### Introdução a Eventos

Eventos são ações do usuário ou do navegador que podem ser detectadas e respondidas por meio de scripts. Exemplos de eventos incluem cliques de mouse, pressionamento de teclas e redimensionamento da janela.

```js
meuElemento.addEventListener("click", function() {
  alert("Cliquei no elemento!");
});
```

### Manipulando Eventos

Você pode criar funções de manipulação de eventos para executar ações quando um evento específico ocorre.

```js
function clicarElemento() {
  alert("Cliquei no elemento!");
}

meuElemento.addEventListener("click", clicarElemento);
```

## Event Bubbling e Delegation
### Event Bubbling

O event bubbling é um comportamento em que eventos ocorrem primeiro nos elementos mais internos e depois se propagam para os elementos pai. Isso afeta a ordem em que os eventos são tratados.

```html
<div id="pai">
  <button id="botao">Clique aqui</button>
</div>
```
```js
document.getElementById("pai").addEventListener("click", function() {
    alert("Cliquei no pai.");
});

document.getElementById("botao").addEventListener("click", function() {
    alert("Cliquei no botão.");
});
```

### Event Delegation

O event delegation é uma técnica em que você adiciona um único manipulador de evento a um elemento pai em vez de adicionar manipuladores a vários elementos filhos. Isso é útil para otimizar o desempenho e tratar eventos em elementos dinâmicos.

```html
<ul id="minha-lista">
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```
```js
document.getElementById("minha-lista").addEventListener("click", function(event) {
  if (event.target.tagName === "LI") {
    alert("Cliquei no item: " + event.target.textContent);
  }
});
```

# Módulo 6: Aplicações e Tópicos Avançados em JavaScript
## Manipulação de Formulários
### Interação com Formulários

JavaScript pode ser usado para interagir com formulários HTML, obtendo dados de entrada do usuário e validando esses dados.

```js
let inputNome = document.getElementById("nome");
let valorNome = inputNome.value;

// Validando
if (!valorEmail.includes("@")) {
  alert("O endereço de email é inválido.");
}
```

##  Programação Assíncrona
### Callbacks

Callbacks são funções que são passadas como argumentos para outras funções e são executadas após a conclusão de uma operação assíncrona.

```js
function fazerAlgoAssincrono(callback) {
  setTimeout(() => {
    console.log("Operação assíncrona concluída.");
    callback();
  }, 2000);
}

fazerAlgoAssincrono(() => {
  console.log("Callback executado após a operação assíncrona.");
});
```

### Promises

Promises são uma forma mais estruturada de lidar com operações assíncronas em JavaScript, tornando o código mais legível e gerenciável.

```js
function fazerAlgoAssincrono() {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      console.log("Operação assíncrona concluída.");
      resolve();
    }, 2000);
  });
}

fazerAlgoAssincrono()
  .then(() => {
    console.log("Promise resolvida com sucesso.");
  })
  .catch((error) => {
    console.error("Erro na Promise: " + error);
  });
```

### Async/Await

* As palavras-chave async e await são usadas para tornar o código mais legível ao trabalhar com operações assíncronas em JavaScript.
* Elas são frequentemente usadas em conjunto com Promises para simplificar o código assíncrono.
* Funções Assíncronas (Async Functions)
* A palavra-chave async é usada para declarar uma função como assíncrona.
* Funções assíncronas sempre retornam uma Promise.

```js
async function minhaFuncao() {
  const resultado = await algumaOperacaoAssincrona();
  console.log(resultado);
}
```

* Tratamento de Erros:
- Você pode usar try...catch para capturar erros ao trabalhar com await.
- Isso torna a manipulação de erros em código assíncrono mais semelhante à manipulação de erros em código síncrono.
```js
async function minhaFuncao() {
  try {
    const resultado = await algumaOperacaoAssincrona();
    console.log(resultado);
  } catch (erro) {
    console.error("Ocorreu um erro: " + erro);
  }
}
```


## Classes

* As classes são uma forma de definir objetos e construtores em JavaScript de maneira mais orientada a objetos.
* Elas simplificam a criação de objetos com propriedades e métodos.

```js
class Pessoa {
  constructor(nome, idade) {
    this.nome = nome;
    this.idade = idade;
  }

  saudacao() {
    console.log(`Olá, meu nome é ${this.nome} e tenho ${this.idade} anos.`);
  }
}

const maria = new Pessoa("Maria", 30);
maria.saudacao();
```

## Módulos

* Os módulos permitem organizar e reutilizar código em diferentes arquivos.
* O ES6 introduziu o sistema de módulos em JavaScript, com as palavras-chave import e export.

```js
// arquivo modulo.js
export const soma = (a, b) => a + b;

// arquivo principal.js
import { soma } from "./modulo.js";
console.log(soma(5, 3)); // Exibe 8
```

# Módulo 7: Manipulação de Dados em JSON

## Sintaxe JSON
* JSON é composto por pares de chave/valor, semelhante à notação de objetos em JavaScript.
* Os valores podem ser strings, números, booleanos, objetos, arrays ou null.
* Chaves devem estar entre aspas duplas (") e seguidas de :.

```js
{
  "nome": "Maria",
  "idade": 30,
  "casado": false,
  "hobbies": ["Leitura", "Esportes"]
}
```

## Conversão entre JSON e JavaScript
É possível converter entre objetos JavaScript e strings JSON usando as funções JSON.stringify() e JSON.parse().

```js
// JSON/Objeto -> string
const pessoa = {
  nome: "Maria",
  idade: 30
};
const jsonPessoa = JSON.stringify(pessoa);
console.log(jsonPessoa);

// string -> JSON/Objeto
const jsonString = '{"nome": "Maria", "idade": 30}';
const objetoPessoa = JSON.parse(jsonString);
console.log(objetoPessoa);
```

## Uso de JSON em Requisições e Respostas HTTP
JSON é frequentemente usado em APIs para transmitir dados entre clientes e servidores.
As solicitações HTTP podem enviar dados JSON no corpo da requisição, e as respostas geralmente são recebidas como JSON.

```js
// Enviar
fetch("https://api.example.com/salvar-dados", {
  method: "POST",
  headers: {
    "Content-Type": "application/json"
  },
  body: JSON.stringify({ nome: "Maria", idade: 30 })
});

// Receber
fetch("https://api.example.com/obter-dados")
  .then(response => response.json())
  .then(data => {
    console.log(data);
  });
```

## Boas Práticas
* Ao criar e manipular JSON, certifique-se de que a sintaxe esteja correta e que os valores estejam no formato adequado.
* Use try...catch ao analisar JSON para lidar com erros de sintaxe.
```js
try {
  const objeto = JSON.parse(jsonString);
} catch (erro) {
  console.error("Erro ao analisar JSON: " + erro);
}
```

# Link da vídeo aula

https://drive.google.com/file/d/1IO_FbpdqCZp-XgA18jCmeRS8gnc2rYeL/view?usp=sharing