# ¿Cómo funciona CSS?

## Especifidad

La especifidad establece cómo de específico es un selector para saber que estilo aplicar.

El cálculo se realiza siguiendo la siguiente fórmula:

- ### Etiquetas y pseudoelementos -> 0,0,1
- ### Clases, atributos y pseudoclases -> 0,1,0
- ### Ids -> 1,0,1
- ### Estilos en línea -> 1,0,0,0
- ### !important -> GANA A TODO Y NO SE USA NUNCA

## Cascada

La cascada funciona siempre que la especifidad sobre el elemento se la misma.

## Herencia

Hay propiedades que heredan los hijos, por ejemplo las propiedades color, font-size, ...

Los enlaces no heredan pero podemos forzar la herencia con el siguiente valor en las propiedades:

```css
inherit

/* Por ejemplo */

.link {
  color: inherit;
}
```

Para evitar herencia podemos usar el valor initial.

# Ejemplos de selectores con diferente especifidad

```css
h1 {
  background-color: red;
}

.title {
  background-color: blue;
}

#title {
  background-color: green;
}

h1.title {
  background-color: yellow;
}

h1#title {
  background-color: teal;
}

h1.title#title {
  background-color: tomato;
}
```
