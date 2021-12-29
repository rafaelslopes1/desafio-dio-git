# Default Functions Arguments

Com o surgimento do ES6, foi introduzida a possibilidade de se atribuir valores padrão aos atributos de uma função, que serão válidos caso o parâmetro não seja recebido, ou caso o parâmetro tenha sido recebido como ```undefined```

```javascript
//Antes
function multiply(a, b){
    b = typeof b === 'undefined' ? 1 : b;

    return a*b;
}
//ou
function multiply(a, b){
    if(typeof b === 'undefined'){
        b = 1;
    }

    return a*b;
}

//Depois
function multiply(a, b=1){
    return a*b;
}
```

Alguns detalhes importantes:
- Pode-se referenciar outros parâmetros da função, atribuindo os seus valores aos parâmetros que o sucedem (importante lembrar que não é possível referenciar parâmetros que ainda não foram declarados);