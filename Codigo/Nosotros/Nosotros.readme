# 📘 Sitio Web - Sección "Nosotros" - Explicación del Código

Este documento proporciona una explicación detallada del código **HTML**, **CSS** y **JavaScript** utilizado para construir la página **\"Nosotros\"** del sitio web de **TechBox**.

---

## 🗂️ `Nosotros.html` - Estructura HTML

El archivo `Nosotros.html` define la estructura de la sección "Nosotros".

### 🔤 Etiquetas HTML clave y su función:

- `<!DOCTYPE html>`: Indica que el documento está escrito en HTML5.
- `<html lang="es">`: Elemento raíz que especifica que el contenido está en español.
- `<head>`: Contiene metadatos del sitio.
  - `<meta charset="UTF-8">`: Usa codificación UTF-8 para caracteres.
  - `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Hace que el sitio sea responsive.
  - `<title>Nosotros</title>`: Define el título de la pestaña del navegador.
  - `<link rel="stylesheet" href="Nosotros.css">`: Enlaza a la hoja de estilos.
- `<body>`: Contiene el contenido visible de la página.
  - `<header>`: Cabecera del sitio.
    - `<nav class="dropdown-menu">`: Menú desplegable con enlaces a otras secciones.
    - `.header-content`: Contenedor del logo y título "Nosotros".
      - `.logo-nosotros`: Imagen del logotipo.
      - `.section-title`: Título principal de la sección.
  - `.carrusel-wrapper`: Contenedor general del carrusel de miembros.
    - `<button class="flecha izquierda">❮</button>` y `<button class="flecha derecha">❯</button>`: Botones para mover el carrusel.
    - `.equipo-container`: Carrusel horizontal que contiene las tarjetas.
      - `.miembro`: Cada tarjeta de integrante del equipo.
        - `<img>`: Imagen del miembro.
        - `<h4>`: Nombre.
        - `<p>`: Rol o cargo.
- `<script>`: Código JavaScript para controlar el movimiento del carrusel.

---

## 🎨 `Nosotros.css` - Estilos CSS

El archivo `Nosotros.css` define la apariencia visual de la sección "Nosotros".

### 🎛️ Reglas CSS destacadas:

- `*`: Resetea márgenes, paddings y define fuente general.
- `body`: Fondo oscuro, texto blanco y sin desbordamiento horizontal.
- `header`: Fondo azul (color corporativo).

### 📂 Menú desplegable:

- `.dropdown-menu`: Posiciona el menú en la parte superior.
- `.menu-toggle`: Estilo del botón del menú (color, tamaño, hover).
- `.dropdown-content`: Contenedor de los enlaces, aparece al enfocar o pasar el mouse.

### 🧱 Cabecera principal:

- `.header-content`: Centra el logo y el título, con fondo azul más claro y borde redondeado.
- `.logo-nosotros`: Tamaño ajustado del logo.
- `.section-title`: Título grande, blanco, centrado.

### 🖼️ Carrusel:

- `.carrusel-wrapper`: Contenedor del carrusel con posición relativa.
- `.equipo-container`: Carrusel horizontal con scroll automático y diseño tipo "snap".
- `.miembro`: Tarjetas de los integrantes:
  - Fondo oscuro, bordes redondeados y sombra.
  - Escala al hacer hover.
  - Imagen en blanco y negro que se colorea al pasar el mouse.
- `.flecha`: Botones de navegación del carrusel (izquierda/derecha).
  - Están sobre el carrusel, centrados verticalmente, con fondo semitransparente.

---

## ⚙️ JavaScript embebido (`<script>` dentro de `Nosotros.html`)

```js
function moverCarrusel(direccion) {
    if (isTransitioning) return;
    isTransitioning = true;

    carrusel.scrollBy({ left: tarjetaAncho * direccion, behavior: "smooth" });

    setTimeout(() => {
        const scrollPos = carrusel.scrollLeft;
        const maxScroll = tarjetaAncho * (tarjetasOriginales.length - 1);

        if (scrollPos <= 0) {
            carrusel.scrollLeft = maxScroll;
        } else if (scrollPos >= maxScroll) {
            carrusel.scrollLeft = 0;
        }

        isTransitioning = false;
    }, 300);
}
