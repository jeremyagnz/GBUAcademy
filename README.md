# GBU English Academy – Landing Page

Landing page estilo **link-in-bio** para [GBU English Academy](https://gbuenglishacademy.com), construida con React + Vite y desplegada en Netlify.

## Requisitos

- Node.js `^20.19.0` o `>=22.12.0`
- npm `>=9`

## Desarrollo local

```bash
npm install
npm run dev
```

Abre http://localhost:5173 en tu navegador.

## Build de producción

```bash
npm run build      # genera la carpeta dist/
npm run preview    # previsualiza el build localmente
```

## Deploy en Netlify

El proyecto incluye `netlify.toml` listo para usar. Solo conecta el repositorio en Netlify y el deploy se realizará automáticamente con cada push a `main`.

- **Comando de build**: `npm run build`
- **Directorio de publicación**: `dist`

## Estructura

```
├── index.html
├── netlify.toml
├── src/
│   ├── App.jsx        # Componente principal (links, perfil, redes)
│   ├── App.css        # Estilos de la landing page
│   ├── index.css      # Reset global
│   ├── main.jsx       # Punto de entrada React
│   └── assets/        # Imágenes y recursos
└── public/
    ├── favicon.svg
    └── icons.svg
```
