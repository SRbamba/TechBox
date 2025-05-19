Primero: index.html (HTML Structure)

El archivo HTML define la estructura y el contenido de tu página web.  Aquí tienes una explicación de las etiquetas más importantes:

<!DOCTYPE html>: Indica al navegador que este es un documento HTML5, la versión más reciente de HTML.
<html>: La etiqueta raíz que envuelve todo el contenido de la página. lang="es" especifica que el idioma principal del documento es español.
<head>: Contiene metadatos sobre el documento, información que no se muestra directamente al usuario, pero es importante para el navegador, los motores de búsqueda, etc.
<meta charset="UTF-8">: Especifica la codificación de caracteres como UTF-8, que soporta una amplia variedad de caracteres de diferentes idiomas.
<meta name="viewport" content="width=device-width, initial-scale=1.0">: Configura el viewport para que la página se adapte bien a diferentes tamaños de pantalla (dispositivos móviles, tabletas, etc.). width=device-width hace que el ancho de la página coincida con el ancho del dispositivo, y initial-scale=1.0 establece el zoom inicial en 1.
<title>TechBox</title>: Define el título que se muestra en la pestaña del navegador.
<link rel="icon" href="Logo-TechoBox.ico">: Enlaza un icono (favicon) que se muestra en la pestaña del navegador.
<link rel="stylesheet" href="index.css">: Enlaza el archivo CSS (index.css) para aplicar estilos a la página.
<body>: Contiene el contenido visible de la página web.
<div class="video-background">: Un contenedor para el video de fondo. La clase video-background se utiliza en el CSS para aplicar estilos específicos.
<video autoplay muted loop playsinline>: La etiqueta <video> inserta un video en la página.
autoplay: El video comienza a reproducirse automáticamente.
muted: El video se reproduce sin sonido.
loop: El video se repite continuamente.
playsinline: Permite que el video se reproduzca dentro de la página en dispositivos móviles en lugar de abrirse en pantalla completa.
<source src="/Archivos/Video de WhatsApp 2025-04-06 a las 16.31.04_fd6b582e.mp4" type="video/mp4">: Especifica la ruta al archivo de video y su tipo.
<header>: La sección de la cabecera de la página, típicamente contiene el logo y la navegación principal.
<a href="#" class="logo-link">: Un enlace (ancla) que en este caso parece que vuelve a la misma página (el "#" significa la parte superior de la página). La clase logo-link se usa para aplicar estilos.
<img src="/Archivos/Logo-TechoBox.png" alt="Logo de TechBox" class="logo-fixed">: Inserta la imagen del logo. alt proporciona un texto alternativo para la imagen si no se puede cargar (importante para accesibilidad y SEO). logo-fixed es una clase para aplicar estilos al logo.
<div class="servicios-header">: Un contenedor para los enlaces de servicios.
<span class="servicio">Instalación</span>, <span class="servicio">Reparación</span>, <span class="servicio">Mantenimiento</span>: Elementos <span> que representan los diferentes servicios. La clase servicio se usa para darles estilo.
<section>: Define secciones de contenido temáticamente agrupadas.
<h2 id="servicios">¿Qué ofrecemos?</h2>: Un encabezado de segundo nivel. id="servicios" crea un identificador único para este elemento, lo que permite enlazar directamente a esta sección desde otras partes de la página (aunque no se usa en este código).
<ul>: Una lista no ordenada.
<li>: Elementos de la lista.
<strong>...</strong>: Texto en negrita, usado aquí para resaltar los títulos de los servicios/productos.
<button class="boton-contacto">: Un botón. La clase boton-contacto se utiliza para darle estilo.
<a href="/Contacto/contacto.html">Contáctanos</a>: Un enlace dentro del botón.
<button class="boton-mvv">: Otro botón.
<a href="/Mvv/MVV.html">Misión, Visión y Valores</a>: Enlace dentro del botón.
Segundo: index.css (CSS Styling)

El archivo CSS define cómo se ve el contenido HTML.  Funciona aplicando reglas a los selectores.

