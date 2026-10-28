# Changelog

## 1.8.0
- **Nueva marca: Kaiten** (antes «Sushi Score»). Título, manifest, tarjetas para compartir, nombres de archivo, README, capturas, GIF y portada actualizados.
- Tus datos antiguos se migran solos: partidas (`sushiscore.v3` → `kaiten.v3`) y fotos (`sushiscore-photos` → `kaiten-photos`). Las copias de seguridad anteriores se siguen pudiendo importar.
- **Sin conexión de verdad:** `sw.js` estaba vacío y no cacheaba nada; ahora guarda la app y la sirve offline.
- «Gastado» suma lo que costó cada comida guardada (ya no cambia hacia atrás al modificar el precio por pieza).
- Deshacer (−1) resta de una pieza que exista aunque hayas cambiado de tipo.
- «Borrar todo» también elimina las fotos guardadas.
- Fondo de adorno en temas oscuros: el arroz de los nigiri y onigiri se veía casi negro; ahora se ve blanco.
- Manifest: `id` propio e iconos «any» y «maskable» separados.

## 1.7.0
- **Reseñas** al terminar la comida: valoración de 1 a 5, etiquetas, nota, hasta 4 fotos (IndexedDB) y ubicación por GPS; detalle y edición desde el Historial.
- **Mapa** de tus sitios con OpenFreeMap + MapLibre (carga bajo demanda), ranking por nota, colocar pin a mano y enlace a Google Maps.
- **Tarjeta por comida** con tu foto, **copia completa** con fotos y aviso a los 30 días.
- Corregidas colisiones de atributos `data-*` con el código original y una carrera en la limpieza de fotos huérfanas.

## 1.6.1
- Licencia cambiada de MIT a PolyForm Noncommercial 1.0.0 (uso no comercial). Las copias obtenidas antes de este cambio conservan la licencia con la que se recibieron.

## 1.6.0
- **Interfaz de escritorio** (≥1000 px): contador y panel en directo en dos columnas, secciones abiertas en el panel y atajos de teclado.
- Adaptación a móviles bajos (320×568), apaisado en dos columnas y tabletas.
- Ventanas modales centradas en escritorio y cierre con Escape.

## 1.5.1
- Instalación como app: nombre bajo el icono en iOS, estilo de barra de estado y `favicon.ico`; guía de instalación en el README.

## 1.5.0
- Importador validado y saneado; historial ampliado a 500 comidas; importes en formato español.
- Botón Atrás del móvil integrado con el menú y las secciones; se permite el zoom; respeta `prefers-reduced-motion`.
- Iconos PNG (192, 512 y apple-touch), manifest completo y service worker con red primero.
- Repositorio listo: README con capturas y GIF, portada social, workflow de GitHub Pages, guía de publicación, plantillas de issues y CONTRIBUTING.

## 1.4.1
- Corregido el color gris y el recorte en las secciones por una colisión de clases con el código original (`sub`, `big`, `hx`, `lk`).
- Ajustados los solapes entre ilustraciones y texto en el menú.

## 1.4.0
- Iconografía propia en SVG (nigiri, maki, palillos, torii, bento, trofeo, salsa de soja…) en lugar de emojis: hub, botón central, estadísticas, logros y retos.
- Teselas con ilustración, brillo y animación sutil.

## 1.3.2
- La app ya no depende de la altura heredada del documento (100vh/100dvh): corrige el área de contenido colapsada en visores embebidos.

## 1.3.1
- Corregido el recorte de contenido en el hub y en las vistas interiores (filas de altura automática y rejilla sin encoger).

## 1.3.0
- Hub rediseñado: tarjeta héroe con anillo de comida y nivel, teselas con color propio, gráfica semanal real, medallas, puntos de retos y emojis flotantes de fondo.

## 1.2.0
- Vistas interiores rediseñadas en bento: Estadísticas (hoy, semana, racha, favoritas), Logros (anillo de nivel y medallas) y cabeceras unificadas en Historial y Ajustes.

## 1.1.0
- **Hub bento**: la barra inferior se sustituye por un botón-plato central que abre un menú de teselas grandes con vista previa en vivo (también con swipe ↑).
- **Retos diarios**: 3 retos distintos cada día.
- **Historial** de comidas con lugar, coste y duración (borrable).
- **Tarjeta compartible** en imagen (PNG).
- PWA real: `manifest.webmanifest`, `icon.svg` y `sw.js` (offline).
- Seguridad: el texto del usuario (lugar) se escapa antes de pintarse.

## 1.0.0
- Contador, estadísticas, logros, temas, sonidos y copia de datos.
