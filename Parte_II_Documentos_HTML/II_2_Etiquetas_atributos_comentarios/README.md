Anteriormente hemos definido **HTML** como un lenguaje de marcas o etiquetas pero, ¿qué es eso de una etiqueta? y ¿qué tipos de etiquetas tengo?

Básicamente podemos distinguir entre dos tipos de etiquetas:

- Etiquetas con contenido
- Etiquetas sin contenido

### Etiquetas con contenido.

Son etiquetas que tiene tres partes (por este orden)

1. Apertura de la etiqueta
2. Contenido de la etiqueta
3. Cierre de la etiqueta

Algo así:

```xml
    <etiqueta>
        Contenido de la etiqueta
    </etiqueta>
```

HTML tiene un número limitado de etiquetas y no es necesario conocer todas. Con una lista más o menos pequeña podemos construir la gran mayoría de páginas web. En caso contrario, siempre podemos visitar las referencias.

Un ejemplo de etiqueta de HTML con contenido sería un párrafo:

```html
    <p>
        HOLA MUNDO
    </p>
```

- **<p\>** Sería la apertura
- **HOLA MUNDO** sería el contenido, en este caso sólo texto aunque podríamos meter muchas cosas "dentro"
- **</p\>** Sería el cierre de la etiqueta

### Etiquetas sin contenido

Son etiquetas que sólo tienen parte de apertura y carecen de contenido. Pueden estar cerradas o no, aunque yo recomiendo que se cierren. De esta manera:

- `<etiqueta >`
- `<etiqueta />`

Un ejemplo de etiqueta HTML sin contenido sería una imagen:

```html
<img ...  />
```

### Atributos

Las etiquetas pueden tener atributos de los que nos interesa saber lo siguiente:

- Proporcionan información adicional sobre la etiqueta.
- Las etiquetas puede tener o no tener atributos e incluso tener más de uno.
- Siempre se añaden en la etiqueta de apertura.
- Hay atributos generales (para todas) o específicos (para algunas).
- Se respresentan nombre_atributo="valor_atributo".

Un ejemplo:

```html
<img src="foto.png"  />
```

### Tipos de etiquetas

Hay muchos tipos de etiquetas pero a lo largo de este curso vamos a centrarnos en las siguientes:

- Etiquetas de cabecera
- Etiquetas de texto
- Etiquetas de imágenes, tablas, listas y enlaces
- Etiquetas multimedia
- Etiquetas semánticas
- Y alguna más pero no todas ;) .

### Comentarios

Además de todas estas etiquetas nuestra página web podrá llevar comentarios que son, normalmente, texto descriptivos que no se van a mostrar en nuestra web.

Los comentarios van encerrados en esta estructura **`<!-- -->`** y un ejemplo sería:

```html
<!-- Esto es un comentario en HTML -->
```