:root { ... }: Define variables CSS (custom properties) que se pueden reutilizar en todo el archivo. Esto hace que sea más fácil mantener y modificar los colores y otros estilos.
--primary-color: #1a73e8;: Define el color primario.
--background-color: #f0f4f8;: Define el color de fondo general.
--text-color: #333;: Define el color del texto principal.
* { ... }: El selector * aplica los estilos a todos los elementos de la página.
margin: 0; padding: 0;: Elimina los márgenes y el relleno predeterminados de los elementos.
box-sizing: border-box;: Cambia el modelo de caja para que el padding y el border se incluyan dentro del ancho y alto de un elemento, lo que facilita el diseño.
font-family: system-ui, sans-serif;: Establece la fuente del texto.
body { ... }: Estilos específicos para el elemento <body>.
background: var(--background-color);: Usa la variable para el color de fondo.
color: var(--text-color);: Usa la variable para el color del texto.
line-height: 1.6;: Establece el espaciado entre líneas.
header { ... }: Estilos para la cabecera.
background: var(--primary-color);: Color de fondo usando la variable.
color: #fff;: Color del texto (blanco).
padding: 5vh 5vw;: Relleno vertical y horizontal (el uso de vh y vw hace que el relleno sea relativo al tamaño de la ventana, lo que ayuda a la adaptabilidad).
text-align: center;: Alinea el texto al centro.
display: flex; flex-direction: column; align-items: center;: Usa Flexbox para organizar los elementos dentro de la cabecera.
.servicios-header { ... }: Estilos para el contenedor de los servicios en la cabecera.
display: flex; justify-content: center; gap: 10vw; margin-top: 5vh; margin-left: 4vw;: Usa Flexbox para centrar los elementos y crear espacio entre ellos.
.servicio { ... }: Estilos para cada elemento de servicio.
background: rgba(255, 255, 255, 0.1);: Fondo blanco con transparencia.
padding: 1vh 2vw;: Relleno.
border-radius: 8px;: Esquinas redondeadas.
font-size: 2vw; font-weight: 500;: Tamaño y grosor de la fuente.
.logo-link { ... }: Estilos para el enlace del logo (usa Flexbox para centrar).
.logo-fixed { ... }: Estilos para la imagen del logo.
max-width: 15vw; height: auto;: Ajusta el tamaño del logo.
header p { ... }: Estilos para los párrafos dentro de la cabecera.
section { ... }: Estilos para las secciones principales de contenido.
h2 { ... }: Estilos para los encabezados de segundo nivel.
ul { ... }: Estilos para las listas no ordenadas (usa Grid Layout para crear una disposición de columnas adaptable).
li { ... }: Estilos para los elementos de la lista.
background: #fff;: Fondo blanco.
padding: 2vh;: Relleno.
border-radius: 1vh;: Esquinas redondeadas.
box-shadow: 0 0.4vh 1.2vh rgba(0, 0, 0, 0.05);: Sombra suave.
transition: 0.3s ease;: Animación suave para las propiedades que cambian.
li:hover { ... }: Estilos para cuando el cursor pasa por encima de un elemento de la lista (efecto "hover").
transform: translateY(-0.5vh);: Mueve el elemento ligeramente hacia arriba.
box-shadow: 0 0.6vh 1.6vh rgba(0, 0, 0, 0.1);: Sombra más pronunciada.
li strong { ... }: Estilos para los elementos <strong> dentro de los <li>.
a { ... }: Estilos para los enlaces.
text-decoration: none; color: white;: Elimina el subrayado y establece el color del texto en blanco.
.video-background { ... }: Estilos para el contenedor del video de fondo (lo posiciona como fondo fijo).
.video-background video { ... }: Estilos para el video.
width: 100vw; height: 100vh; object-fit: cover; opacity: 0.9;: Hace que el video cubra toda la ventana, ajusta la forma en que se escala y establece la opacidad.
.boton-contacto { ... } y .boton-mvv { ... }: Estilos para los botones (muy similares, con un degradado de fondo, bordes redondeados, sombra y efectos de hover)
