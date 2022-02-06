# % vs auto

Cuando usamos % para establecer el tamaño vertical a un elemento tenemos que tener en cuenta que el elemento contenedor tienen que tener un tamaño establecido.

Si no tiene un tamaño vertical su tamaño es **auto** con lo cual si no tiene contenido no se renderizará y el % del elemento hijo no funcionará.

```html
<body>
  <div class="box">
    <div class="box-children"></div>
  </div>
</body>
```

```css
/*

En este ejemplo ni box ni box-children tienen contenido asi que no se renderiza nada

*/

.box {
  width: 100%;
  background-color: antiquewhite;
}

.box-children {
  height: 50%;
  width: 50%;
  background-color: aquamarine;
}
```

Aunque no tenga contenido si el elemento padre tiene tamaño:

```html
<body>
  <div class="box">
    <div class="box-children"></div>
  </div>
</body>
```

```css
/*

En este ejemplo box no tiene contenido pero si que tiene un tamaño de 40px asi que box-children ocupara 40px de alto ya que tiene height: 100%.

*/

.box {
  height: 40px;
}

.box-children {
  height: 100%;
  background-color: antiquewhite;
}
```

Si por ejemplo el elemento no tiene contenedor, está en el body, y aplicamos un 100% al height. En este caso ocurre lo mismo, el tamaño se ajustará al tamaño del contenido, no ocupara el 100% del body ya no tiene un tamaño declarado, así que el navegador lo trata como si tuviera un height: auto;

```html
<body>
  <div class="box"></div>
</body>
```

```css
/*

En este ejemplo box no tiene contenido asi que no se renderiza nada y si tuviera contenido se ajustaría a ese contenido.

*/

.box {
  height: 100%;
  background-color: antiquewhite;
}
```

**En los tres casos anteriores el height depende del contenido o de que su elemento contenedor tenga establecida un tamaño de alto**

## Peligro del height

Es peligroso declarar un height a un elemento ya que si cambia su contenido puede romper los estilos. Si por ejemplo necesitas que haya un espacio al final del contenido es mejor utilizar un padding-bottom. Si se añade más contenido lograrás que el estilo siga funcionando.

```css
.box {
  /* height: 250px; */
  padding-bottom: 20px;
}
```

## Height y position absolute

Si al elemento que declaramos con un porcentaje en el height también declaramos que tenga **position: absolute;** lo que hará en ese caso es calcular el tamaño del height en base al **viewport**.

```css
.box {
  position: absolute;
  height: 50%;
}
```

## Diseño mobile only

Si lo que quieres es que sí tenga height y el contenido que se desborde se oculte. Por ejemplo al hacer un diseño mobile only. Puedes establecer el height pero teniendo en cuenta que tendrás que usar la propiedad overflow para controlar el desbordamiento.

```css
.box {
  position: absolute;
  width: 375px;
  height: 80%;
  overflow: auto;
}
```
