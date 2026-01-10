# Actividad guiada: selectores individuales

En esta actividad vas a practicar **los selectores individuales de CSS** utilizando un documento HTML ya preparado.

El objetivo es que **aprendas a seleccionar elementos concretos** y apliques estilos sencillos, centrándote únicamente en **un selector cada vez**.

!!! note "Objetivo de la actividad"
    Comprender y utilizar correctamente los **selectores individuales** más importantes de CSS.

---

## Archivos de trabajo

Descarga el archivo con el código HTML base:

- [actividad-guiada-selectores-individuales.txt](./actividades/actividad-guiada-selectores-individuales.txt){: target="_blank" }


Antes de empezar:

1. Crea el fichero `actividad-guiada-selectores-individuales.html`.
2. Copia el contenido del fichero .txt en el .html.
3. Abre el archivo HTML en el navegador.
4. Abre la carpeta del ejercicio en Visual Studio Code.
5. Crea el archivo `actividad-guiada-selectores-individuales.css` en la misma carpeta que el HTML.


---

## Paso 1: selector de elemento

### Qué se quiere conseguir
Cambiar el color del texto de **todos los párrafos** de la página.

✏️ Intenta escribir tú la regla CSS antes de mirar la solución.

### Solución

??? success "Solución (haz clic para mostrar)"
    ```css
      p {
      color: blue;
    }
    ```

---

## Paso 2: selector de clase

### Qué se quiere conseguir
Añadir un borde y un relleno a **todas las cajas**.

✏️ Utiliza un selector de clase.

### Solución

??? success "Solución (haz clic para mostrar)"
    ```css
    .caja {
      border: 2px solid black;
      padding: 10px;
      margin-bottom: 15px;
    }
    ```

---

## Paso 3: selector de identificador (id)

### Qué se quiere conseguir
Cambiar el color del título de la **caja destacada**.

✏️ Utiliza un selector de identificador.

### Solución

??? success "Solución (haz clic para mostrar)"
    ```css
    #titulo-destacado {
      color: darkred;
    }
    ```

---

## Paso 4: selector universal (`*`)

### Qué se quiere conseguir
Hacer que todas las cajas de la página calculen su tamaño de la misma forma.

✏️ Utiliza el selector universal.

### Solución

??? success "Solución (haz clic para mostrar)"
    ```css
    * {
      box-sizing: border-box;
    }
    ```

!!! warning "Uso con precaución"
    El selector universal afecta a todos los elementos de la página.

---

## Paso 5: selector de atributo

### Qué se quiere conseguir
Cambiar el borde únicamente del **campo de texto** del formulario.

✏️ Utiliza un selector de atributo.

### Solución

??? success "Solución (haz clic para mostrar)"
    ```css
    input[type="text"] {
      border: 2px solid green;
    }
    ```

---

## Comprobación final

Comprueba que:

- Todos los párrafos han cambiado de color.
- Las cajas tienen borde y separación interior.
- El título destacado tiene un color diferente.
- Solo el campo de texto del formulario tiene el borde verde.

---

## Reflexión final

Responde brevemente:

- ¿Qué selector te ha resultado más sencillo?
- ¿Cuál te ha costado más entender?
- ¿Para qué usarías una clase en lugar de un id?

!!! note "Conclusión"
    Esta actividad te permite practicar los selectores individuales de forma progresiva y controlada.
