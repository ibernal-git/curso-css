# Medidas

Las medidas se pueden agrupar en absolutas y relativas.

## Medidas absolutas

Las medidas absolutas **no cambian** y siempre mantendrán su tamaño, independientemente del dispositivo o la interacción del usuario.

La mas usada es **px** (píxeles) cuya medida es 1/96 de 1in.

Existen otras medidas como:

- cm (centimetros) -> 1cm = 96px/2,54
- mm (milímetros) -> 1mm = 1/10 de 1cm
- Q (cuarto de milímetro) -> 1Q = 1/40 de 1cm
- in (pulgadas) -> 1in = 2,54cm = 96px
- pc (picas) -> 1pc = 1/16 de 1in
- pt (puntos) -> 1pt = 1/72 de 1in

Normalmente se usa px y el resto podrían ser interesantes en salida de impresión pero no para pantalla.

## Medidas relativas

Las medidas relativas **siempre** dependen de un contexto. Se recomiendan usar en la mayoría de ocasiones porque nos van a permitir que todos los elementos escalen proporcionalmente.

Las más usadas son **em, rem, %, vw, vh, vmin y vmax**.

Existen otras medidas como:

- ex -> Altura x de la fuente del elemento
- ch -> La medida del ancho del glifo "0" de la letra del elemento
- lh -> Altura de la línea del elemento

## rem vs em

[Diferencias entre rem y em](rem-vs-em.md)

## % vs auto

[Diferencias entre % y auto](%-vs-auto.md)

## Viewport

[Medidas para el viewport](viewport.md)
