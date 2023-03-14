## Imagenes, enlaces y rutas

Tras añadir elementos de texto a nuestra página, al cuerpo <body> de la misma, vamos a continuar mejorando y haciendo nuestras webs más bonitas e interactivas ya que, hasta ahora, lo que hemos venido creando es realmente "feo".

Para ello, en este apartado vamos a añadir dos elementos básicos en toda web:

- Las imágenes
- Los enlaces

Y además, explicaremos qué es un ruta y las clases que hay ya que, estos dos elementos anteriores, van a utilizar rutas en sus atributos.

### Imágene simples

La inclusión de imágenes simples se viene haciendo desde las primeras versiones de HTML con la etiqueta sin contendio **`<img .../>`**

Los atributos más comunes que le podemos poner a esta etiqueta son:

- **src:** que indica la ruta en la que se encuentra el archivo de la imagen.
- **alt:** un texto alternativo para describir la imagen en caso de que no se cargue o para dispositivos especiales para usuarios con discapacidad visual (por ejemplo)
- **width:** para especificar la anchura de la imagen (px, % etc..). Si no se escogerá la anchura propia de la misma.
- **height:** para especificar la altura de la imagen (px, % etc..). Si no se escogerá la altura propia de la misma.

Es importante destacar que la imagen es un elemento en línea que se pone, si cabe, inmediatamente después de los elementos previamente añadidos.

Algunos ejemplos de utilización de estos atributos podrían ser:

```html
    <!-- Si no pongo nada se respetan las dimensiones originales de la imagen-->
    <!-- Ruta relativa -->
    <img alt="Logo de OpenWebinars" src="img/openwebinars-logo.jpg">


    <!-- Ruta absoluta -->
    <img alt="Logo de OpenWebinars" src="/home/pekechis/public_html/openwebinars_iniciacion_html_css/Parte_III_Aniadiendo_contenido_Etiquetas_Basicas/examples/img/openwebinars-logo.jpg">

    <!-- Ruta URL -->
    <img alt="Logo de OpenWebinars" src="https://www.linuxadictos.com/wp-content/uploads/openwebinars-logo.jpg">

    <!-- Si modifico una dimensión se respetan las proporciones-->
    <img height="50px" alt="Logo de OpenWebinars" src="img/openwebinars-logo.jpg">
    <img width="50px" alt="Logo de OpenWebinars" src="img/openwebinars-logo.jpg">

    <!-- Si pongo ambas dimensiones puedo modificar las proporciones-->
    <img height="300px" width="100px" alt="Logo de OpenWebinars" src="img/openwebinars-logo.jpg">
```

### Rutas

El concepto de ruta es un concepto muy importante ya que se utiliza es muchos temas relacionados con la informática y en concreto, en la creación de páginas WEB, se utiliza para referenciar archivos, recursos y/o partes de alguna web. De manera general podemos distinguir:

- **Relativas:** Toman como base el directorio en el que se encuentra nuestro fichero. Son las recomendadas.

```html
    <img alt="Logo de OpenWebinars" src="img/openwebinars-logo.jpg">
```

- **Absolutas:** Toman como base el directorio raíz de mi equipo (/ en Linux y c:\\ en Windows). Cuidado, sólo funcionarán en tu mismo equipo.

```html
    <img alt="Logo de OpenWebinars" src="/home/pekechis/public_html/openwebinars_iniciacion_html_css/Parte_III_Aniadiendo_contenido_Etiquetas_Basicas/examples/img/openwebinars-logo.jpg">
```

- **Url:** La dirección de Internet de un recurso (fichero, imagen etc..). Puede desaparecer y entonces dejará de mostrarse en nuestra web.

```html
<img alt="Logo de OpenWebinars" src="https://www.linuxadictos.com/wp-content/uploads/openwebinars-logo.jpg">
```

### Figuras

Una novedad en HTML5 es la construcción de etiquetas alrededor de **<figure>** que nos va a permitir mostrar una imagen con un texto asociado.

En este caso el árbol DOM será el siguiente:

![Árbol DOM  para una figura](./img/figure_dom.png)

Donde:

- **`<figure>`** es la etiqueta padre.
- **`<img ../>`** es una etiqueta de imagen que hemos visto anteriormente.
- **`<figcaption>`** es una etiqueta que contendrá el texto asociado a la imagen.

Un ejemplo:

```html
<figure>
        <img alt="Logo de OpenWebinars" src="img/openwebinars-logo.jpg">
        <figcaption>Logotipo de OpenWebinars con la etiqueta figure</figcaption>
    </figure>
```

### Enlaces

Los enlaces, que se representan mediante el uso de la etiqueta **`<a>`** es una de las contrucciones más importantes en HTML. Esta etiqueta puede tener varios atributos, de lo cuáles los más importante son:

- **href:** que es la dirección de Internet de destino (ya sea otra página web, un imágen, un fichero o lo que sea).
- **target:** que indica dónde voy a abrir ese enlace. Si no pongo nada se abrirá en la misma pantalla y si le doy el valor **target="\_blank"** se abrirá en una nueva ventana de mi navegador.

Varios ejemplos de enlaces:

```html
<p><a href="http://www.openwebinars.net">Esto en un enlace en la propia página</a></p>

 <p><a href="http://www.openwebinars.net" target="_blank">Esto en un enlace en la propia página</a></p>

<!-- Haciendo que una imagen sea enlace. Anidando etiquetas -->
<a href="http://www.openwebinars.net"><img width="100px" alt="Logo de OpenWebinars" src="img/openwebinars-logo.jpg"></a>
```

### Enlaces dentro de la misma página

Puedo enlazar enlaces dentro de la misma página con construcciones como la siguiente:

```html
    ...
    <a href="#contacto">Contacto</a>
    ...
    <section id="contacto">
        .....
    </section>
    ....
```

