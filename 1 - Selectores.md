# SELECTORES CSS

- ## Selectores simples

  - ### Selectores elementales

    - #### Selector Universal \* (selecciona todos los elementos)

    - #### Selector de tipo o etiqueta -> Nombre de etiqueta

  - ### Selectores de atributo

    - #### id -> id del elemento

    - #### clase -> Clase del elemento

    - #### Otros atributos

      ```css

      [atributo] /* [href] */

      [atributo=valor]  /* [href="https://google.es"] */

      [atributo^=valor] /* [href^="color"] para seleccionar los que empiezan con color */

      [atributo*=valor] /* igual que el de antes pero la coincidencia se realiza en cualquier lado no solo si empieza con ese valor */

      [atributo$=valor] /* si termina con ese valor */

      [atributo|=valor] /* Se usa para lang="en" ya que funciona con en- */

      ```

---

- ## Selectores Compuestos

  - ### Selectores Agrupados
    ```css
    .text,
    text-2,
    text-3,
    text-4 {
    }
    ```
  - ### Selectores Combinadores

    - #### Selector de hijo directo
      ```css
      .container > p;
      ```
    - #### Selector descendiente

      ```css
      div p
      .text-2 strong
      div .tittle-2
      ```

      Es decir hay que poner un espacio entre los diferentes atributos.
      Por norma general es recomendable como máximo 2 elementos.

    - #### Selector de hermano siguiente

      Sirve para seleccionar elementos del mismo nivel

      ```css
      .text-2 + h2 div + p #titulo + span;
      ```

      También se puede seleccionar todos los hermanos siguientes con ~.

      ```css
      .text-2 ~ p;
      ```

  - ### Pseudoclases - Pseudoelementos

# EJEMPLOS CON SELECTORES

```css
/* Selectores elementales */

* {
  background-color: lightcoral;
}
h1 {
  background-color: lightcyan;
}
p {
  background-color: lightgreen;
}

/* Selectores de atributo */

#title {
  background-color: lightgreen;
}
.firstP {
  background-color: lightsalmon;
}
```
