De igual manera, veremos que al trabajar en proyectos grandes con CSS hay tareas que son tediosas y que favorecen la aparación de errores. Para evitar esto han ido surgiendo muchas herramientas pero aquellas que han tenido más éxito y que deberías conocer son los preprocesdores CSS.

Un **preprocesador CSS** es un programa que te permite generar CSS...haciendo que la estructura sea más legible y más fácil de mantener.

Añaden al CSS tradicional características como:

- Las **variables**
- Los **selectores anidados**
- Los **bucles**
- Los **mixins**
- Etc.

Y los preprocesadores más conocidos son: **LESS**,**SASS** y **POSTCSS** que no es exactamente un preprocesador pero nos va a facilitar mucho el trabajo con CSS y es fácilmente extensible.

Un ejemplo sería:

```css
$font-stack: Helvetica, sans-serif;
$primary-color: #333;

body {
  font: 100% $font-stack;
  color: $primary-color;
}
```

Donde estamos usando variables, la variable **$font-stack**
