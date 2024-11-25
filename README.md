# Estudando JavaScript
Aqui, vamos explorar alguns tópicos e destacar principalmente as diferenças em relação a outras linguagens. Meu conhecimento é focado em C e Java, então, se eu não mencionar algo sobre o assunto, pode assumir que é igual ao que acontece nessas linguagens.

## Caracteriscas
- Todas as instruções de código devem terminar com um ponto-e-vírgula `;`.
- As variáveis diferenciam maiúsculas de minúsculas.

## Tipos de variáveis
JavaScript é uma "linguagem tipada dinamicamente", o que significa que, ao contrário de algumas outras linguagens, você não precisa especificar qual tipo de dados uma variável conterá (números, strings, arrays, etc.).

```javascript
let myNameArray = ["Chris", "Bob", "Jim"];
let myNumberArray = [10, 15, 40];
```

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

```
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
