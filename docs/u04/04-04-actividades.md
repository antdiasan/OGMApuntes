# Actividades: el modelo de caja (box model)

En este apartado se proponen actividades prácticas para comprender cómo el navegador calcula el tamaño de los elementos y cómo influyen el contenido, el padding, el borde y el margen en la maquetación.

Las actividades están pensadas para **observar, razonar y comprobar resultados en el navegador**.

---

## Actividad 1: identificando las partes de la caja

Crea un archivo HTML con un único elemento `<div>` que contenga texto.

Aplica el siguiente CSS:

```css
.caja {
  width: 200px;
  padding: 20px;
  border: 5px solid black;
  margin: 30px;
}
```

Responde:

- ¿Qué parte corresponde al contenido?
- ¿Dónde se encuentra el padding?
- ¿Qué función tiene el borde?
- ¿El margen forma parte del tamaño de la caja?

---

## Actividad 2: calculando el tamaño real

Utilizando el mismo CSS de la actividad anterior, calcula **sin usar el navegador**:

- la anchura total de la caja
- el espacio horizontal total que ocupa respecto a otros elementos

Después, comprueba el resultado usando las herramientas de desarrollador del navegador.

---

## Actividad 3: varias cajas en horizontal

Crea tres cajas con el siguiente estilo:

```css
.caja {
  width: 150px;
  padding: 10px;
  border: 2px solid blue;
  margin: 10px;
  display: inline-block;
}
```

Coloca las tres cajas dentro de un contenedor.

Responde:

- ¿Cuánto espacio horizontal ocupa cada caja?
- ¿Cuántas cajas caben en una fila de 1000px?
- ¿Qué propiedades influyen en ese cálculo?

---

## Actividad 4: el papel del margen

Modifica únicamente el valor del margen en la actividad anterior.

Prueba distintos valores y observa:

- cómo cambia la separación entre las cajas
- si cambia o no el tamaño de cada caja
- cómo afecta al número de cajas que caben en una fila

Explica por qué ocurre esto.

---

## Actividad 5: reflexión final

Explica con tus propias palabras:

- qué es el modelo de caja
- por qué el margen no forma parte del tamaño del elemento
- por qué es importante entender el box model para maquetar correctamente
