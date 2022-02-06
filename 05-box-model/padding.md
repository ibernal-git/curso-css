# Padding

Es la propiedad que nos permite generar espacio interno entre el borde y y la caja.

Es un **shorthand** (propiedad abreviada) que controla los 4 lados posibles a los que dar padding.

- padding-top
- padding-right
- padding-bottom
- padding-left

Admite hasta 4 valores que van en el sentido de las agujas del reloj.

- 4 valores -> padding: top right bottom left
- 3 valores -> padding: top left/right bottom
- 2 valores -> padding: top/bottom left/right
- 1 valor -> padding: top/right/bottom/left

## Ejemplo

```css
.box {
  padding: 50px 60px 20px 10px;
}

.box-2 {
  padding: 0 25px;
}

.box-3 {
  padding-top: 10px;
}
```
