# Enhanced Object Literals

O ES6 trouxe como novidade alguns atalhos na declaração de objetos literais. Podemos citar os seguintes:

```javascript
//atribuir valores já existentes (variáveis e métodos) a atributos do objeto
const prop1 = 'Hello World!';
function metodo1(){
    console.log('Sou o método 1');
}

const objeto1 = {
    prop1: prop1,
    metodo1: metodo1()
}
//pode ser resumido em 
const objeto2 = {
    prop1,
    metodo1
}

//outra forma de atribuir métodos a atributos de objetos é declarando-os dentro dos objetos. Ex.:
const objeto3 = {
    metodo2 =  function(a, b){
        return a+b;
    }
}

```