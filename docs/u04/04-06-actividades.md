# Actividades: posicionamiento básico en CSS

En estas actividades se trabajará el uso de la propiedad `position` y sus valores principales.
El objetivo es comprender **cómo cambia el comportamiento de un elemento** cuando se modifica su posicionamiento.

En todas las actividades, observa el resultado en el navegador antes de consultar la solución.

---

## Actividad 1: position static

Crea una página HTML con dos cajas (`div`) una debajo de otra.
Intenta mover la segunda caja usando las propiedades `top` y `left`.

Responde:

  - ¿Se mueve la caja?
  - ¿Por qué ocurre esto?

??? success "Solución (haz clic para mostrar)"
    ```css
    .caja {
      position: static;
      top: 20px;
      left: 20px;
    }
    ```

    Un elemento con `position: static` no responde a las propiedades `top`, `left`, `right` ni `bottom`.
    Sigue siempre el flujo normal del documento y no puede desplazarse manualmente.

---

## Actividad 2: position relative

Partiendo del mismo HTML anterior, aplica `position: relative` a la segunda caja y desplázala.

Responde:

  - ¿Desde dónde se mueve la caja?
  - ¿Afecta al resto de elementos?

??? success "Solución (haz clic para mostrar)"
    ```css
    .caja {
      position: relative;
      top: 20px;
      left: 30px;
    }
    ```

    El elemento se desplaza **respecto a su posición original**.
    Aunque se mueva visualmente, el espacio original sigue reservado y el resto de elementos no cambia su posición.

---

## Actividad 3: position absolute

Crea un contenedor con una caja en su interior.
Aplica `position: absolute` a la caja y colócala en la esquina superior derecha.

Responde:

  - ¿Sigue ocupando espacio en el flujo?
  - ¿Respecto a qué elemento se posiciona?

??? success "Solución (haz clic para mostrar)"
    ```css
    .contenedor {
      position: relative;
    }

    .caja {
      position: absolute;
      top: 0;
      right: 0;
    }
    ```

    El elemento con `position: absolute` sale del flujo normal.
    Se posiciona respecto al contenedor más cercano que tenga `position` distinta de `static`.

---

## Actividad 4: position fixed

Crea una caja que permanezca visible en la esquina inferior derecha de la pantalla aunque se haga scroll.

Responde:

  - ¿Se mueve la caja al desplazarse la página?
  - ¿Respecto a qué se posiciona?

??? success "Solución (haz clic para mostrar)"
    ```css
    .caja {
      position: fixed;
      bottom: 20px;
      right: 20px;
    }
    ```

    Un elemento con `position: fixed` se posiciona respecto a la ventana del navegador.
    No se desplaza al hacer scroll.

---

## Actividad 5: comparación de comportamientos

Compara `relative`, `absolute` y `fixed` respondiendo:

- ¿Qué valores salen del flujo?
- ¿Cuál mantiene su espacio reservado?
- ¿Cuál se fija a la ventana del navegador?

Reflexiona sobre en qué casos utilizarías cada uno.
