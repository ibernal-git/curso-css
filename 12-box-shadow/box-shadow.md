# Box shadow

La propiedad box-shadow se creo para añadir efectos de sombra a las cajas.

Box shadow crea un clon de la caja respetando la forma de su box-model (ancho, alto, border).

La sintaxis de box-shadow se puede escribir de distintas formas en función de lo que queramos conseguir.

- offset-x -> Desplazamiento en x (obligatorio)
- offset-y -> Desplazamiento en y (obligatorio)
- blur-radius -> Desenfoque de la sombra
- spread-radius -> Expansión de la sombra
- color -> El color de la sombra, si no lo es pecificamos se hereda
- inset -> Determina si la sombra será interior o exterior

## Ejemplo

```css
/* 

Desplazamos la sombra 10px en horizontal y 25px en vertical

*/

.box {
  box-shadow: 10px 25px;
}

/* Aplicamos un desenfoque */

.box {
  box-shadow: 5px 5px 10px;
}

/* Establecemos un color */

.box {
  box-shadow: 5px 5px 10px blue;
}

/* Expandimos la sombra */

.box {
  box-shadow: 5px 5px 10px 20px;
}

/*

Expandimos la sombra sin desenfoque y con color.
Ademas quitamos el desplazamiento horizontal

*/

.box {
  box-shadow: 0 30px 0 10px 20px red;
}

/* Dibujamos la sombra por dentro */

.box {
  box-shadow: inset 10px 0 10px 0 red;
}
```

Podemos añadir varias sombras separando los valores con comas.

```css
.box {
  box-shadow: 5px 5px red, 10px 10px blue;
}
```
