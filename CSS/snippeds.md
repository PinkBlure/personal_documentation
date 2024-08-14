## Media Queries

Ecribir las Media Queries puede ser tedioso, entonces hacemos un atajo en el ide para ello.

Vamos a las opciones de snippeds y vamos al archivo de css.

```json
"Crea un Media Querie": {
    "prefix": "mq",
    "body": "@media (min-width: $1) {\n    $2\n}"
}
```

Al escribir mq en el css nos saldrá directamente todo el cuerpo de la query, y el cursor parará primero en donde el $1 y al tabular se colocará en la segunda posición $2,