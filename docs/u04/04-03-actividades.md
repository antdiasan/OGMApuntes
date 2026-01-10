# Ejercicios: la propiedad display

En este apartado se proponen ejercicios prácticos para comprender mejor el funcionamiento de la propiedad **`display`** y cómo afecta al comportamiento de los elementos dentro del flujo del documento.

Los ejercicios deben realizarse de forma progresiva, observando siempre el resultado en el navegador.

---

## Ejercicio 1: comportamiento por defecto

Crea un archivo HTML con el siguiente contenido:

```html
<div>Caja 1</div>
<div>Caja 2</div>
<span>Texto 1</span>
<span>Texto 2</span>
```

No apliques ningún estilo CSS.

Observa el resultado en el navegador y responde:

- ¿Cómo se colocan los elementos `<div>`?
- ¿Cómo se colocan los elementos `<span>`?
- ¿Qué diferencias observas entre ambos tipos de elementos?

---

## Ejercicio 2: display inline

Partiendo del siguiente HTML:

```html
<div class="caja">Caja 1</div>
<div class="caja">Caja 2</div>
<div class="caja">Caja 3</div>
```

Aplica este CSS:

```css
.caja {
  display: inline;
  border: 2px solid blue;
  padding: 10px;
  width: 150px;
  height: 60px;
}
```

Observa el resultado y responde:

- ¿Se colocan las cajas en la misma línea?
- ¿Se respetan las propiedades `width` y `height`?
- ¿De qué depende ahora el tamaño de cada caja?

---

## Ejercicio 3: display block

Usa el mismo HTML del ejercicio anterior y aplica ahora este CSS:

```css
.caja {
  display: block;
  border: 2px solid blue;
  padding: 10px;
  width: 150px;
  height: 60px;
}
```

Observa el resultado y responde:

- ¿Cada caja empieza en una nueva línea?
- ¿Se respetan el ancho y el alto?
- ¿Qué diferencia principal observas respecto al ejercicio anterior?

---

## Ejercicio 4: display inline-block

Manteniendo el mismo HTML, aplica el siguiente CSS:

```css
.caja {
  display: inline-block;
  border: 2px solid blue;
  padding: 10px;
  width: 150px;
  height: 60px;
}
```

Observa el resultado y responde:

- ¿Se colocan las cajas en línea?
- ¿Se respetan ahora el ancho y el alto?
- ¿En qué se diferencia este comportamiento de `inline` y de `block`?

---

## Ejercicio 5: display none

Añade una cuarta caja al HTML:

```html
<div class="caja">Caja 4</div>
```

Y aplica este CSS únicamente a esa caja:

```css
.caja {
  display: block;
}

.caja:nth-child(4) {
  display: none;
}
```

Observa el resultado y responde:

- ¿Se muestra la cuarta caja?
- ¿Ocupa espacio en la página?
- ¿Qué ocurre con el resto de cajas?

---

## Ejercicio 6: reflexión final

Explica con tus propias palabras:

- Para qué sirve la propiedad `display`.
- Qué diferencias hay entre `inline`, `block` e `inline-block`.
- En qué casos utilizarías `display: none`.
