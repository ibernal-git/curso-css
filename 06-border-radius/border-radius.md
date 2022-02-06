# Border Radius

Es la propiedad que nos permite redondear vertices de forma independiente. Es un **shorthand** que engloba 4 propiedades:

- border-top-left-radius -> Radio del borde superior izquierdo
- border-top-right-radius -> Radio del borde superior derecho
- border-bottom-right-radius -> Radio del borde inferior derecho
- border-bottom-left-radius -> Radio del borde inferior izquierdo

Si solo recibe un valor dibujará un círculo en cada vértice del radio que especifiquemos.

```css
.box {
  border-radius: 50px; /* Círculo con 50px de radio */
}
```

Si damos un valor a border-radius a todas las esquinas se redondearan con un circulo de radio del valor dado, si damos dos valores, el primer valor se aplica a la esquina superior izquierda y a la esquina inferior derecha, el segundo valor aplica a la esquina superior derecha y a la esquina inferior derecha.

```css
.box {
  border-radius: 50px 100px;
}
```

Si damos 3 valores el primer valor será para la esquina superior izquierda, el segundo para la esuina superior derecha y el tercer valor para la esquina inferior derecha. La esquina inferior izquierda, al no tener un valor adoptará el valor dado a su esquina contraria, la esquina superior derecha.

```css
.box {
  border-radius: 50px 100px 150px;
}
```

Si utilizamos el border-radius como **shorthand** hay diferencias entre si queremos dar un valor a cada lado (círculo) o dos (elipse).

Ejemplo con una esquina

```css
.box {
  border-top-right-radius: 50px 100px; /* Elipse con 50px en el radio X y 100px en el radio Y */
}
```

Ejemplo con el shorthand

```css
.box {
  border-radius: 50px / 100px; /* Elipse con 50px en el radio X y 100px en el radio Y  para todas las esquinas*/
}
.box-2 {
  border-radius: 50px 100px / 100px 150px;

  /*
    Los primeros valores corresponden con el eje X y los segundos con el Y.
    Aquí formamos 2 elipses en esquinas opuestas
  */
}
.box-3 {
  border-radius: 50px 100px 150px / 100px 150px 200px; /* 3 elipses y la elipse de la esquina inferiror izquierda es igual a la superiror derecha */
}
.box-3 {
  border-radius: 50px 100px 150px 200px / 100px 150px 200px 250px; /* 4 elipses */
}
```
