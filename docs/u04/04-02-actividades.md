# Ejercicios: el flujo de los elementos en el navegador

En este apartado se proponen una serie de ejercicios prácticos para afianzar el concepto de **flujo normal del documento** y comprender cómo el navegador coloca los elementos HTML por defecto.

Los ejercicios deben realizarse **sin utilizar técnicas de maquetación avanzadas** como Flexbox o Grid, salvo que se indique lo contrario.

---

## Ejercicio 1: observando el flujo normal

Crea un archivo HTML sencillo que contenga los siguientes elementos, en este orden:

- Un encabezado `<h1>`
- Dos párrafos `<p>`
- Un `<div>` con texto

No apliques ningún estilo CSS.

Observa en el navegador cómo se colocan los elementos y responde:

- ¿En qué orden aparecen?
- ¿Empiezan todos en una nueva línea?
- ¿Alguno se coloca junto a otro?

---

## Ejercicio 2: elementos en bloque y en línea

Partiendo del siguiente código HTML:

```html
<p>
  Este es un <span>texto en línea</span> dentro de un párrafo.
</p>
```

Responde:

- ¿El elemento `<span>` empieza en una nueva línea?
- ¿Ocupa toda la anchura disponible?
- ¿Por qué se comporta de forma distinta al párrafo?

---

## Ejercicio 3: cambiando el flujo con display

Utiliza el siguiente HTML:

```html
<div class="caja">Caja 1</div>
<div class="caja">Caja 2</div>
<div class="caja">Caja 3</div>
```

Aplica los siguientes estilos CSS, uno cada vez, y observa el resultado:

```css
.caja {
  display: block;
}
```

```css
.caja {
  display: inline;
}
```

```css
.caja {
  display: inline-block;
}
```

Describe qué ocurre en cada caso y explica qué ha cambiado respecto al flujo normal.

---

## Ejercicio 4: el orden del HTML

Cambia el orden de las cajas en el HTML del ejercicio anterior.

Por ejemplo:

```html
<div class="caja">Caja 3</div>
<div class="caja">Caja 1</div>
<div class="caja">Caja 2</div>
```

Responde:

- ¿Cambia la posición visual de las cajas?
- ¿Qué relación existe entre el orden del HTML y el flujo del documento?

---

## Ejercicio 5: reflexión final

Explica con tus propias palabras:

- Qué es el flujo normal del documento.
- Por qué es importante entenderlo antes de maquetar una página web.
- Qué ocurre cuando se modifica el flujo mediante CSS.

No es necesario escribir código en este ejercicio, solo razonar las respuestas.
