# Text Align

Esta propiedad nos permite alinear horizontalmente el contenido de un elemento de bloque sobre la página, **siempre que el contenido no tenga ancho declarado, si no, se centrará sobre el tamaño de la caja**.

Acepta 4 valores:

- text-align: left
- text-align: right
- text-align: center
- text-align: justify

**Importante Recordar**

- Solo funciona en elementos de bloque
- Alinea el contenido que tiene ese bloque

## Text align en imágenes

Las imágenes por defecto tienen la propiedad **display: inline-block;** con lo que no podemos aplicar text-align. Además el contenido de la imagen es la porpia imagen con lo que si cabliamos a bloque y aplicamos text-align no veremos cambios.

En este caso tenemos que centrar la propia caja con margin.

Si tenemos un contenedor y dentro una imagen podemos aplicar **text-align: center;** sobre el contenedor. En este caso tenemos que recordar que no podemos poner **display: block;** a la imagen ya que si no ocuparía toda la caja y no pasaría igual que antes. Si solamentes realizamos el text align sobre el contenedor en este caso si que nos va a centrar la imagen.
