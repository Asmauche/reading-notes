# READ 11

**1. ¿Qué es el DOM?**

El DOM (Document Object Model) es una interfaz de programación para los documentos HTML y XML. Representa la estructura del documento como un árbol de nodos, donde cada nodo es un objeto que representa una parte del documento, como un elemento, un atributo o un texto. Con el DOM se pueden acceder y manipular el contenido, la estructura y el estilo de los documentos de manera dinámica utilizando JavaScript.

**2. Describe brevemente la relación entre el DOM y JavaScript:**

DOM es la estructura del documento y JavaScript es la herramienta que permite interactuar con esa estructura para crear páginas web interactivas y dinámicas.

**3.¿Qué método usarías para seleccionar un elemento del DOM por su ID y cómo se utiliza?**
Para seleccionar un elemento del DOM por su ID, se puede usar el método getElementById() de JavaScript. Este método devuelve una referencia al primer objeto con el ID especificado.

```js
// Tenemos un elemento con el ID "miElemento" en HTML
// <div id="miElemento">Hola, mundo!</div>

// Se puede seleccionar este elemento con JavaScript de la siguiente manera:
var elemento = document.getElementById("miElemento");

// Ahora se puede manipular el elemento seleccionado
elemento.textContent = "¡Hola, JavaScript!";
```

**4.¿Qué método utilizarías para cambiar el color de fondo de un elemento en el DOM y cómo se implementaría?**
Para cambiar el color de fondo de un elemento en el DOM, puedes usar la propiedad style del elemento y modificar su propiedad backgroundColor:

```js
// Tenemos un elemento con el ID "miElemento" en HTML
// <div id="miElemento">Hola, mundo!</div>

// Se puede seleccionar este elemento con JavaScript de la siguiente manera:
var elemento = document.getElementById("miElemento");

// Ahora se puede cambiar el color de fondo del elemento seleccionado
elemento.style.backgroundColor = "lightblue";
```
