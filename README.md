
# Portafolio de Cuervo (Jekyll + GitHub Pages)

Portafolio técnico gratuito alojado en GitHub Pages usando el tema **Minimal Mistakes**.

## Despliegue rápido

1. Crea un repo llamado `USERNAME.github.io` en tu cuenta de GitHub.
2. Sube todos los archivos de esta carpeta al repo.
3. Edita `_config.yml` y reemplaza `USERNAME` por tu usuario de GitHub y tu email.
4. En GitHub, ve a **Settings → Pages** y asegúrate de que la rama `main` está publicada.
5. Espera 1–2 minutos y abre `https://USERNAME.github.io`.

## Estructura
- `_pages/`: páginas (Proyectos, Sobre mí, Contacto)
- `_posts/`: proyectos como posts (ejemplo incluido)
- `_data/navigation.yml`: navegación principal
- `assets/images/`: imágenes del sitio
- `_config.yml`: configuración del sitio y del tema

## Añadir proyectos
Crea archivos en `_posts/` con nombre `YYYY-MM-DD-titulo.md`. Usa el front matter del ejemplo.

## Desarrollo local (opcional)
Requiere Ruby:
```bash
gem install bundler
bundle install
bundle exec jekyll serve
```
Luego abre `http://127.0.0.1:4000`.

## Licencia
Tu contenido es tuyo. El tema Minimal Mistakes se usa bajo su licencia.
