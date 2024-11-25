# Estudando JavaScript

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
