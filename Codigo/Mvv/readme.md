# Página de Misión, Visión y Valores - Explicación del Código

Este documento describe el código HTML y CSS para la página de Misión, Visión y Valores.

## `MVV.html` - Estructura HTML

Este archivo define la estructura y el contenido de la página.

### Etiquetas HTML Clave y sus Funciones:

* **`<!DOCTYPE html>`**: Declara el documento como HTML5.
* **`<html>`**: El elemento raíz de la página; `lang="es"` indica que el idioma es español.
* **`<head>`**: Contiene metadatos.
    * **`<meta charset="UTF-8">`**: Establece la codificación de caracteres a UTF-8.
    * **`<meta name="viewport" content="width=device-width, initial-scale=1.0">`**: Configura la ventana gráfica para la respuesta adaptable.
    * **`<title>Misión, Visión y Valores</title>`**: Establece el título de la página.
    * **`<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Montserrat:wght@400;600&display=swap" rel="stylesheet">`**:  Importa fuentes de Google Fonts (Poppins y Montserrat).
    * **`<link rel="stylesheet" href="mvv.css">`**: Enlaza la hoja de estilos CSS (`mvv.css`).
* **`<body>`**: Contiene el contenido visible de la página.
    * **`<header>`**: La cabecera de la página.
        * **`<img src="/Archivos/Logo-TechoBox.png" alt="Logo Techbox">`**: Muestra el logotipo. `alt` proporciona texto alternativo para accesibilidad.
        * **`<h1>Misión, Visión y Valores</h1>`**: El título principal de la página.
    * **`<div class="container">`**: Un contenedor para el contenido principal.
        * **`<div class="section">`**:  Una sección para la Misión.
            * **`<h2>Misión</h2>`**: Encabezado de la sección.
            * **`<p>...</p>`**: Párrafo que describe la misión.
        * **`<div class="section">`**:  Una sección para la Visión.
            * **`<h2>Visión</h2>`**: Encabezado de la sección.
            * **`<p>...</p>`**: Párrafo que describe la visión.
        * **`<div class="section">`**:  Una sección para los Valores.
            * **`<h2>Valores</h2>`**: Encabezado de la sección.
            * **`<ul>`**: Lista no ordenada de los valores.
                * **`<li>...</li>`**: Elementos de la lista, cada uno representando un valor.

## `mvv.css` - Estilos CSS

Este archivo define la apariencia de la página de Misión, Visión y Valores.

* **`body { ... }`**: Estilos para el elemento `<body>`.
    * `margin: 0;`:  Elimina los márgenes predeterminados.
    * `background-color: #1c1c1e;`: Establece el color de fondo.
    * `color: #f5f5f7;`: Establece el color del texto.
    * `font-family: 'Poppins', 'Arial', sans-serif;`: Establece la fuente.
    * `font-size: 1.8vh;`: Establece el tamaño de la fuente (relativo a la altura de la ventana gráfica).
* **`header { ... }`**: Estilos para la cabecera (`<header>`).
    * `background-color: #1a73e8;`: Establece el color de fondo de la cabecera.
    * `color: white;`: Establece el color del texto en blanco.
    * `padding: 4vh 0;`: Agrega relleno vertical.
    * `text-align: center;`: Centra el texto horizontalmente.
    * `position: relative;`:  Establece el posicionamiento relativo para permitir el posicionamiento absoluto del logo.
* **`header img { ... }`**: Estilos para la imagen del logo dentro de la cabecera.
    * `position: absolute;`: Posiciona la imagen absolutamente dentro de la cabecera.
    * `top: 1vh; left: 1vw;`: La posiciona en la esquina superior izquierda.
    * `width: 8vw; height: 16vh;`: Establece el ancho y la altura (relativos al ancho y alto de la ventana gráfica).
* **`header h1 { ... }`**: Estilos para el encabezado `<h1>` dentro de la cabecera.
    * `font-family: 'Montserrat', sans-serif;`:  Establece la fuente.
    * `font-size: 4vh;`: Establece el tamaño de la fuente (relativo a la altura de la ventana gráfica).
* **`.container { ... }`**: Estilos para el contenedor principal (`<div class="container">`).
    * `padding: 6vh 4vw;`: Agrega relleno.
    * `max-width: 80vw;`: Establece el ancho máximo.
    * `margin: auto;`: Centra el contenedor horizontalmente.
* **`.section { ... }`**: Estilos para las secciones (`<div class="section">`).
    * `background: #2c2c2e;`: Establece el color de fondo.
    * `margin-bottom: 4vh;`: Agrega margen inferior.
    * `padding: 4vh 3vw;`: Agrega relleno.
    * `border-radius: 2vh;`: Redondea las esquinas.
    * `box-shadow: 0 0.5vh 1vh rgba(0, 0, 0, 0.5);`: Agrega una sombra.
* **`.section h2 { ... }`**: Estilos para los encabezados `<h2>` dentro de las secciones.
    * `color: #a29bfe;`: Establece el color del texto.
    * `font-size: 3vh;`: Establece el tamaño de la fuente.
    * `margin-bottom: 2vh;`: Agrega margen inferior.
* **`p { ... }`**: Estilos para los párrafos (`<p>`).
    * `line-height: 1.6;`: Establece el espaciado entre líneas.
* **`ul { ... }`**: Estilos para las listas no ordenadas (`<ul>`).
    * `list-style: none;`: Elimina los estilos de lista predeterminados (puntos).
    * `padding: 0;`: Elimina el relleno predeterminado.
* **`ul li { ... }`**: Estilos para los elementos de la lista (`<li>`).
    * `margin-bottom: 1.5vh;`: Agrega margen inferior.
    * `font-size: 2vh;`: Establece el tamaño de la fuente.
* **`ul li::before { ... }`**: Estilos para el pseudo-elemento `::before` de los elementos de la lista.  Esto agrega el "🔹" antes de cada elemento.
    * `content: "🔹 ";`:  Inserta el contenido.
    * `color: #a29bfe;`: Establece el color.
    * `font-size: 2.2vh;`: Establece el tamaño de la fuente.

En resumen, `MVV.html` estructura el contenido de la página de Misión, Visión y Valores, mientras que `mvv.css` define su estilo visual, incluyendo colores, fuentes, espaciado y diseño.
