# VIEWPORT

El viewport es el área util donde se mostrará la página web. Este área no tiene en cuenta el scroll, simplemente es lo que se puede ver.

## Podemos usar viewport con las siguientes medidas:

- vw
- vh
- vmax
- vmin

### vw

Viewport Width. Hace referencia al ancho del viewport.

### vh

Viewport Width. Hace referencia al alto del viewport.

### vmax

Utiliza el valor más grande entre el ancho y el alto del viewport.

### vmin

Utiliza el valor más pequeño entre el ancho y el alto del viewport.

## Como se utilizan

1vw = 1% del ancho del viewport (100vw es el 100% del ancho)

1vh = 1% del alto del viewport (100vh es el 100% del alto)

1vmin = 1% del valor que sea mas pequeño del viewport

1vmax = 1% del valor que sea más grande del viewport

**NOTA**: si utilizas 100vw hay que tener en cuenta que va a generar un scroll horizontal en dispositivos de escritorio ya que hay que tener en cuenta también lo que ocupa el scroll del navegador. Si en vez de vw utilizas 100% no ocurrirá.
