# Contribuir

¡Gracias por ayudar! La app es un solo archivo sin dependencias.

1. Haz un fork y crea una rama: `git checkout -b mi-mejora`.
2. Edita `index.html` y pruébalo con `python3 -m http.server 8000`.
3. Comprueba en un móvil (o en el modo responsive del navegador) el contador, el menú y cada sección.
4. Sube el número de versión (`VER` en `index.html`, `CACHE` de `sw.js` y `CHANGELOG.md`).
5. Abre una *pull request* explicando el cambio, con capturas si toca la interfaz.

**Licencia de las aportaciones:** al enviar una pull request aceptas que tu contribución se distribuya bajo la misma licencia (PolyForm Noncommercial 1.0.0) y que el autor pueda ofrecerla también bajo otras licencias, incluidas comerciales.

**Estilo:** JavaScript sin librerías, textos de usuario en español y escapados con `esc()` antes de pintarlos con `innerHTML`. Evita nombres de clase y atributos `data-*` genéricos (`sub`, `big`, `tile`, `data-g`, `data-s`…) porque ya existen estilos y manejadores con esos nombres.
