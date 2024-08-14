## Especificidad de los selectores

Cuando aplicamos el css hay que tener en cuenta que el css es en cascada, es decir, lee el archivo de arriba a abajo, pero tambien tiene en cuenta la especificidad de los atributos.

```css
p {
    color: blue;
}

p {
    color: red;
}
```

En este ejemplo, como solo es un selector de una etiqueta en ambos casos y tienen el mismo grado de especificidad, se aplicará el último leído por el fichero. Es decir, el de color rojo.

```css
p.parrafo {
    color: blue;
}

p {
    color: red;
}
```

En este ejemplo, podemos ver que el selector de arriba es más específico al hacer referencia a las etiquetas p con una clase aplicada llamada parrafo. En la página web veríamos como todos los textos que se encuentran con una etiqueta p se sobreescriben con el color rojo, menos los que tengan como clase parrafo, ya que al ser ese selector que cambia a azul el texto más específico que el que cambia a rojo, no se sobreescribe.

```css
p#parrafo {
    color: blue;
}

p {
    color: red!important;
}
```

Usar el !important hace que el atributo de ese selector ignore la especificidad y se aplique, pero no es recomendable su uso.

## Probar la página web en diferentes navegadores

Como cada navegador es diferente, hay que normalizar los elementos de los navegadores para que nuestra página se vea igual sin importar el navegador.

Para esto existe normalize.css que se puede poner en un archivo a parte.

[Ir a normalize.css](https://necolas.github.io/normalize.css/)

## ¿BEM, Utility first, módulos?

Son formas de escribir el css.

* BEM

Significa bloques, elementos y modificadores.

```css
.card {}
.card__titulo {}
.card__imagen {}
.card__boton {}
.card__boton--activo {}
```

* Utility first

```css
.text-center {}
.color-red-100 {}
.bg-blue-200 {}
.p-2 {}
.m-2 {}
```

* Módulos

```css
.card {}
.card h2 {}
.card img {}
.card a {}
```

## Arreglar el box-sizing

Para no calcular las sumas de los altos y anchos con los paddings tenemos lo siguiente.

```css
html {
    box-sizing: border-box;
}

body {
    box-sizing: inherit;
}
```

Nos ayuda a respetar las medidas del ancho y alto de los elementos.