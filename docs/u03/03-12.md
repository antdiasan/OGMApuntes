# Actividad guiada: Pseudoselectores en CSS

En esta actividad guiada vas a **practicar los pseudoselectores** vistos en el apartado anterior.

Trabajarás siempre sobre el mismo archivo HTML y **añadirás las reglas CSS poco a poco**, comprobando el resultado en el navegador.

!!! note "Objetivo"
    Comprender cómo y cuándo se aplican los pseudoselectores según el estado, la posición o la interacción del usuario.

---

## Material de partida

Dispones de un archivo con extensión `.txt` que contiene el código HTML base.

1. Descarga el archivo: [actividad-guiada-pseudoselectores.txt](actividad-guiada-pseudoselectores.txt){: target="_blank" }
2. Cópialo y guárdalo como:  `actividad-guiada-pseudoselectores.html`
3. Crea un archivo CSS llamado: `pseudoselectores.css`
4. Enlaza el archivo CSS desde el HTML.

!!! warning "Importante"
    No modifiques el HTML salvo que se indique expresamente.  
    Todo el trabajo se realiza desde el archivo CSS.

---

## Paso 1: Pseudoselector `:hover`

### Objetivo
Cambiar el color de fondo de los enlaces cuando el ratón pase por encima.

### Inténtalo tú
Aplica un color de fondo diferente a los enlaces cuando el usuario pase el ratón.

### Solución
```css
a:hover {
  background-color: #e0e0e0;
}
```

---

## Paso 2: Pseudoselector `:active`

### Objetivo
Cambiar el color del texto del enlace mientras se hace clic.

### Solución
```css
a:active {
  color: red;
}
```

---

## Paso 3: Pseudoselector `:focus`

### Objetivo
Resaltar los campos de formulario cuando reciben el foco.

### Solución
```css
input:focus {
  border: 2px solid blue;
}
```

---

## Paso 4: Pseudoselectores `:link` y `:visited`

### Objetivo
Diferenciar visualmente los enlaces visitados de los no visitados.

### Solución
```css
a:link {
  color: blue;
}

a:visited {
  color: purple;
}
```

!!! note "Recuerda"
    El orden correcto es: `:link`, `:visited`, `:hover`, `:active`.

---

## Paso 5: Pseudoselectores de posición `:first-child` y `:last-child`

### Objetivo
Aplicar estilos al primer y último elemento de una lista.

### Solución
```css
li:first-child {
  font-weight: bold;
}

li:last-child {
  font-style: italic;
}
```

---

## Paso 6: `:nth-child()`

### Objetivo
Colorear elementos concretos de una lista.

### Solución
```css
li:nth-child(2) {
  background-color: #f0f0f0;
}
```

---

## Paso 7: `:nth-child(odd)` y `:nth-child(even)`

### Objetivo
Crear un efecto de filas alternas.

### Solución
```css
li:nth-child(odd) {
  background-color: #fafafa;
}

li:nth-child(even) {
  background-color: #eaeaea;
}
```

---

## Paso 8: Pseudoselector `:not()`

### Objetivo
Aplicar estilos a todos los botones excepto uno concreto.

### Solución
```css
button:not(.cancelar) {
  border: 2px solid green;
}
```

---

## Paso 9: Pseudoselector `:empty`

### Objetivo
Ocultar elementos que no tengan contenido.

### Solución
```css
p:empty {
  display: none;
}
```

---

## Paso 10: Introducción a pseudoelementos

### Objetivo
Aplicar estilos a partes concretas del texto.

### Solución
```css
p::first-line {
  font-weight: bold;
}

p::first-letter {
  font-size: 1.5em;
}
```

---

## Paso 11: `::before` y `::after`

### Objetivo
Añadir contenido decorativo antes y después de un elemento.

### Solución
```css
.etiqueta::before {
  content: "★ ";
}

.etiqueta::after {
  content: " ✔";
}
```

!!! warning "Recuerda"
    Los pseudoelementos `::before` y `::after` necesitan siempre la propiedad `content`.

---

## Finalización de la actividad

Si has llegado hasta aquí, has practicado:

- Pseudoselectores de estado
- Pseudoselectores de posición
- `:not()` y `:empty`
- Introducción a pseudoelementos

!!! note "Autoevaluación"
    Comprueba que entiendes **por qué se aplica cada estilo** y no solo el resultado visual.
