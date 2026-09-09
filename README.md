Rincones favoritos de Mia

Nombre y apellido: Celina Daiub

Materia: Diseño y Desarrollo Web

Actividad 1 — Galería Visual

Título de la galería: Rincones favoritos de Mia

Tema elegido: Mi mascota — Mia, mi gata

Breve descripción de la propuesta

Esta galería reúne fotos de mi gata Mia en los distintos rincones de la
casa que eligió como propios: el rascador, su camita redonda, el sillón,
una manta, la ventana del balcón y hasta el teclado de la notebook. Cada
rincón tiene su propia página con una o más fotos y una breve descripción
de por qué es un lugar especial para ella.

Objetivo de la galería

Mostrar, a través de fotos reales, la personalidad de Mia y su forma de
"apropiarse" de distintos espacios de la casa según el momento del día,
la luz o las ganas de estar cerca de alguien. La idea es que cualquiera
que entre a la página pueda conocer un poco a Mia y sonreír viendo sus
rincones favoritos.

Descripción de los contenidos

La galería está organizada en una página principal (`index.html`), una
barra de navegación presente en todas las páginas, y una página por cada
rincón:

`rascador.html` — el rascador junto a la pared roja del living.
`camita.html` — su camita redonda de peluche.
`sofa.html` — el sillón bordó donde duerme panza arriba.
`manta.html` — la manta turquesa donde se esconde para dormir.
`ventana.html` — la camita junto a la ventana del balcón.
`escritorio.html` — el teclado de la notebook, su lugar "de trabajo".

Desde la página principal se puede acceder a cada uno de estos rincones
mediante la barra de navegación o las tarjetas de la grilla, y desde
cada rincón se puede volver fácilmente al inicio con el mismo menú o el
botón "Volver a la página principal".

---

Decisiones de diseño

Colores

La paleta se tomó directamente de las fotos de Mia, para que el sitio se
sienta parte de la misma historia:

- Bordó/ladrillo (`#a8434c`), tomado de la alfombra del rascador y del
  sillón donde duerme. Se usa en el encabezado, los títulos y los
  enlaces al pasar el mouse.
- Bordó oscuro (`#7f333a`), para la barra de navegación.
- Turquesa (`#1f7480`), de la manta donde se esconde a dormir. Se usa en
  los enlaces y en los botones "Ver más".
- Marrón atigrado (`#6b5642`), inspirado en el color de su pelaje. Se
  usa en el pie de página.
- Crema (`#f6efe2`) como fondo general, para que las fotos sean siempre
  las protagonistas.

Tipografías

-Trebuchet MS (con `Verdana` como alternativa), para los títulos
  (`h1`, `h2`, `h3`): es una tipografía de sistema con formas más
  redondeadas y amigables que Arial, sin necesidad de importar nada
  externo.
-Arial (con `Helvetica` como alternativa), para el texto del
  cuerpo, la navegación y las descripciones: una tipografía de sistema
  simple y muy legible, pensada para que el contenido se lea cómodo sin
  competir con las fotos.

Ambas son fuentes del sistema operativo (no se importan desde
servicios externos como Google Fonts), así que el sitio no depende de
conexión a internet para mostrarlas correctamente.

Por qué estas elecciones

Al ser una galería sobre una gata de casa, buscamos colores cálidos y
reales (sacados de su propio entorno, no genéricos) y una tipografía
amigable pero legible. Se mantuvo un diseño simple, sin sombras ni
animaciones, para que el foco esté siempre en las fotos y en el
contenido de cada rincón.

Layout y responsive

- La grilla de rincones de la página principal usa **CSS Grid**
  (`repeat(auto-fit, minmax(...))`) para acomodar automáticamente las
  tarjetas según el ancho de pantalla.
- Las galerías de fotos de cada rincón y la barra de navegación usan
  **Flexbox**, para que los elementos se acomoden y envuelvan en
  pantallas chicas.
- Se trabajó con unidades relativas (`rem`, `%` y `em`) en vez de valores
  fijos en píxeles: `rem` para tamaños de texto y espaciados generales
  (relativos al documento), y `em` puntualmente en detalles como el
  espaciado entre letras de los títulos o el padding horizontal de los
  botones (relativos al tamaño de fuente de ese elemento en particular).
- Se agregaron **media queries** en dos puntos de corte (768px y 480px)
  para adaptar el tamaño de los títulos, el espaciado y la cantidad de
  columnas de la grilla en tablets y celulares.

Estructura del proyecto

```
mia-galeria/
│
├── index.html
├── rascador.html
├── camita.html
├── sofa.html
├── manta.html
├── ventana.html
├── escritorio.html
├── README.md
│
├── css/
│   └── style.css
│
└── img/
    ├── rascador-1.jpg
    ├── rascador-2.jpg
    ├── camita-1.jpg
    ├── camita-2.jpg
    ├── sofa-1.jpg
    ├── manta-1.jpg
    ├── ventana-1.jpg
    └── escritorio-1.jpg
```
