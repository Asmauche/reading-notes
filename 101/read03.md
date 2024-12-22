# ¿Qué es y cómo funciona CSS?

CSS (Cascading Style Sheets) es un lenguaje utilizado para describir la presentación visual de un documento HTML. Permite definir estilos como colores, fuentes, tamaños y diseño, mejorando la apariencia y experiencia de usuario en la web.

## ¿Como insertar CSS

**En línea**  

Se usa el atributo `style` dentro de una etiqueta HTML:  

```html:
<p style="color: blue; font-size: 16px;">Texto con estilo en línea<p/>
```

**En una hoja de estilo interna**

Se escribe dentro de la etiqueta `style` en el `head` del documento HTML:
```html
<style>
    p {
        color: blue;
        font-size: 16px;
    }
</style>
```

**En una hoja de estilo externa**

Se enlaza un archivo CSS externo mediante 
`link` en el `head`:
```html
<link rel="stylesheet" href="estilos.css">
```



## Partes esenciales de CSS

1. **Selectores**  
   Identifican los elementos HTML a los que se aplicarán los estilos. Algunos ejemplos:  
   - `elemento`: Selecciona todas las etiquetas de ese tipo (p. ej., `p` para párrafos).  
   - `.clase`: Selecciona elementos con una clase específica.  
   - `#id`: Selecciona un elemento único con un identificador.

2. **Propiedades y valores**  
   Definen cómo se aplicarán los estilos. Cada propiedad tiene un valor asociado. Ejemplos:  
   - `color: red;` (color del texto).  
   - `font-size: 16px;` (tamaño de fuente).  
   - `margin: 10px;` (margen alrededor del elemento).

3. **Reglas de cascada**  
   Determinan qué estilos se aplican cuando hay conflictos. La prioridad sigue este orden:  
   - Estilos en línea (dentro del atributo `style`).  
   - Estilos en una hoja de estilo interna (`<style>` en el HTML).  
   - Estilos en hojas de estilo externas (archivos `.css`).

## Resumen del funcionamiento de CSS

1. El navegador carga el documento HTML y su hoja de estilo CSS.  
2. CSS aplica estilos a los elementos HTML según los selectores y las reglas definidas.  
3. El resultado es una página con un diseño visual coherente y atractivo.
