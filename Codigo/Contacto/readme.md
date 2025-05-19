# Formulario de Contacto - Explicación del Código

Este documento explica el código HTML y CSS utilizado para crear el formulario de contacto.

## `contacto.html` - Estructura HTML

Este archivo define la estructura del formulario de contacto.

### Etiquetas HTML Clave y sus Funciones:

* **`<!DOCTYPE html>`**: Declara el documento como HTML5.
* **`<html>`**: El elemento raíz de la página; `lang="es"` especifica el español.
* **`<head>`**: Contiene metadatos.
    * **`<meta charset="UTF-8">`**: Establece la codificación de caracteres a UTF-8.
    * **`<meta name="viewport" content="width=device-width, initial-scale=1.0">`**: Configura la ventana gráfica para la respuesta adaptable.
    * **`<title>Contacto | TechBox</title>`**: Establece el título de la página.
    * **`<link rel="stylesheet" href="contacto.css">`**: Enlaza la hoja de estilos CSS.
* **`<body>`**: Contiene el contenido visible de la página.
    * **`<main class="contacto-container">`**: El elemento `<main>` representa el contenido principal, y la clase `contacto-container` se usa para estilos.
        * **`<h1>Contacto</h1>`**: El encabezado principal del formulario.
        * **`<form class="formulario-contacto">`**: El elemento `<form>` define el formulario, y la clase `formulario-contacto` se usa para estilos.
            * **`<label for="nombre">Nombre</label>`**: Etiqueta para el campo de entrada del nombre. `for` lo asocia con el `id` "nombre".
            * **`<input type="text" id="nombre" name="nombre" required>`**: Campo de entrada de texto para el nombre.
                * `type="text"`: Especifica que es un campo de texto.
                * `id="nombre"`: Un identificador único para el campo.
                * `name="nombre"`: El nombre del campo (para enviar datos).
                * `required`: Indica que el campo es obligatorio.
            * **`<label for="apellido">Apellido</label>`**: Etiqueta para el campo de entrada del apellido.
            * **`<input type="text" id="apellido" name="apellido" required>`**: Campo de entrada de texto para el apellido.
            * **`<label for="email">Correo electrónico</label>`**: Etiqueta para el campo de entrada del correo electrónico.
            * **`<input type="email" id="email" name="email" required>`**: Campo de entrada de correo electrónico. `type="email"` valida el formato básico.
            * **`<label for="mensaje">Mensaje</label>`**: Etiqueta para el área de texto del mensaje.
            * **`<textarea id="mensaje" name="mensaje" rows="5" required></textarea>`**: Área de texto para escribir el mensaje. `rows="5"` define las filas iniciales.
            * **`<button type="submit">Enviar mensaje</button>`**: Botón para enviar el formulario. `type="submit"` lo define como botón de envío.

## `contacto.css` - Estilos CSS

Este archivo define la apariencia del formulario.

* **`body { ... }`**: Estilos para el elemento `<body>`.
    * `background: #066fd8;`: Color de fondo de la página.
    * `font-family: system-ui, sans-serif;`: Fuente.
    * `margin: 0; padding: 0;`: Márgenes y relleno a cero.
* **`.contacto-container { ... }`**: Estilos para el contenedor principal (`<main>`).
    * `max-width: 600px;`: Ancho máximo del contenedor.
    * `margin: 5vh auto; margin-top: 6.5%;`: Centrado vertical y horizontal.
    * `padding: 4vh 4vw;`: Relleno dentro del contenedor.
    * `background: white;`: Fondo blanco del contenedor.
    * `border-radius: 1vh;`: Esquinas redondeadas.
    * `box-shadow: 0 0.5vh 2vh rgba(0, 0, 0, 0.1);`: Sombra suave.
* **`.contacto-container h1 { ... }`**: Estilos para el encabezado `<h1>`.
    * `text-align: center;`: Texto centrado.
    * `margin-bottom: 3vh;`: Margen inferior.
    * `color: #1a73e8;`: Color del texto.
* **`.formulario-contacto { ... }`**: Estilos para el formulario (`<form>`).
    * `display: flex; flex-direction: column; gap: 2vh;`: Flexbox para organizar los elementos en columna.
* **`.formulario-contacto label { ... }`**: Estilos para las etiquetas (`<label>`).
    * `font-weight: 600;`: Texto en negrita.
* **`.formulario-contacto input, .formulario-contacto textarea { ... }`**: Estilos para los campos de entrada y el área de texto.
    * `padding: 1vh 1vw;`: Relleno.
    * `font-size: 1rem;`: Tamaño de la fuente.
    * `border: 1px solid #ccc;`: Borde gris.
    * `border-radius: 0.5vh;`: Esquinas redondeadas.
    * `resize: vertical;`: Permite redimensionar verticalmente el área de texto.
* **`.formulario-contacto button { ... }`**: Estilos para el botón de envío (`<button>`).
    * `padding: 1.5vh 2vw;`: Relleno del botón.
    * `background: #1a73e8;`: Color de fondo.
    * `color: white;`: Color del texto.
    * `border: none;`: Sin borde.
    * `font-weight: bold;`: Texto en negrita.
    * `border-radius: 1vh;`: Esquinas redondeadas.
    * `cursor: pointer;`: Cursor como mano al pasar por encima.
    * `transition: background 0.3s;`: Transición suave del color de fondo.
* **`.formulario-contacto button:hover { ... }`**: Estilos para el botón al pasar el cursor.
    * `background: #155ab6;`: Color de fondo más oscuro al pasar el cursor.
