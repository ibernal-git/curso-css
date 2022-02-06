# REM VS EM

## REM

Corresponde a la medida de la "m" de la raíz del documento (html).

Normalmente los navegadores tienen como medida base de la fuente 16px. Entonce 1 rem = 16px, 2 rem = 32px, ...

Para fuentes usar siempre rem en vez de em.

## EM

Corresponde a la medida de la "m" del contexto donde se encuentra.

Por ejemplo si tenemos un contenedor con un font-size diferente, los valores de em se calculan en base a ese font-size.

Ejemplo: font-size: 10px; 1 rem = 10px, 2 rem = 20px, ...

## Ejemplo de utilización

Si tenemos un botón, enlace, contenedor y queremos que el espacio sea proporcional debemos usar em

```css
/*

Tenemos un padding y un border radius con medidas absolutas

*/

.box {
  padding: 16px 32px;
  border-radius: 8px;
  font-size: 1rem;
}
```

Con estas medias absolutas si modificamos el tamaño de fuente veremos que el padding y el border radius no crecen de manera proporcional si aumentamos el tamaño de letra. Ese espacio se veria más pequeño que cuando teníamos un tamaño de letra pequeño.

```css
.box {
  padding: 16px 32px;
  border-radius: 8px;
  font-size: 4rem;
}
```

Lo mismo ocurre si utilizamos rem en esas propiedades.

```css
.box {
  padding: 1rem 2rem;
  border-radius: 0.5rem;
  font-size: 4rem;
}
```

Para que el espacio crezca de manera proporcional tenemos que usar em.

```css
.box {
  padding: 1em 2em;
  border-radius: 0.5em;
  font-size: 4rem;
}
```

De esta manera si modificamos el font-size el espacio aumentará o disminuirá de manera proporcional a ese tamaño.

```css
.box {
  padding: 1em 2em;
  border-radius: 0.5em;
  font-size: 1rem;
}
```
