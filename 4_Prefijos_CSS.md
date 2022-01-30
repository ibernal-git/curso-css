# Prefijos CSS

Para poder utilizar CSS moderno y añadir prefijos de navegadores de forma automática para las funcionalidades que todavía no forman parte del estandar CSS pero sí que están soportadas en esos navegadores podemos usar diferentes métodos.

Prefijos de los navegadores más comunes:

```css
-moz-
-o-
-webkit-
-ms-
-chrome-
-khtml-
```

Autoprefixer nos permite añadir esos prefijos de forma automática y así evitar que nosotros los tengamos que aprender, implementar y mantener.

El proyecto actual está creado con Vite. Vite soporta de forma nativa PostCSS. PostCSS transformará el código CSS tanto en desarrollo como en la compilación final con las modificaciones de autoprefixer.

Instalamos PostCSS y Autoprefixer:

```
npm install -D -E postcss autoprefixer
```

Creamos el archivo de configuración para que Vite y PostCSS funcionen junto con Autoprefixer.

El archivo tiene que estar en la raíz y se llama

```
postcss.config.js
```

Y en el contenido del archivo temos que añadir el plugin de autoprefixer de la siguiente manera:

```js
module.exports = {
  plugins: [require('autoprefixer')],
}
```

Con esto el CSS se debería procesar de forma automática para añadir los prefijos que Autoprefixer considera en función de la web [Can I Use](https://caniuse.com/).
