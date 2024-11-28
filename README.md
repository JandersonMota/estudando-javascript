# Estudando JavaScript
Aqui, vamos explorar alguns tópicos e destacar principalmente as diferenças em relação a outras linguagens. Meu conhecimento é focado em C e Java, então, se eu não mencionar algo sobre o assunto, pode assumir que é igual ao que acontece nessas linguagens.

## Caracteriscas
- É uma linguagem interpretada.
- É uma linguagem não tipada, ou seja, não se especifica os tipos de dados representados.
- Os tipos de dados são dinâmicos, o que significa que a mesma variável pode ser usada com tipos diferentes.
- As variáveis são case-sensitive, ou seja, diferenciam maiúsculas de minúsculas.
- Todas as instruções de código devem terminar com um ponto-e-vírgula `;`.

## Marcador <script>
O marcador `<script>` possui alguns atributos importantes, como:
- **type**: informa ao navegador o tipo de texto contido no elemento, ou seja, o tipo de script.
- **src**: especifica o local do arquivo .js, caso seja usado um arquivo externo contendo o código JavaScript.
Obs.: não precisa informar `type`, já que os navegadores reconhecem apenas com `<script>`.

Código JavaScript interno na página HTML.
```javascript
<script type="text/javascript">
  // AQUI VAI O CÓDIGO
</script>
```

Código JavaScript sendo usado em um arquivo externo.
```javascript
<script type="text/javascript" src="nomeDoArquivo.js"></script>
// Ou
<script src="nomeDoArquivo.js"></script>
```

## Tipos de variáveis
JavaScript é uma "linguagem tipada dinamicamente", o que significa que, ao contrário de algumas outras linguagens, você não precisa especificar qual tipo de dados uma variável conterá (números, strings, arrays, etc.).

Os tipos de dados são:
- Número inteiro
- Número de ponto flutuante
- String: devem ser representados entre aspas simples ou duplas.
- Booleano
- Array
- Objeto

Tipos de variáveis:
- `var`

```javascript
var nome;
var a=20, b=40.65, codigo="S43X";
var estado=true;
```

`typeof`: informa o tipo da variável.

```javascript
var a=10, b=4.50, c="Água", d=true, e;

document.write("a é " + typeof a + "<br/>"); // a é number
document.write("b é " + typeof b + "<br/>"); // b é number
document.write("c é " + typeof c + "<br/>"); // c é string
document.write("d é " + typeof d + "<br/>"); // d é boolean
document.write("e é " + typeof e + "<br/>"); // e é undefined
```


```javascript
let myNameArray = ["Chris", "Bob", "Jim"];
let myNumberArray = [10, 15, 40];
```

## Alguns comandos
- Exibir a mensagem dentro do HTML: `document.write("ESCREVA AQUI");`
- Exibir uma caixa de mensagem: `alert("ESCREVA AQUI");`

## Funções
Definimos uma função usando a palavra-chave `function`, seguida por um nome `checkGuess`, com parênteses colocados depois dela.

```javascript
function checkGuess() {
  // AQUI VAI O CÓDIGO
}
```

## Operadores

| Operador  | Nome                                      |
|-----------|-------------------------------------------|
| ===       | Igualdade estrita (é exatamente a mesma?) |
| !==       | Não igualdade (não é a mesma coisa?)      |

## Cadeias de caracteres de texto

```javascript
function checkGuess() {
  alert("I am a placeholder");
}
```
| Exemplos                                | Descrição                                                                                |
|-----------------------------------------|------------------------------------------------------------------------------------------|
| alert("I am a placeholder");            | Pode declarar strings usando aspas duplas.                                               |
| alert('I am a placeholder');            | Pode declarar strings usando aspas simples.                                              |
| alert(\`I am a placeholder\`);          | Pode declarar strings usando acentos graves. As cadeias de caracteres declaradas assim são chamadas de *literais de modelo* e têm algumas                                                   propriedades especiais. |

## Condicionais

```javascript
function checkGuess() {
  if() {
    // AQUI VAI O CÓDIGO
  } else if () {
    // AQUI VAI O CÓDIGO
  } else {
    // AQUI VAI O CÓDIGO
  }
}
```

## Eventos

Eventos são coisas que acontecem no navegador - um botão sendo clicado, uma página carregando, um vídeo sendo reproduzido, etc. - em resposta às quais podemos executar blocos de código. Os ouvintes de eventos observam eventos específicos e chamam manipuladores de eventos, que são blocos de código executados em resposta a um acionamento de evento.

```javascript
guessSubmit.addEventListener("click", checkGuess);
```

Acima, temos um ouvinte de eventos associado ao botão. O método `addEventListener` recebe dois argumentos: o tipo de evento que queremos ouvir (neste caso, a cadeia de caracteres `click`) e o código que desejamos executar quando o evento ocorre (neste caso, a função `checkGuess`). Observe que, ao passar a função `checkGuess` como argumento, não incluímos os parênteses, pois estamos referenciando a função e não executando-a imediatamente.

## Loops

```javascript
const fruits = ["apples", "bananas", "cherries"];
for (const fruit of fruits) {
  console.log(fruit);
}
```

## Melhoria

```javascript
guessField.focus();
```

Esta linha usa o método `focus()` para colocar automaticamente o cursor de texto no campo de entrada `<input>`. Isso significa que, ao executar essa linha de código, o usuário pode começar a digitar imediatamente, sem precisar clicar no campo do formulário. Embora seja uma pequena adição, ela melhora a usabilidade.

### Matemática

Para arredondar seu número para um número fixo de casas decimais, use o método `toFixed()`.
```javascript
const lotsOfDecimal = 1.766584958675746364;
lotsOfDecimal;
const twoDecimalPlaces = lotsOfDecimal.toFixed(2);
twoDecimalPlaces;
```

Às vezes, você pode acabar com um número armazenado como um tipo de cadeia de caracteres, o que dificulta a realização de cálculos com ele. Isso geralmente acontece quando os dados são inseridos em uma entrada de formulário e o tipo de entrada é texto.

```javascript
let myNumber = "74";
myNumber = Number(myNumber) + 3;
```
## Objetos

Criando objetos.

```javascript
let dog = { name: "Spot", breed: "Dalmatian" };
```

Para recuperar as informações armazenadas no objeto.

```javascript
dog.name;
dog.breed;
// Ou
dog["name"];
dog["breed"];
```
