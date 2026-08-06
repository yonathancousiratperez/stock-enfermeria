# Stock Enfermería · RASI

Web de consulta y carga del stock de medicamentos de Enfermería.

- **En vivo:** https://yonathancousiratperez.github.io/stock-enfermeria/
- **Datos:** Supabase (PostgreSQL). El descuento por atención lo hace un trigger
  cuando el bot de Telegram registra la atención; la tabla se actualiza sola por
  Realtime. Google Sheets ya no participa del flujo.
- **Acceso:** una sola contraseña, validada por Supabase Auth. La contraseña no
  está en este repo.

## Archivos

| Archivo | Qué es |
|---|---|
| `index.html` | La aplicación entera: HTML, CSS y JS en un solo archivo, sin build |
| `supabase.js` | supabase-js 2.112.1, versión fija servida desde el propio repo para no depender de un CDN |
| `.github/workflows/deploy-pages.yml` | Publica el sitio en GitHub Pages |

Las cantidades se cuentan **por unidad** (comprimido, ampolla, sobre), nunca por caja.
