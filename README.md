# UZDI · Landing page

Landing de presentación del **backend** del Sistema de Gestión Integral UZDI
(proyecto académico PUCE): módulos, explorador de endpoints, arquitectura,
seguridad RBAC, stack y equipo. Es un sitio estático: un solo `index.html`,
sin dependencias ni build.

Con el backend encendido, la página lee **en vivo** su Swagger (`/api/docs-json`)
para listar los endpoints y muestra si la API está en línea. Si el backend no
responde, usa una copia incluida en la página.

Backend: [alex171215/uzdi-backend-p8](https://github.com/alex171215/uzdi-backend-p8)

## Verla en local

Abre `index.html` en el navegador, o sírvela con:

```bash
npx serve .
# o
python -m http.server 5500
```

## Conectar con el backend

La landing consulta `/api/v1` y `/api/docs-json` y enlaza a Swagger. Por defecto usa
el backend desplegado en Render: `https://uzdi-backend-api.onrender.com`.

- Para usar el backend local: `index.html?api=http://localhost:3000`
- Para cambiar el valor por defecto: `API_POR_DEFECTO` al inicio del `<script>` en `index.html`.

El plan gratuito de Render apaga el servicio tras 15 minutos sin uso; la primera
visita puede tardar ~50 s en mostrar "API en línea".

## Publicarla

Funciona en GitHub Pages, Netlify, Vercel o Render (Static Site) sin configuración:
la raíz del repo es la raíz del sitio.

---
Sitio de demostración. No es un sitio oficial del SNAI.
