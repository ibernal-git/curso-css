# Margin

## Funcionamiento

Margin es un shorthand de margint-top, margin-right, margin.bottom y margin-left.

La propiedad margin admite hasta 4 valores y se computa siguiendo las agujas del reloj.

- 4 valores -> margin: top right bottom left
- 3 valores -> margin: top left/right bottom
- 2 valores -> margin: top/bottom left/right
- 1 valor -> margin: top/right/bottom/left

Si ponemos uno de los márgenes horizontales en auto:

```css
margin-right: auto;
/* o */
margin-left: auto;
```

en un elemento de bloque y, importante, este elemento tiene un tamañao declarado (width) el bloque se moverá hacia la derecha o hacia la izquierda hasta llegar al límite de su contenedor.

## Ejemplos

Ejemplos utilizando margin para diferentes elementos, utilización de margin para centrar elementos, ...

```css
body {
  background-color: #333;
  color: #fff;
}
.container {
  background-color: red;
  width: 100%;
  height: 500px;
}

.block {
  background-color: purple;
  width: 200px;
  height: 200px;
  margin: 100px 50px 10px 200px;

  /*
  
  Podemos centrar un elemento, para ello
  el elemento debe de contar con un tamaño
  y ponemos en auto los márgenes left y right
  
  */
  margin-left: auto;
  margin-right: auto;

  /* 
  
  El margin-left y margin-right están sobreescribiendo
  la propiedad margin de la línea anterior, ya sabemos que CSS
  funciona en cascada
  
  */
}

.inline {
  background-color: lightsalmon;
  color: inherit;
  margin-top: 100px;
}
```

## Margin en etiqueta body

Los navegadores suelen tener un margen sobre el body de 8px asi que si creamos un menú veremos ese espacio.

```css
.header {
  background-color: red;
  height: 50px;
}
```

Para evitarlo podemos estilar el elemento body.

```css
body {
  margin: 0;
}
```
