# Portfolio — Ana Carolina Luján

Sitio web personal que funciona como CV online y portfolio de proyectos.

Construido con HTML, Tailwind CSS y Flowbite. No requiere instalación ni servidor — es un único archivo que abrís en cualquier navegador.

---

## Cómo usar este repositorio

La página completa está en `index.html`. Podés abrirlo directamente en tu navegador para verlo, o subir el archivo a GitHub Pages para publicarlo online.

Para publicar en GitHub Pages:
1. Subí `index.html` a tu repositorio
2. Andá a Settings → Pages
3. Elegí la rama `main` y carpeta raíz
4. En unos minutos el sitio queda en vivo

---

## Cómo editar el contenido

Todo está en `index.html`. El archivo tiene comentarios que explican cada sección.

**Cambiar textos**
Buscá el texto que querés editar directamente en el archivo. Los títulos, descripciones y datos de contacto están escritos en HTML plano, fácil de encontrar y modificar.

**Cambiar colores**
Al inicio del archivo hay una sección `:root { }` con variables CSS. Ahí están todos los colores del sitio agrupados. Cambiando esos valores se actualiza toda la página.

**Agregar un proyecto**
En la sección `id="proyectos"` hay tres bloques con la clase `project-card`. Copiás uno, lo pegás abajo y editás el título, descripción, tecnologías y links.

**Agregar una certificación**
En la sección `id="certificaciones"` hay bloques con la clase `cert-item`. Mismo proceso: copiás uno y editás los datos.

**Agregar tu foto**
Guardá tu foto como `assets/images/foto-perfil.jpg` (preferentemente cuadrada). Luego en `index.html` buscá el emoji 🌸 dentro del hero y reemplazalo con:
```html
<img src="assets/images/foto-perfil.jpg" alt="Ana Carolina Luján" />
```

**Agregar CV descargable**
Guardá tu CV como `docs/cv-ana-lujan.pdf`. Después buscá los botones del hero y agregá:
```html
<a href="docs/cv-ana-lujan.pdf" download class="btn-secondary">Descargar CV</a>
```

---

## Estructura

```
/
├── index.html          — la página completa
├── README.md           — este archivo
├── assets/
│   └── images/         — fotos e imágenes
└── docs/               — CV en PDF u otros documentos
```

---

## Formulario de contacto

Los mensajes del formulario llegan a `annacarolinalujan@gmail.com` a través de Formspree. Si en algún momento querés cambiar el email receptor, creá un nuevo formulario en formspree.io y reemplazá el ID en esta línea de `index.html`:

```html
<form id="contact-form" action="https://formspree.io/f/xlgzybjz"
```

---

## Tecnologías

- HTML5 y CSS3
- Tailwind CSS (via CDN)
- Flowbite (componentes interactivos, via CDN)
- Formspree (formulario de contacto)
- Google Fonts — Fraunces + Inter
- GitHub Pages (hosting)

---

Ana Carolina Luján · annacarolinalujan@gmail.com
