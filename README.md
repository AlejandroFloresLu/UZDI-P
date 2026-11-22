# UZDI · Presentación del backend

Presentación web de la defensa del **backend** del Sistema de Gestión Integral UZDI
(proyecto académico PUCE). Es un sitio estático: `index.html` y `assets/der-uzdi.svg`,
sin dependencias ni build.

Publicada en GitHub Pages: https://alejandrofloreslu.github.io/UZDI-P/

Backend: [alex171215/uzdi-backend-p8](https://github.com/alex171215/uzdi-backend-p8)

## Estructura (unos 20 minutos)

| # | Pantalla | Tiempo |
|---|---|---|
| 0 | Portada y agenda | 0:30 |
| 1 | Diagrama entidad-relación | 3 min |
| 2 | Flujo de una petición | 3 min |
| 3 | Seguridad y permisos | 2 min |
| 4 | Auditoría de datos | 2 min |
| 5 | Endpoints (petición y respuesta reales) | 4 min |
| 6 | Despliegue en Linux y Docker | 2 min |
| 7 | Demo en vivo en Swagger | 3 min |
| 8 | Cierre | 0:30 |

Cada pantalla tiene a la derecha el panel **"Qué cambiamos"** (antes → ahora).
Al final hay un anexo con el explorador de todos los endpoints.

## Cómo presentar

- **Flechas ← →** (o Re Pág / Av Pág): pantalla anterior y siguiente. Inicio y Fin van a la primera y la última.
- **Botón 20:00** (arriba): inicia o pausa el temporizador; doble clic lo reinicia. Se pone rojo en los últimos 2 minutos.
- Los botones de la demo abren cada endpoint directamente en Swagger.
- Abrir la página 2 minutos antes: el plan gratuito de Render tarda unos 50 s en despertar.

## Conectar con el backend

Por defecto usa el backend desplegado en Render: `https://uzdi-backend-api.onrender.com`.

- Backend local: `index.html?api=http://localhost:3000`
- Para cambiar el valor por defecto: `API_POR_DEFECTO` al inicio del `<script>` en `index.html`.

Con el backend en línea, la página muestra "API en línea" y lee la lista de endpoints de
`/api/docs-json`. Si no responde, usa una copia incluida en la página.

---
Sitio de demostración. No es un sitio oficial del SNAI.
