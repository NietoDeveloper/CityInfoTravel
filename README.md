# App Travel Info en JavaScript

Link para ver resultado: [VENTA VIAJES FINALIZADO](https://nietodeveloper.github.io/CityInfoTravel/)

Este es un tutorial que te guiará a o JavaScas y sus precios asocs.

## Requisitos previo
1.  Clona oarga l

Clone the repository:git clone <https://github.com/NietoDeveloper/CityInfoTravel>

## Funcionamiento del código JavaScript
ando se hace clic en un enlace de ciudad.

### Importación de datos de las ciudadté disponible en el repositorio junto con el código JavaScript.


-   `subTituloElemento
-   `parrafoElemento`: el ea ciudad seleccionada.io de la ciudad seleccionada.

### Agregar evento CLICK a los enlaces

Se agrega un evento `click` a cada ció

-   Remueve la clase `active` de todos los enlaces utilizando otro bucle `forEach`.
-   Agrega la clase `active` al enlace actual (`this`).
-   Obtiene el contenido correspondiente a la ciudad seleccionada utilizando la función `obtenerContenido` y el texto del enlace actual.
-   Actualiza los elementos del DOM con la información de la ciudad seleccionada.

### Función para obtener contenido de la ciudad

La función `obtenerContenido` toma el texto del enlace como parámetro y devuelve el contenido correspondiente de la ciudad desde el archivo `ciudades.js`. Utiliza un objeto `contenido` para mapear el texto del enlace con el contenido de la ciudad.

## Personalización del contenido

Puedes personalizar el contenido de las ciudades modificando el archivo `ciudades.js`. Cada ciudad es representada por un objeto con propiedades como `titulo`, `subtitulo`, `parrafo` y `precio`.

