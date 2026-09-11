# La Senda — Sitio Web de Restaurante

Sitio web informativo para un restaurante ficticio llamado **"La Senda"**, desarrollado con **HTML5 y CSS3** puros (sin frameworks ni JavaScript). El proyecto presenta la identidad del negocio, su carta dividida por categorías, eventos, opiniones de clientes y un formulario de contacto, todo distribuido en varias páginas enlazadas mediante una barra de navegación común.

## Características

- 🏠 **Página de inicio** con carrusel de imágenes de presentación del restaurante.
- 🍽️ **Carta dividida en tres secciones**: Entrantes, Platos principales y Postres, cada una con su propia página y estilos.
- 👨‍👩‍👧 **Sección "Nosotros"** con la historia y presentación del equipo/familia detrás del restaurante.
- 🎉 **Sección de Eventos**, mostrando actividades y celebraciones especiales.
- ⭐ **Sección de Opiniones** de clientes.
- 📜 **Página de Política** (privacidad/condiciones).
- ✉️ **Página de Contacto**.
- 🗺️ **Sitemap XML** incluido para SEO.
- 🎨 Estilos organizados en un archivo **general.css** (compartido por todas las páginas) más un archivo **CSS específico por cada página**.

## Estructura del proyecto

```
La-Senda-Proyecto-final-JLSP-HTML_CSS/
├── HTML/
│   ├── index.html          # Página de inicio
│   ├── nosotros.html       # Sobre el restaurante
│   ├── entrantes.html      # Carta: entrantes
│   ├── principales.html    # Carta: platos principales
│   ├── postres.html        # Carta: postres
│   ├── eventos.html        # Eventos del restaurante
│   ├── opiniones.html      # Opiniones de clientes
│   ├── contacto.html       # Formulario / datos de contacto
│   └── politica.html       # Política de privacidad
├── CSS/
│   ├── general.css         # Estilos base compartidos (header, footer, tipografías, fondo)
│   ├── index.css
│   ├── nosotros.css
│   ├── entrantes.css
│   ├── principales.css
│   ├── postres.css
│   ├── eventos.css
│   ├── opiniones.css
│   ├── contacto.css
│   └── politica.css
├── img/                     # Todas las imágenes del sitio (fondos, slider, platos, eventos, equipo)
├── XML(Visual)/
│   └── sitemap.xml          # Mapa del sitio para SEO
└── .vscode/
    └── settings.json        # Configuración del puerto para Live Server
```

## Corrección aplicada

⚠️ **Nota importante:** la versión original del proyecto tenía las rutas de los archivos **CSS e imágenes rotas** (los `<link>` y `<img>` apuntaban a los archivos como si estuvieran en la misma carpeta que los `.html`, cuando en realidad estaban organizados en carpetas separadas `CSS/` e `img/`). Esto hacía que el HTML se mostrara sin ningún estilo aplicado.

En esta versión se corrigieron todas las rutas relativas (`../CSS/...` y `../img/...`) en los 9 archivos HTML, se ajustó la ruta de la imagen de fondo dentro de `general.css`, y se renombraron un par de archivos de imagen que tenían espacios en el nombre (para evitar futuros problemas de rutas). El sitio ahora carga sus estilos e imágenes correctamente.

## Tecnologías utilizadas

- **HTML5**
- **CSS3**

## Cómo ejecutar

1. Clona o descarga el repositorio.
2. Abre la carpeta `HTML/` y ejecuta `index.html` en tu navegador (se recomienda usar la extensión **Live Server** de VS Code, ya que el proyecto incluye su configuración de puerto en `.vscode/settings.json`).
3. Navega por el sitio usando el menú superior: Inicio, Carta (Entrantes, Principales, Postres), Nosotros, Eventos, Contacto, Política y Opiniones.

## Posibles mejoras futuras

- Añadir interactividad con JavaScript (por ejemplo, un slider funcional en la página de inicio en lugar de imágenes estáticas).
- Hacer el formulario de contacto funcional (envío real de mensajes).
- Optimizar y estandarizar los formatos de imagen (mezcla actual de `.jpg`, `.jfif`, `.webp`, `.avif`).
- Mejorar la accesibilidad (atributos `alt` en todas las imágenes, etiquetas semánticas).
