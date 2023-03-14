## Propiedades específicas de navegadores

En uno de los apartados anteriores de este mismo curso hablamos de CSS3. Dijimos que era una especificación modular, extensa y que se iba implantándose poco a poco.

Los distintos navegadores conforme dan soporte a propiedades experimentales lo que hacen es añadirles un prefijo para indicar que ellos sí les han dado soporte antes de que sean soportadas por los demás o antes de que sean parte del estándar.

Estos son los llamados **prefijos de navegadores** y tienen una síntaxis similar a la siguiente:

```css
a {
  -webkit-transition: -webkit-transform 1s;
  transition: -ms-transform 1s;
  transition: transform 1s;
}
```

Y los valores más comunes de esos prefijos son:

- **\-webkit** para Chrome, Safari, nuevas versiones de Opera y para Firefox para iOS
- **\-moz** para navegadores Firefox que no sean para iOS
- **\-o** para versiones antiguas de Opera
- **\-ms** para Internet Explorer y Microsoft Edge

El problema que surge es que nosotros, como desarrolladores no sabemos cuándo usarlo. CSS3 es una especificación larga con muchos módulos y es prácticamente imposible saber cuando hay que añadir estos prefijos o cuándo las propiedades han dejado de ser experimentales.

Tenemos la suerte, no obstante de tener varias herramientas para ello.

- [ShoudIPrefix](http://shouldiprefix.com/)
- [Autoprefixer](https://github.com/postcss/autoprefixer)
