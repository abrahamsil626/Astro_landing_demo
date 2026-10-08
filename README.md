# Astro Landing Demo

Landing page de **portafolio de proyectos web** hecha con Astro y Tailwind CSS: una página estática, rápida y adaptable que presenta una selección de proyectos con su descripción e imagen.

> **Prueba el proyecto en vivo:** [abrahamsil626.github.io/Astro_landing_demo](https://abrahamsil626.github.io/Astro_landing_demo/)

## Funcionalidad

* Interfaz íntegramente **en español**.
* Secciones: Hero, Más información, Características, Acerca de y Proyectos.
* Contenido de proyectos y características cargado desde archivos JSON (`src/config/`), sin tocar los componentes.
* Diseño adaptable (responsive) con soporte de modo oscuro.
* Sitio 100 % estático, publicado en GitHub Pages.

## Stack

Astro 5 · Tailwind CSS v4 · GitHub Pages.

## Empezar

```bash
npm install
npm run dev        # http://localhost:4321/Astro_landing_demo/
```

| Script | Qué hace |
|--------|----------|
| `npm run dev` | Servidor de desarrollo |
| `npm run build` | Build de producción en `dist/` |
| `npm run preview` | Sirve localmente el build |
| `npm run deploy` | Publica `dist/` en GitHub Pages |

> El sitio usa `base: '/Astro_landing_demo'`, por eso la ruta local incluye ese prefijo. Las imágenes de `public/` se referencian con `import.meta.env.BASE_URL`.

## Estructura

```
public/
  images/       Imágenes de proyectos e ilustración del Hero
src/
  components/   Footer y landing/ (Hero, More, Features, About, Projects)
  config/       projects.json y features.json (contenido editable)
  layouts/      Layout base
  pages/        index y about
  styles/       Estilos globales
.github/
  workflows/    Despliegue a GitHub Pages
```

## Sistema de diseño

Estilos con utilidades de Tailwind CSS v4 (integrado vía `@tailwindcss/vite`), con variantes `dark:` para el modo oscuro y estilos globales en `src/styles/`.
