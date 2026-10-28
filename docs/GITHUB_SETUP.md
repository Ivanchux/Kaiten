# Publicar el repositorio

## Descripción (campo *About*)
```
🍣 Cuenta tus piezas de sushi, sube de nivel y completa retos. PWA de un solo archivo, sin cuentas ni anuncios, 100% offline. Ilustraciones SVG propias, temas, logros y tarjeta para compartir.
```

## Topics (categorías)
`sushi` `pwa` `progressive-web-app` `vanilla-javascript` `html5` `css3` `single-file` `offline-first` `mobile-first` `counter-app` `gamification` `localstorage` `no-dependencies` `svg` `spanish` `food` `maplibre` `openstreetmap` `indexeddb` `geolocation`

## Website
`https://ivanchux.github.io/Kaiten/`

## Pasos
```bash
cd Kaiten
git init -b main
git add .
git commit -m "feat: Kaiten v1.8.0"
git remote add origin https://github.com/Ivanchux/Kaiten.git
git push -u origin main
```
Con la CLI `gh` (opcional, hace también lo de la descripción y los topics):
```bash
gh repo create Kaiten --public --source=. --remote=origin --push \
  --description "🍣 Cuenta tus piezas de sushi, sube de nivel y completa retos. PWA de un solo archivo, sin cuentas ni anuncios, 100% offline."
gh repo edit --homepage "https://ivanchux.github.io/Kaiten/" \
  --add-topic sushi,pwa,progressive-web-app,vanilla-javascript,html5,css3,single-file,offline-first,mobile-first,counter-app,gamification,localstorage,no-dependencies,svg,spanish,food
```

## GitHub Pages
*Settings → Pages → Build and deployment → Source: **GitHub Actions***. El workflow `.github/workflows/pages.yml` publica la app en cada push a `main`.

## Imagen para redes
*Settings → General → Social preview → Upload* y elige `docs/social-preview.png` (1280×640).

## Antes de anunciar la app
- Haz una captura del mapa real (no se puede generar sin conexión) y súbela a `docs/screenshots/14-mapa.png`; añádela a la galería del README.
- Si la publicas en serio, añade una política de privacidad: la ubicación y las fotos son datos personales (RGPD).

## Lanzar la versión
*Releases → Draft a new release* con la etiqueta `v1.8.0` y el texto de `CHANGELOG.md`.
