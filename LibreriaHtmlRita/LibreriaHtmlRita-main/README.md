# Proyecto: Aurora's Keys
Es una interfaz web d euna libreria fictica usando un diseño anteriormente hecho con Figma.
Consta de: 
- Página principal
- Página de compra online

## Tecnologías usadas
- HTML5
Uso de etiquetas semánticas como:

<header>, <nav>, <main>, <section>, <article>, <aside>, <footer>

- CSS3

Flexbox para alineaciones internas (cabecera, botones, cards)

Grid Layout para estructuras principales (productos, footer)

Pseudoclases (:hover, :active) para interacción visual

- Font Awesome (CDN)

Para los iconos de redes sociales, sin necesidad de descargar imágenes adicionales

- IA 
    - ChatGPT ha sido la IA principal, comunicandole lo que queria sobre todo a través de imagenes
    - En Visual Studio Code cuento con las extensiones de Copilot, Windsurf y Gemini. 

## Estrutura el proyecto: 
/
├── index.html        → Página principal
├── tienda.html       → Página de compra online
├── styles.css        → Hoja de estilos
└── img/              → Imágenes (logo, portadas de libros, decoraciones)

## Desarollo de la página
### Cabecera (Header + Nav)
- Logo y nombre de la libreria alineados a la izquierda
- Buscador centrado mediante Grid de tres columnas
- Icono de usuario alineado a la derecha
- Menú de navegación común a todas las páginas

- Problema encontrado: Al aumentar el tamaño del logo, la altura del header crecía de forma no deseada. Para solucionarlo se fijo la altura del header y se centraron elementos.

### Quienes somos? 
- Titulo centrado
- Imagen con fondo morado
- Texto alineado a la derecha con fondo blanco, y usando <strong> para destacar partes del texto

### Que ofrecemos? 
- Fondo morado en toda la seccion
- Texto introductorio
- Lista de productos con scroll horizontal
- Tarjetas de tamaño fijo

- Problema encontrado: las tarjetas se estiraban por lo que se limitó el ancho. 

### Busca tu librería más cercana
- Imagen de un mapa
- Lista de tiendas en la tarjeta
- Cada tiene tiene un enlace a la URL de Google Maps con esa direccion que te lleva dandole clicl encima

### Footer
- Estructura de tres columnas usando grid
- Logo decorativo a la izquierda
- Texto legal y redes sociales centradas
- Imagen decorativa a la derecha

## Página de compra (tienda.html)

### Navegación entre páginas
Se usa un enlace normal de href

### Estructura princial: 
Siguiendo lo indicado en la práctica en la columna de la izquierda para las categorias y las checkboxes ocupa un 25% mientras que el grid de productos ocupa un 75%

### Tarjeta de producto
Cada producto tiene un <article> que se reutiliza con la información. 

### Etiqueta Oferta
- Se implementa en los productos necesarios
- Se usa la clase <span> porque no aporta contenido (es más bien decorativo)
- Banda diagonal como en el modelo

### Interacción visual de botones 
- Cambian de color con :hoover

#### Buenas prácticas aplicadas
- HTML semántico
- Cards para reutilizar
- Separar HTML y CSS
- Clases claras
- En el CSS hay comentarios indicando a que Primary/Secondary corresponde cada color usando el codigo exacto proporcionado por canva