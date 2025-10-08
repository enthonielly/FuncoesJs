# FuncoesJs

Este projeto tem como objetivo explicar como **definir e criar funções em JavaScript** utilizando os formatos:

- **Function Declaration**
- **Function Expression**
- **Arrow Function**

## O que são funções?
>Funções em JavaScript são blocos de código reutilizáveis que executam uma tarefa específica.  
>Elas permitem organizar melhor o código, evitar repetições e tornar o programa mais legível.

## Tipos de funções em JavaScript

***
 ### 1. Function Declaration
>É a forma mais tradicional de declarar funções.
>Elas são **içadas (hoisted)**, ou seja, podem ser chamadas antes mesmo de serem definidas no código.

```
 //Declaração
function saudacao(nome) {
  return `Olá, ${nome}!`;
}

 //Uso
console.log(saudacao("Maria")); // Olá, Maria!
```

- Vantagens: pode ser chamada em qualquer parte do código, mesmo antes da declaração.  
- Atenção: sobrescrevê-la pode causar problemas em códigos maiores.
***

 ### 2. Function Expression
>A função é atribuída a uma variável ou constante.
>Diferente da declaration, não sofre hoisting (só pode ser chamada após ser definida).

```
// Expressão
const soma = function (a, b) {
  return a + b;
};

// Uso
console.log(soma(5, 3)); // 8
```

- Vantagem: maior controle sobre o escopo da função.  
- Atenção: precisa ser definida antes de ser usada.
***

 ### 3. Arrow Function
>Introduzidas no ES6, são funções mais curtas e modernas.
>Além disso, não têm seu próprio 'this', herdando do contexto onde foram criadas.

```
// Arrow Function
const multiplicar = (a, b) => a * b;

// Uso
console.log(multiplicar(4, 6)); // 24
````

- Vantagens: sintaxe curta e limpa; ótima para callbacks e funções anônimas.  
- Atenção: não podem ser usadas como construtoras (com new); cuidado ao usar com objetos que dependem de 'this'.
***
