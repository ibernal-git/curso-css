# Position

Esta propiedad nos permite posicionar los elementos.

## Conceptos básicos

### Flujo de renderizado

Por norma general los elementos se dibijan de izquierda a derecha y de arriba a abajo. El punto 0,0 de los eleemntos, por norma general, es la esquina superior izquierda.

### Espacio reservado

Es el espacio que tiene un elemento asignado en el navegador.

### Elemento posicionado

Esto significa que el elemento tiene la propiedad position con un valor diferente a "static", que es el valor que tiene por defecto.

### Stacking context

Contexto de apilamiento. Es el orden en el que se apilarán las cajas que se superponene dentro del mismo contenedor.

## Propiedades que podemos utilizar

Al posicionar un elemento se habilitan 5 propiedades que podemos utilizar para mover los elementos en los 3 ejes.

- ### top

  El elemento se moverá desde la parte superior la distancia indicada.

- ### right

  El elemento se moverá desde la parte derecha la distancia indicada.

- ### bottom

  El elemento se moverá desde la parte inferior la distancia indicada.

- ### left

  El elemento se moverá desde la parte izquierda la distancia indicada.

- ### z-index

  Nos permite mover el elemento en el contexto de apilamiento (eje z).

Si a un elemento le declaramos la propiedad top, bottom ya no funciona. Lo mismo ocurre si hacemos con left y right.

## Valores que podemos dar a position

- ## static

  Es el valor por defecto. Con este valor el elemento no está posicionado por lo que no podremos moverlo.

- ## relative

  El elemento mantendrá su posición y medidas en el flujo de renderizado y mantendrá su espacio reservado. Si lo movemos lo hará usando su posición en el html como punto de referencia.

- ## absolute

  El elemento perderá sus medidas y su espacio reservado. Si lo movemos usará el elmento padre posicionado como referencia. Si no tiene ninguno usará el elemento html de referencia.

- ## fixed

  El elemento perderá sus medidas y su espacio reservado. Si lo movemos usará el elemento html de referencia y además se quedará fijo en esa posición aunque hagamos scroll.

- ## sticky

  Es un mezcla de position relative y fixed. Con este tipo de posicionamiento los valores top, left, bottom, right no sirven para mover el elemento. Estos valores sirven para indicarle en que punto pasará a tener un comportamiento de posicionamiento fixed. Hasta llegar a ese punto se comportará como si tuviera relative.
