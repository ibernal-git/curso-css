# Border

Es la propiedad que nos permite modificar el borde de la caja. Es un **shorthand** (propiedad abreviada) que agrupa 3 propiedades:

- border-width: ancho del borde
- border-style: estilo del borde
- border-color: color del borde

## Ejemplo

```css
.button {
  border: 20px solid red;
}
.button-2 {
  border-width: 20px;
  border-style: solid;
  border-color: red;
}
```

A su vez border-width es un **shorthand** de:

- border-top-width
- border-right-width
- border-bottom-width
- border-left-width

border-style es un **shorthand** de:

- border-top-style
- border-right-style
- border-bottom-style
- border-left-style

border-color es un **shorthand** de:

- border-top-color
- border-right-color
- border-bottom-color
- border-left-color

## Listado de valores para la propiedad style

- none
- hidden
- dotted
- dashed
- solid
- double
- groove
- ridge
- inset
- outset
