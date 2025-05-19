# Sitio Web de TechBox - Explicación del Código

Este documento proporciona una explicación detallada del código HTML y CSS utilizado para crear el sitio web de TechBox.

## `index.html` - Estructura HTML

El archivo `index.html` define la estructura y el contenido de la página web.

### Etiquetas HTML Clave y sus Funciones:

* **`<!DOCTYPE html>`**: Declara el documento como HTML5.
* **`<html>`**: El elemento raíz de la página; `lang="es"` especifica el español como idioma.
* **`<head>`**: Contiene metadatos (información sobre el documento).
    * **`<meta charset="UTF-8">`**: Establece la codificación de caracteres a UTF-8.
    * **`<meta name="viewport" content="width=device-width, initial-scale=1.0">`**: Configura la ventana gráfica para la respuesta adaptable.
    * **`<title>TechBox</title>`**: Establece el título que se muestra en la pestaña del navegador.
    * **`<link rel="icon" href="Logo-TechoBox.ico">`**: Enlaza al favicon.
    * **`<link rel="stylesheet" href="index.css">`**: Enlaza a la hoja de estilos CSS.
* **`<body>`**: Contiene el contenido visible de la página.
    * **`<div class="video-background">`**: Contenedor para el video de fondo.
        * **`<video autoplay muted loop playsinline>`**: Inserta el video con reproducción automática, silencio, bucle y reproducción en línea.
            * **`<source src="/Archivos/Video de WhatsApp 2025-04-06 a las 16.31.04_fd6b582e.mp4" type="video/mp4">`**: Especifica la fuente del video.
    * **`<header>`**: La sección de la cabecera, que contiene el logotipo y la navegación.
        * **`<a href="#" class="logo-link">`**: Enlace para el logotipo.
            * **`<img src="/Archivos/Logo-TechoBox.png" alt="Logo de TechBox" class="logo-fixed">`**: Muestra la imagen del logotipo.
        * **`<div class="servicios-header">`**: Contenedor para los enlaces de servicios.
            * **`<span class="servicio">Instalación</span>`**, **`<span class="servicio">Reparación</span>`**, **`<span class="servicio">Mantenimiento</span>`**: Enlaces de servicios.
    * **`<section>`**: Secciones para el contenido principal.
        * **`<h2 id="servicios">¿Qué ofrecemos?</h2>`**: Encabezado de la sección (con un ID para posible enlace).
        * **`<ul>`**: Lista no ordenada para mostrar los servicios.
            * **`<li>`**: Elementos de la lista.
                * **`<strong>...</strong>`**: Resalta los títulos de los servicios/productos.
    * **`<section>`**: Otra sección de contenido para los productos.
        * **`<h2 id="productos">Productos que ofrecemos</h2>`**: Encabezado de la sección para productos.
        * **`<ul>`**: Lista no ordenada para mostrar los productos.
            * **`<li>`**: Elementos de la lista.
                * **`<strong>...</strong>`**: Resalta los títulos de los productos.
    * **`<button class="boton-contacto">`**: Botón de contacto.
        * **`<a href="/Contacto/contacto.html">Contáctanos</a>`**: Enlace dentro del botón.
    * **`<button class="boton-mvv">`**: Botón de Misión, Visión y Valores.
        * **`<a href="/Mvv/MVV.html">Misión, Visión y Valores</a>`**: Enlace dentro del botón.

## `index.css` - Estilos CSS

El archivo `index.css` define la presentación visual de los elementos HTML.

### Conceptos Clave y Reglas CSS:

* **`:root { ... }`**: Define variables CSS (propiedades personalizadas) para estilos reutilizables.
    * `--primary-color: #1a73e8;`: Color primario.
    * `--background-color: #f0f4f8;`: Color de fondo.
    * `--text-color: #333;`: Color del texto.
* **`* { ... }`**: Selector universal; aplica estilos a todos los elementos.
    * `margin: 0; padding: 0;`: Restablece los márgenes y el relleno predeterminados.
    * `box-sizing: border-box;`: Incluye el relleno y el borde en el ancho/alto total del elemento.
    * `font-family: system-ui, sans-serif;`: Establece la fuente predeterminada.
