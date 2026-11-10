# Juan Beltran · App (v0.5)

App web instalable (PWA) de Juan Beltran: restaurantes, recetas costeadas, materia prima, eventos, Shopin, Moodboards, JBShare (Pole/Podio/Rookie/Box), Controles (turnos, asesorías, pagos, recibos PDF), Ideas y Configuración.

## Archivos
- `index.html` – toda la app (HTML + CSS + JS en un solo archivo).
- `lamp.jpg` – fondo de la pantalla de carga.
- `manifest.webmanifest`, `icons/` – para instalarla en el celular con ícono propio.
- `sw.js` – service worker: la app abre sin internet después de la primera vez.
- Los datos NO van en el repositorio (sería público). Se cargan en cada dispositivo con Configuración → Restaurar copia, usando el archivo juan-beltran-copia-datos.json.

## Cómo funciona por dentro
- Sin servidor ni base de datos: es 100% estática. Los datos se guardan en el almacenamiento local del navegador (localStorage) de cada dispositivo.
- Librerías por CDN: SheetJS 0.18.5 (Excel) y jsPDF 2.5.1 (recibos), fuente M PLUS Rounded 1c de Google Fonts.
- Copia de seguridad: Configuración → Descargar copia / Restaurar copia (archivo .json). Sirve para pasar los datos entre dispositivos.

## Publicarla gratis
Cualquier hosting estático con HTTPS sirve (GitHub Pages, Netlify, Vercel, Cloudflare Pages). Se sube la carpeta tal cual; no hay que compilar nada.

## Instalarla en iPhone
Abrir la URL en Safari → botón Compartir → "Agregar a pantalla de inicio".

