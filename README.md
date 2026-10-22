# Portafolio personal

Sitio web de portafolio personal construido con HTML5 semántico y CSS moderno, con diseño responsivo, accesible y validado con los estándares del W3C.

## Objetivo

Presentar mi perfil académico y profesional en una página clara y fácil de navegar, aplicando principios de usabilidad, accesibilidad y validación de estándares web. El sitio contiene tres secciones:

1. **Acerca de mí:** foto, datos personales, presentación y habilidades.
2. **Certificaciones y cursos:** tres certificaciones completadas y una en proceso, con imagen del diploma y descripción.
3. **Contacto:** datos de contacto (teléfono, correo, LinkedIn, GitHub y ubicación).

## Tecnologías

| Tecnología | Uso |
|---|---|
| HTML5 semántico | Estructura con `header`, `nav`, `main`, `section`, `article`, `figure`, `address` y `footer` |
| CSS3 | Variables personalizadas, Flexbox, CSS Grid, `clamp()`, `aspect-ratio`, media queries |
| GitHub Pages | Publicación del sitio |

No se usan frameworks, librerías externas ni JavaScript.

## Estructura del proyecto

```
portafolio/
├── index.html
├── README.md
├── css/
│   └── styles.css
└── img/
    ├── foto-placeholder.svg
    └── diploma-placeholder.svg
```

## Diseño responsivo

Enfoque *mobile-first* con dos puntos de quiebre:

- **≥ 768px (`48rem`):** el perfil pasa a dos columnas, las certificaciones a una cuadrícula de 2×2, el contenido de contacto se limita a un ancho cómodo de lectura y el encabezado queda fijo.
- **≥ 1024px (`64rem`):** se amplía la foto de perfil y el título del sitio.

## Accesibilidad

- Idioma declarado (`lang="es"`) y enlace para saltar al contenido principal.
- Jerarquía de encabezados: un `h1`, `h2` por sección y `h3` dentro de cada tarjeta.
- Texto alternativo descriptivo en todas las imágenes.
- Enlaces externos que avisan con texto oculto que se abren en una pestaña nueva.
- Navegación con `nav` etiquetado, foco visible con teclado y áreas táctiles de al menos 44 px.
- Contraste de color suficiente y estado de las certificaciones indicado con texto, no solo con color.
- Respeto a `prefers-reduced-motion`.

## Cómo personalizar

1. Abre `index.html` y busca los textos entre corchetes `[...]` y los comentarios `RELLENAR`.
2. Coloca tus imágenes en `img/` (por ejemplo `mi-foto.jpg`, `diploma-1.jpg`) y cambia los atributos `src` y `alt`.
3. Actualiza los enlaces de contacto (`tel:`, `mailto:`, LinkedIn, GitHub).
4. En cada certificación, ajusta el atributo `datetime` de `<time>` con formato `AAAA-MM`.

## Validación

- **HTML:** [validator.w3.org](https://validator.w3.org/) (por URL, subida de archivo o entrada directa).
- **CSS:** [jigsaw.w3.org/css-validator](https://jigsaw.w3.org/css-validator/) (perfil CSS nivel 3).
- **Accesibilidad:** pestaña *Lighthouse* de Chrome DevTools.

## Prueba en vista móvil

1. Abre el sitio en Chrome y presiona `F12`.
2. Activa el modo dispositivo (`Ctrl + Shift + M`) y prueba con 375 px (móvil) y 768 px (tablet).
3. Verifica que no haya desplazamiento horizontal, que el menú sea legible y que los datos de contacto se vean completos.
4. Una vez publicado, abre la URL en tu teléfono real.

## Publicación en GitHub Pages

1. Crea una cuenta en [github.com](https://github.com) si aún no tienes una.
2. Crea un repositorio nuevo público, por ejemplo `portafolio` (o `tu-usuario.github.io` para obtener la URL más corta).
3. Sube los archivos con el botón **Add file → Upload files** (arrastra `index.html`, `README.md` y las carpetas `css` e `img`) y confirma con **Commit changes**. El archivo `index.html` debe quedar en la raíz del repositorio.
4. Ve a **Settings → Pages**.
5. En **Build and deployment**, elige **Source: Deploy from a branch**, selecciona la rama `main` y la carpeta `/ (root)`, y guarda.
6. Espera uno o dos minutos. El sitio quedará disponible en `https://tu-usuario.github.io/portafolio/`.
7. Cada vez que hagas un cambio en el repositorio, el sitio se actualiza automáticamente.

**Alternativa:** [Netlify Drop](https://app.netlify.com/drop) permite arrastrar la carpeta del proyecto y obtener una URL pública en segundos, sin usar Git.

## Autor

[Tu nombre] — [Tu carrera], [Tu universidad]