* **`body { ... }`**: Estilos para el elemento `<body>`.
    * `background: var(--background-color);`: Utiliza la variable de color de fondo.
    * `color: var(--text-color);`: Utiliza la variable de color de texto.
    * `line-height: 1.6;`: Establece el espaciado entre líneas.
* **`header { ... }`**: Estilos para el elemento `<header>`.
    * `background: var(--primary-color);`: Utiliza la variable de color primario.
    * `color: #fff;`: Establece el color del texto en blanco.
    * `padding: 5vh 5vw;`: Agrega relleno (relativo a la altura/ancho de la ventana gráfica).
    * `text-align: center;`: Centra el texto.
    * `display: flex; flex-direction: column; align-items: center;`: Utiliza Flexbox para el diseño.
* **`.servicios-header { ... }`**: Estilos para el contenedor de la cabecera de servicios.
    * `display: flex; justify-content: center; gap: 10vw; margin-top: 5vh; margin-left: 4vw;`: Utiliza Flexbox para centrar los elementos y agregar espaciado.
* **`.servicio { ... }`**: Estilos para elementos de servicio individuales.
    * `background: rgba(255, 255, 255, 0.1);`: Fondo blanco transparente.
    * `padding: 1vh 2vw;`: Agrega relleno.
    * `border-radius: 8px;`: Redondea las esquinas.
    * `font-size: 2vw; font-weight: 500;`: Establece el tamaño y el grosor de la fuente.
* **`.logo-link { ... }`**: Estilos para el enlace del logotipo (utilizando Flexbox para centrar).
* **`.logo-fixed { ... }`**: Estilos para la imagen del logotipo.
    * `max-width: 15vw; height: auto;`: Establece el ancho máximo y la altura automática.
* **`header p { ... }`**: Estilos para los párrafos dentro de la cabecera.
* **`section { ... }`**: Estilos para los elementos `<section>`.
* **`h2 { ... }`**: Estilos para los encabezados `<h2>`.
* **`ul { ... }`**: Estilos para listas no ordenadas (utilizando Grid Layout).
* **`li { ... }`**: Estilos para los elementos de la lista.
    * `background: #fff;`: Fondo blanco.
    * `padding: 2vh;`: Agrega relleno.
    * `border-radius: 1vh;`: Redondea las esquinas.
    * `box-shadow: 0 0.4vh 1.2vh rgba(0, 0, 0, 0.05);`: Agrega una sombra sutil.
    * `transition: 0.3s ease;`: Efecto de transición suave.
* **`li:hover { ... }`**: Estilos para los elementos de la lista al pasar el cursor.
    * `transform: translateY(-0.5vh);`: Mueve el elemento ligeramente hacia arriba.
    * `box-shadow: 0 0.6vh 1.6vh rgba(0, 0, 0, 0.1);`: Aumenta la sombra.
* **`li strong { ... }`**: Estilos para los elementos `<strong>` dentro de los elementos de la lista.
* **`a { ... }`**: Estilos para los enlaces.
    * `text-decoration: none; color: white;`: Elimina el subrayado y establece el color del texto en blanco.
* **`.video-background { ... }`**: Estilos para el contenedor del fondo de video (posicionamiento fijo).
* **`.video-background video { ... }`**: Estilos para el video.
    * `width: 100vw; height: 100vh; object-fit: cover; opacity: 0.9;`: Cubre toda la ventana gráfica, escala el video y establece la opacidad.
* **`.boton-contacto { ... }`** y **`.boton-mvv { ... }`**: Estilos para los botones (estilos similares para los botones de contacto y MVV).

### Fundamentos de CSS:

* **Selectores**: Seleccionan elementos HTML (por ejemplo, `body`, `h2`, `.clase`, `#id`).
* **Propiedades y Valores**: Definen los estilos (por ejemplo, `color: red;`, `font-size: 16px;`).
* **Cascada e Herencia**: Determinan cómo se aplican los estilos cuando hay conflictos.
* **Modelo de Caja**: Describe las cajas rectangulares que representan los elementos HTML (contenido, relleno, borde, margen).
* **Diseño (Layout)**: Técnicas CSS para organizar los elementos (por ejemplo, Flexbox, Grid, posicionamiento).
