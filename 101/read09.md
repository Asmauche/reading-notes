# READ 09

**1. ¿Cuáles son los diferentes tipos de datos que se pueden utilizar en JavaScript y cómo se diferencian entre sí?**
El último estándar ECMAScript define ocho tipos de datos:

- Boolean: Representa valores de verdad, true o false.
- Null: Representa la ausencia intencional de cualquier valor. Es un valor asignable.
- Undefined: Indica que una variable ha sido declarada pero no se le ha asignado un valor.
- Number: Representa tanto números enteros como decimales. Ejemplo: 42, 3.14.
- BigInt. Un número entero con precisión arbitraria.
- String: Cadena de caracteres. Se define entre comillas simples o dobles. Ejemplo: 'Hola', "Mundo".
- Symbol: Representa un valor único y anónimo. Se utiliza principalmente para crear identificadores únicos.

**2. ¿Cómo se utilizan las estructuras condicionales if y else en JavaScript, y qué propósito cumplen dentro de un programa?**
Las estructuras condicionales if y else en JavaScript se utilizan para tomar decisiones en el código, permitiendo que el programa ejecute diferentes bloques de código en función de ciertas condiciones.

- La estructura if evalúa una condición y, si esta es verdadera, ejecuta el bloque de código asociado. Ejemplo:

```js
let edad = 18;

if (edad >= 18) {
    console.log("Eres mayor de edad.");
}
```

En este caso, si la variable edad es mayor o igual a 18, se imprimirá "Eres mayor de edad." en la consola.

- La estructura if-else permite definir un bloque de código alternativo que se ejecutará si la condición es falsa. Ejemplo:

```js
let edad = 16;

if (edad >= 18) {
    console.log("Eres mayor de edad.");
} else {
    console.log("Eres menor de edad.");
}
```

Aquí, si la variable edad es menor a 18, se imprimirá "Eres menor de edad." en la consola.

- El propósito de las estructuras condicionales es permitir que el programa tome decisiones y ejecute diferentes bloques de código según las condiciones especificadas. Esto es fundamental para crear programas dinámicos y adaptables que puedan responder a diferentes situaciones y entradas del usuario.

**3. ¿Cuáles son los diferentes tipos de operadores en JavaScript y cómo se utilizan los operadores aritméticos para realizar cálculos?**

Operadores Aritméticos: Se utilizan para realizar cálculos matemáticos.

- Suma (+): Añade dos valores. Ejemplo: 5 + 3 resulta en 8.

- Resta (-): Resta un valor de otro. Ejemplo: 5 - 3 resulta en 2.

- Multiplicación (*): Multiplica dos valores. Ejemplo: 5 * 3 resulta en 15.

- División (/): Divide un valor por otro. Ejemplo: 6 / 3 resulta en 2.

- Módulo (%): Devuelve el resto de una división. Ejemplo: 5 % 2 resulta en 1.

- Exponenciación (**): Eleva un valor a la potencia de otro. Ejemplo: 2 ** 3 resulta en 8.

- Incremento (++): Incrementa el valor de una variable en 1. Ejemplo: let x = 5; x++; resulta en x = 6.

- Decremento (--): Decrementa el valor de una variable en 1. Ejemplo: let x = 5; x--; resulta en x = 4.

**4. ¿Cómo se declara una variable en JavaScript y cuáles son las diferencias entre var, let y const en cuanto a su alcance y mutabilidad?**

- var: Se utiliza para declarar variables que pueden ser reasignadas. Ejemplo:

```js
var nombre = "Juan";
nombre = "Pedro";
```

- let: Similar a var, pero con un alcance más limitado. Ejemplo:

```js
let edad = 25;
edad = 30;
```

- const: Se utiliza para declarar constantes, es decir, valores que no pueden ser reasignados. Ejemplo:

```js
const PI = 3.14;
// PI = 3.14159; // Esto causará un error
```

- var: Tiene un alcance de función, lo que significa que es accesible en toda la función en la que se declara. Si se declara fuera de una función, tiene un alcance global.
- let y const: Tienen un alcance de bloque, lo que significa que solo son accesibles dentro del bloque en el que se declaran (por ejemplo, dentro de un if, for, etc.).
