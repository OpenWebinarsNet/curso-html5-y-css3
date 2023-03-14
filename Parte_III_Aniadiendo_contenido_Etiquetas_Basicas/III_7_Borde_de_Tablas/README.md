## Borde de las tablas

En el apartado anterior, apartado en el que hemos presentado las tablas, no hemos hablado para nada de los bordes que normalmente pueden presentar estas estructuras.

De hecho habéis podido ver que, por defecto, los navegadores no le ponen borde a las tablas.

Para ponerles bordes nos tenemos que adelantar un poquito en el temario y hablar de estilos, de CSS.

No es totalmente correcto lo que vamos a hacer aquí, pero nos va a servir para entender los tipos de bordes más usados (hay muchos más).

En princio lo que vamos a hacer es lo siguiente:

```html
    <head>
        ...
        <!--Etiqueta para definir estilos-->
        <!-- Aquí definiremos los bordes-->
        <style>
            ...
            /*Estilos para los bordes*/
            ...
        </style>

    </head>
```

Y vamos a presentar tres tipos de bordes, los que considero más usados.

- **Bordes Simple**
- **Bordes sin colapsar**
- **Bordes inferior o superior**

### Bordes Simples

Pondremos dentro la etiqueta **`<style>`** lo siguiente:

```css
table {
  border-collapse: collapse;
}

td,
th {
  border: 1px solid black;
}
```

### Bordes sin Colapsar

Pondremos dentro la etiqueta **`<style>`** lo siguiente:

```css
table,
td,
th {
  border: 1px solid black;
}
```

### Bordes Inferior/Superior

Pondremos dentro la etiqueta **`<style>`** lo siguiente:

```css
table {
  border-collapse: collapse;
}

td,
th {
  border-bottom: 1px solid black;
}
```

Si lo quisiéramos superior debemos cambiar _border-bottom_ por _border-top_.
