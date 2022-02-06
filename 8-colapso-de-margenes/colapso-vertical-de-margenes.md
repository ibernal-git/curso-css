# Colapso vertical de márgenes

En CSS ocurre un problema cuando intentamos aplicar un margen vertical a elementos contiguos. Ocurre que si aplicamos un **margin-bottom** a uno de ellos y un **margin-top** al otro, los márgenes van a colapsar y no veremos la suma de ambos márgenes.

Se recomienda entonces aplicar solamente un margin-bottom e ir empujando elementos hacia abajo sin utilizar el margin-top.

El colapso de márgenes también ocurre de padres a hijos. Por ejemplo si tenemos un contenedor y dentro de el un h1, En cuanto añadimos el título (por defecto tiene un márgen) vemos como este colapsa y sobrepasa el límite de su contenedor

**Se puede ver el ejemplo en el [index.html](../index.html)**

Para evitar este comportamiento podemos usar varios **hacks** de CSS sobre el contenedor.

```css
/* Podemos usar overflow */
.box {
  overflow: hidden;
}
/* Podemos usar padding */
.box {
  padding-top: 0.1px;
}
/* Podemos usar un border */
.box {
  border-top: 0.1px solid transparent;
}
```
