# Arrow Functions
De maneira geral, o javascript possuía 2 tipos de declarações de funções:
- 1º: Convencional
```javascript
function teste(params){
    comandos
}
```
- 2º: Anônimas - atribuídas a uma variável ou com parâmetro para outra função
```javascript
var teste = function (params){
    comandos
}

//ou

var sum = function (a, b){
    return a + b;
}

console.log(sum(a,b));
```

Com o surgimento do ES6, outra forma de escrever funções foi introduzida, sendo consideradas anônimas e chamadas de Arrow Functions:
- Ex.:
```javascript
var sum = (a, b) => a + b;
console.log(sum(a,b));
```
Alguns detalhes importantes para a utilização de Arrow Functions
 - Caso a função possua apenas um parâmetro, pode-se omitir os parênteses em volta deste parâmetro. Caso possua mais de um parâmetro, os parênteses são obrigatórios;
 - Em caso de necessidade de declaração de variáveis, ou executar laços, condicionais, etc, dentro da função, faz-se necessário o uso de chaves em volta do corpo desta função;
 - Caso a função seja composta apenas por uma operação, deve-se omitir o ```return```;
 - Elas não podem ser utilizadas como funções construtoras;
 - O Hoisting não se aplica a Arrow Functions;
 - Contexto de execução das Arrow Functions é relativo ao do bloco que o envolve;