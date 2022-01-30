# Box sizing

Es la propiedad que nos permite controlar el cálculo que hace el navegador a la hora de modificar las propiedades content, padding y border.

Los 2 valores que podemos darle son:

- content-box -> Valor por defecto
- border-box -> Cálculo de tamaño del elemento incluyendo el padding y el border

Si nuestra caja tiene un tamaño de 200px y aplicamos un padding 20px, el tamaño de nuestra caja habrá llegado a 240px. A los 200px de la caja sumamos 20px por cada lado del padding.

```css
.box {
  width: 200px;
  padding: 20px;
}
```

Para que nuestro width sea el tamaño total tenemos que usar border-box.

```css
.box {
  width: 200px;
  padding: 20px;
  box-sizing: border-box;
}
```

También podemos añadir un borde y aplicaría el mismo principio. En vez de añadir tamaño a la caja resta tamaño al contenido.

Si quieres tener este comportamiento en toda tu página puedes utilizar el selector universal que ya hemos visto.

```css
* {
  box-sizing: border-box;
}
```
