## Añadir estilos a HTML

En apartados anteriores de este mismo curso hemos ido, de manera esporádica, añadiendo estilos en algunos ejercicios.

Ahora vamos a ver existen otras formas de añadir estos estilos y vamos a explicar qué formas son más recomendables y porqué.

De manera general podremos añadir CSS a nuestro HTML de cuatro formas:

- **Estilos In-line**
- **Etiqueta Style**
- **Directiva `@import` **
- **Etiqueta link**

### Estilos In-line

La inclusión de estilos In-line consiste en la inclusión de estilos visuales usando el atributo **style** de las etiquetas.

Este atributo es una atributo general que está presente en todas aquellas etiquetas que sirven para describir el contenido de la página.

Un ejemplo de estilos In-Line sería:

```html
    <h1 style="color:red">
    ...
    <h1>
    ...
    <h2 style="color:red">
    ...
    <h2>
```

Es directo pero si quieres realizar un cambio en todos los elementos que tienen ese color de letra en éste y en todos los demás fichero de mi sitio tendrías un montón de trabajo.

### Etiqueta Style

La etiqueta **`<style>`** me permite definir todos los estilos de una misma página web en un único sitio que, normalmente, suele estar en la cabecera.

Un ejemplo del uso de esta etiqueta sería:

```html
    <style>
     h2 {
         color: green;
     }
    </style>
```

Si hubiera algún cambio en el estilo de mi sitio sólo tendría que hacerlo una vez por página. Sigue siendo mucho trabajo si mi sitio web está compuesto, por ejemplo, por miles de páginas.

### Directiva `@import`

Nos permite importar un fichero css directamente en nuestro HTML.

Se utiliza dentro de la etiqueta **style** de esta manera:

```html
    <style>
        @import 'css/import.css';
    </style>
```

_import.css_ sería el nombre de nuestro fichero de estilos puediendo ser el que nosotros queramos.

Utilizar esta técnica me permite realizar cambios en el estilo de toda mi web únicamente tocando un fichero.

Sin embargo hay un inconveniente. El rendimiento, ya que es bloqueante en algunos navegadores, y se para la descarga del resto de la página hasta que no se ha descargado la hoja de estilos.

Por lo tanto hay que usar esta opción con cuidado.

### Etiqueta Link

Es la opción que os recomiendo. Tendremos un único punto de cambio y a la vez no es bloqueante.

Un ejemplo de uso de esta etiqueta, que se pone dentro de la cabecera, es:

```html
    <link href="css/estilos.css" rel="stylesheet" type="text/css" />
```

Tiene tres atributos en los que indicamos qué fichero quiero (_href_), que tipo de fichero es (_type_) y relación que existe entre el documento y el documento enlazado (_rel_)
