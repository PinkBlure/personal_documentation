## Tamaño de las fuentes responsive

Hay muchas veces que es complicado hacer las fuentes responsive, y las medidas rem pueden resultar liosas de usar.

Para esto, podemos añadir al principio de nuestro archivo css:

```css
html {
    font-size: 62.5%;
}

body {
    font-size: 16px;
}
```

Esta configuración nos permite adaptar la medida del rem a que 1rem es igual a 10px, facilitando el uso del rem para el programador y manteniendo la ventaja de ser responsive del rem.

## Fuentes bonitas

* Krub - Google fonts

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Krub:wght@400;700&display=swap" rel="stylesheet">
```

```css
font-family: "Krub", sans-serif;
```