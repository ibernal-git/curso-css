# Ordenar las propiedades

No existe ninguna norma ni especificación para ordenar las propiedades cuando estilamos nuestros elementos. De todas maneras es recomnedable seguir un patrón y hacerlo siempre de esta manera para que al trabajar y/o revisar el código podamos hacerlo de la mejor manera y con la mayor rapidez.

La mayoría de expertos coinciden que se debe ordenar las propiedades de la siguiente manera.

1. Propiedades de posicionamiento
2. Propiedades del box model
3. Propiedades del texto
4. Propiedades visuales (colores, bordes, background, ...)
5. El resto

## Ejemplo

```css
.box {

  /* Position */
  position: relative;
  top: 0;
  left: 0;

  /* Box Model */
  display: block:
  width: 300px;
  height: 300px;
  padding: 10px;
  margin: 10px;
  overflow: hidden;

  /* Text */
  font-size: 16px;
  text-align: center;

  /* Visual */
  color: white;
  border: 2px solid red;
  border-radius: 10px;

  /* Other properties */
  opacity: 1;
}
```
