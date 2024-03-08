---
author: Andres Parra
pubDatetime: 2024-03-08T17:48:00-05:00
title: "Fundamentos de JavaScript III: Tipo de Dato number en JavaScript"
slug: "tipo-number"
featured: true
draft: false
tags:
  - JavaScript
  - Number
description: "El tipo de dato number en JavaScript es utilizado para representar números, ya sean enteros o de punto flotante. En este artículo, exploraremos en detalle el tipo de dato number, incluyendo cómo se declara, las operaciones que se pueden realizar con él y algunas consideraciones importantes a tener en cuenta al trabajar con números en JavaScript."
---

El tipo de dato "number" en JavaScript es utilizado para representar números, ya sean enteros o de punto flotante. En este artículo, exploraremos en detalle el tipo de dato "number", incluyendo cómo se declara, las operaciones que se pueden realizar con él y algunas consideraciones importantes a tener en cuenta al trabajar con números en JavaScript.

## Declaración de Variables de Tipo "number"

Para declarar una variable de tipo "number" en JavaScript, simplemente utilizamos la palabra clave `var`, `let` o `const`, seguida del nombre de la variable y el valor numérico. No es necesario especificar explícitamente el tipo de dato "number", ya que JavaScript es un lenguaje de tipado dinámico.

```javascript
var edad = 30;
let precio = 49.99;
const PI = 3.14159;
```

En este ejemplo, hemos declarado tres variables de tipo "number": `edad` que es un número entero, `precio` que es un número de punto flotante y `PI` que es una constante con un valor numérico.

## Operaciones con Números

JavaScript proporciona una amplia variedad de operaciones que se pueden realizar con números, incluyendo operaciones aritméticas básicas como suma, resta, multiplicación y división, así como operaciones más avanzadas como exponenciación y operadores de asignación abreviada.

```javascript
var x = 10;
var y = 5;

var suma = x + y;
var resta = x - y;
var multiplicacion = x * y;
var division = x / y;
var exponenciacion = x ** y;

console.log("Suma:", suma);
console.log("Resta:", resta);
console.log("Multiplicación:", multiplicacion);
console.log("División:", division);
console.log("Exponenciación:", exponenciacion);
```

## Consideraciones Importantes

Al trabajar con números en JavaScript, es importante tener en cuenta algunas consideraciones, como la precisión de los cálculos con números de punto flotante, los límites de los números en JavaScript y los casos especiales como NaN (Not a Number) e Infinity.

```javascript
console.log(0.1 + 0.2); // 0.30000000000000004
console.log(Number.MAX_VALUE); // 1.7976931348623157e+308
console.log(Number.MIN_VALUE); // 5e-324
console.log(1 / 0); // Infinity
console.log("abc" / 5); // NaN
```
