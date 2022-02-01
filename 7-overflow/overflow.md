# Overflow

El desbordamiento sucede cuando el tamaño del contenido es mayor que el tamaño del contendor. Por ejemplo, si tenemos un contenedor \<div\> con un tamaño determinado (width y height) y dentro un texto cuyo tamaño es mayor, veremos como el texto se desborda.

Gracias a overflow podemos controlar este desbordamiento.

Podemos dar 4 valores diferentes a overflow:

- visible -> Es el valor por defecto
- hidden -> El contenido que se desborde no se verá. Si aplicamos esta propiedad en un solo eje el otro eje se pondra con valor scroll.
- scroll -> Aparecen las barras de scroll en el eje asignado (x, y, o ambos)
- auto -> Aparecen barras de scroll en el caso que haga falta
