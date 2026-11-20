# Farpal.cl

Sitio web de Farpal Ltda. — Aseo industrial y servicios generales, Santiago de Chile.

Sitio estático (HTML/CSS/JS en un solo archivo). Para desplegar en Vercel: importar este repo, framework "Other", sin build command, output directory raíz.

## Características

- Diseño moderno con animaciones al hacer scroll (AOS library)
- Hero con foto real del equipo
- Franja de clientes (Metro, MOP, Ferrovial, etc.)
- Galería de trabajos reales
- Testimonios de clientes
- Totalmente responsive (mobile-first)
- WhatsApp como canal principal de contacto
- Contador animado de estadísticas
- SEO optimizado con Schema.org

## Tecnologías

- HTML5 + CSS3 (custom properties, grid, flexbox)
- AOS (Animate On Scroll) via CDN
- Google Fonts (Sora + Inter)
- Sin dependencias de build

## Despliegue en Vercel

1. Importar repositorio desde GitHub
2. Framework Preset: **Other**
3. Root Directory: `/`
4. Build Command: (vacío)
5. Output Directory: (vacío o `.`)
6. Deploy

## Pendientes de editar

- Nombres del equipo (sección eliminada temporalmente — agregar cuando se tengan los datos)
- Verificar que las fotos se vean correctamente en producción

## Fotos de trabajos (galería)

Las fotos están en `assets/trabajos/` con el formato `<servicio>-NN.webp` (tamaño grande, para el visor) y `<servicio>-NN-t.webp` (miniatura, para la grilla).
Servicios: `aseo`, `tabiqueria`, `pintura`, `pisos`, `gasfiteria`, `climatizacion`, `electricidad`, `sanitizacion`.

Para agregar una foto: sube los dos archivos y agrega una línea en el objeto `PHOTOS` al final de `index.html`
(formato `["NN", "Descripción", 1 si es horizontal / 0 si es vertical]`). Las 13 fotos destacadas de "Todos" se definen en `FEATURED`.

La imagen para redes sociales (vista previa al compartir el link) es `assets/og-image.jpg` (1200×630).
