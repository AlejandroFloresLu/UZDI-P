# UZDI · Landing page

Página de inicio pública del Sistema de Gestión Integral UZDI (proyecto académico PUCE).
Es un sitio estático: un solo `index.html`, sin dependencias ni build.

Backend: [alex171215/uzdi-backend-p8](https://github.com/alex171215/uzdi-backend-p8)

## Verla en local

Abre `index.html` en el navegador, o sírvela con:

```bash
npx serve .
# o
python -m http.server 5500
```

## Conectar con el backend

La landing muestra si la API está en línea y enlaza a Swagger. Por defecto usa
`http://localhost:3000`. Para apuntar a otro backend:

- Cambia `API_POR_DEFECTO` al inicio del `<script>` en `index.html`, o
- Pasa la URL en la dirección: `index.html?api=https://tu-api.onrender.com`

## Publicarla

Funciona en GitHub Pages, Netlify, Vercel o Render (Static Site) sin configuración:
la raíz del repo es la raíz del sitio.

---
Sitio de demostración. No es un sitio oficial del SNAI.
