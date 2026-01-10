# Actividades: introducción a Flexbox para maquetación

En estas actividades se trabajarán los conceptos básicos de **Flexbox** aplicados a la maquetación.
El objetivo es comprobar cómo Flexbox resuelve de forma sencilla problemas que antes requerían soluciones complejas.

Antes de desplegar las soluciones, prueba cada ejercicio y observa el resultado en el navegador.

---

## Actividad 1: activar Flexbox

Crea un contenedor con tres cajas en su interior.
Aplica Flexbox al contenedor para que las cajas se coloquen automáticamente en una fila.

Responde:

- ¿Qué propiedad activa el modo Flexbox?
- ¿Cómo se colocan los elementos hijos al activarlo?

??? success "Solución (haz clic para mostrar)"
    ```css
    .contenedor {
      display: flex;
    }
    ```

    Al aplicar `display: flex` al contenedor, sus elementos hijos pasan a colocarse en una fila de forma automática, siguiendo el eje principal.

---

## Actividad 2: cambio de dirección

Partiendo del ejercicio anterior, modifica la dirección para que las cajas se coloquen en columna.

Responde:

- ¿Qué propiedad permite cambiar la dirección?
- ¿Qué ocurre con el eje principal?

??? success "Solución (haz clic para mostrar)"
    ```css
    .contenedor {
      display: flex;
      flex-direction: column;
    }
    ```

    Al usar `flex-direction: column`, el eje principal pasa a ser vertical y los elementos se colocan uno debajo de otro.

---

## Actividad 3: centrado horizontal con Flexbox

Utiliza Flexbox para centrar horizontalmente las cajas dentro del contenedor.

Responde:

- ¿Qué propiedad se utiliza?
- ¿Sobre qué eje actúa?

??? success "Solución (haz clic para mostrar)"
    ```css
    .contenedor {
      display: flex;
      justify-content: center;
    }
    ```

    La propiedad `justify-content` alinea los elementos a lo largo del eje principal.

---

## Actividad 4: centrado vertical con Flexbox

Centra verticalmente las cajas dentro del contenedor utilizando Flexbox.

Responde:

- ¿Qué propiedad se utiliza?
- ¿Por qué este centrado no era sencillo sin Flexbox?

??? success "Solución (haz clic para mostrar)"
    ```css
    .contenedor {
      display: flex;
      align-items: center;
    }
    ```

    `align-items` permite alinear los elementos en el eje secundario, facilitando el centrado vertical.

---

## Actividad 5: centrado completo

Consigue que las cajas queden centradas tanto en horizontal como en vertical dentro del contenedor.

Responde:

- ¿Qué combinación de propiedades se necesita?
- ¿Qué ventaja presenta esta solución frente a técnicas anteriores?

??? success "Solución (haz clic para mostrar)"
    ```css
    .contenedor {
      display: flex;
      justify-content: center;
      align-items: center;
    }
    ```

    Flexbox permite centrar elementos de forma clara y directa, sin cálculos ni soluciones alternativas.

---

## Actividad 6: reflexión final

Reflexiona y explica con tus propias palabras:

- Qué problemas de maquetación soluciona Flexbox.
- Por qué Flexbox resulta más sencillo que técnicas como `inline-block`.
- En qué situaciones utilizarías Flexbox para crear un layout.
