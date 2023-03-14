## Otras etiquetas

Estamos llegando al final de lo que queríamos saber sobre HTML. Recordaros que este es un curso de **INTRODUCCIÓN** que pretende ser directo y práctico.

HTML5 tiene muchas más cosas y muchas más etiquetas que no hemos visto. Algunas se escapan al contenido por su complejidad y otras no se van a incluir por mantener las cosas simples.

Hay que conocer la base y saber usar las referencias, esto es fundamental en la informática de hoy en día. Conforme vayamos practicando iremos abandonando las referencias las cuáles sólo visitaremos para consultas muy puntuales.

No obstante, antes de _"cerrar"_ la lista de etiquetas vamos a comentar de manera rápida algunas más que puede ser interesantes. No las vamos a ver en detalle pero pondremos un ejemplo para cada una de ellas.

- **`<iframe>`** nos permite mostrar páginas web dentro de otras páginas.

```html
<!-- Etiqueta iFrame -->
<iframe src="http://www.as.com" height="300px" width="600px"></iframe>
```

- **`<canvas>`** nos permite dibujar, animar y un mundo infinito de posibilidades. Es la base de todos los juegos HTML5, desde el más sencillo al más complejo.

- **`<div>`** es una etiqueta para separar las secciones de los documentos y que se utiliza para maquetar. Es el elemento en bloque por excelencia. Ya veremos luego lo que eso significa.

```html
<div>
  Some text inside a div
</div>
```

- **`<span>`** es un elemento en línea que no aporta nada visualmente pero que a nivel lógico me sirve para, por ejemplo, podeer distinguir ciertas partes dentro de un texto. Ya veremos luego lo que significa _"en línea"_.

```html
and some text with <span>span</span>
```

- **`<script>`** nos sirve para introducir código escrito en otros lenguajes, típicamente en javascript.

```html
<script>
    var nombre = prompt("Hola como te llamas?");
    alert("Encantado " + nombre);
</script>
```

- **`<object>`** y **`<embed>`** sirven para mostrar documento externos o de terceros en la pantalla del navegador. Su uso y significado es similar pero el segundo ha quedado _deprecated_ lo que sinifica que puede llegar algún momento en el que los navegadores no lo entiedan.

```html
<!-- Adding external objects with object -->
    <!-- docs, videos, svg, depende de plugins de terceros-->
    <object type="application/pdf" data="https://www.um.es/atica/documentos/html.pdf" width="300" height="200">
    </object>

    <embed type="application/pdf" src="https://www.um.es/atica/documentos/html.pdf" width="300" height="200" />
```
