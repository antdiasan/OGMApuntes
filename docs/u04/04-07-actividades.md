# Actividades: maquetación con inline-block y columnas

En estas actividades se practicará la creación de **columnas utilizando `display: inline-block`**, analizando sus ventajas y, sobre todo, sus limitaciones.

Antes de consultar las soluciones, es importante **probar, observar y razonar el resultado en el navegador**.

---

## Actividad 1: columnas básicas con inline-block

Crea una página HTML con tres cajas alineadas horizontalmente usando `display: inline-block`.

Cada caja debe ocupar aproximadamente un tercio del ancho disponible.

Responde:

- ¿Se colocan las tres cajas en la misma fila?
- ¿Qué propiedad permite que no bajen de línea?

??? success "Solución (haz clic para mostrar)"
    ```html
    <div class="columna">Columna 1</div>
    <div class="columna">Columna 2</div>
    <div class="columna">Columna 3</div>
    ```

    ```css
    .columna {
      display: inline-block;
      width: 30%;
      padding: 10px;
      border: 1px solid black;
    }
    ```

    Las cajas se colocan en la misma fila gracias al uso de `display: inline-block`, que permite que los elementos se comporten como contenido en línea sin perder su tamaño.

---

## Actividad 2: el problema de los espacios

Utilizando el mismo código anterior, observa el espacio que aparece entre las columnas.

Responde:

- ¿A qué se deben esos espacios?
- ¿Qué ocurre si se aumenta ligeramente el ancho de las columnas?

??? success "Solución (haz clic para mostrar)"
    Los espacios aparecen porque el navegador interpreta los saltos de línea y espacios del HTML como espacios reales, ya que los elementos `inline-block` se tratan como contenido en línea.

    Si el ancho total supera el 100%, alguna de las columnas baja a la siguiente línea.

---

## Actividad 3: alineación vertical

Modifica el CSS de las columnas para que todas se alineen por la parte superior.

Responde:

- ¿Qué propiedad CSS se utiliza?
- ¿Por qué es necesaria en este caso?

??? success "Solución (haz clic para mostrar)"
    ```css
    .columna {
      display: inline-block;
      width: 30%;
      vertical-align: top;
    }
    ```

    La propiedad `vertical-align` permite controlar la alineación vertical de los elementos `inline-block`, que por defecto se alinean según la línea base del texto.

---

## Actividad 4: ajuste del ancho

Cambia el ancho de las columnas para intentar que siempre entren tres en la misma fila, incluso teniendo en cuenta los espacios.

Responde:

- ¿Es necesario reducir el ancho?
- ¿Por qué no se puede usar el 33% exacto?

??? success "Solución (haz clic para mostrar)"
    ```css
    .columna {
      display: inline-block;
      width: 32%;
      vertical-align: top;
    }
    ```

    Es necesario reducir el ancho porque los espacios entre elementos también ocupan ancho. Usar exactamente el 33% suele provocar que una columna no quepa.

---

## Actividad 5: reflexión final

Reflexiona y explica con tus propias palabras:

- Qué problemas presenta `inline-block` para maquetar columnas.
- Por qué esta técnica no es la más adecuada para layouts modernos.
- Qué tipo de herramienta crees que puede solucionar estos problemas.
