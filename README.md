# Kuwü Tejidos - Sitio Web Artesanal

Sitio web para Kuwü Tejidos, negocio de tejidos artesanales hechos a mano.

## 🎨 Características

- Diseño minimalista y elegante con fondo blanco hueso (off-white)
- Single Page Application (SPA) responsive
- Integración directa con WhatsApp para consultas
- Secciones: Hero, Catálogo, Sobre Mí, Filosofía
- Componentes React modulares
- Estilos con Tailwind CSS

## 🚀 Instalación

1. Instalar dependencias:
```bash
npm install
```

2. Iniciar servidor de desarrollo:
```bash
npm run dev
```

3. Abrir navegador en `http://localhost:3000`

## 📁 Estructura de Carpetas

```
kuwütejidos/
├── public/
│   ├── logo.png                 # Logo de la marca
│   └── images/                  # Imágenes de productos
│       ├── hero-placeholder.jpg
│       ├── about-placeholder.jpg
│       ├── product-1.jpg
│       ├── product-2.jpg
│       └── ...
├── src/
│   ├── components/
│   │   ├── Header.jsx
│   │   ├── Hero.jsx
│   │   ├── Catalog.jsx
│   │   ├── About.jsx
│   │   ├── Philosophy.jsx
│   │   └── Footer.jsx
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
└── package.json
```

## 📸 Imágenes Requeridas

Coloca tus imágenes en la carpeta `public/images/`:

- `logo.png` - Logo con araña y palillos de tejer (en carpeta public/)
- `hero-placeholder.jpg` - Foto de la artesana tejiendo o sus manos
- `about-placeholder.jpg` - Foto para la sección "Sobre Mí"
- `product-1.jpg` a `product-6.jpg` - Fotos de los productos/chalecos

## ⚙️ Configuración

### WhatsApp

Actualiza el número de WhatsApp en:
- `src/components/Catalog.jsx` (línea 54)
- `src/components/Footer.jsx` (línea 4)

Cambia `'56912345678'` por tu número con código de país (sin +).

### Productos

Edita el array de productos en `src/components/Catalog.jsx` para personalizar:
- Nombres de productos
- Descripciones
- Rutas de imágenes

## 🎨 Paleta de Colores

- **Fondo principal**: `#FAF9F6` (bone/blanco hueso)
- **Texto**: Negro (`#000000`)
- **WhatsApp**: Verde (`#16A34A`)
- **Acentos**: Grises suaves

## 📱 Responsive

El sitio es completamente responsive y se adapta a:
- 📱 Móviles (< 640px)
- 📱 Tablets (640px - 1024px)
- 💻 Desktop (> 1024px)

## 🛠️ Tecnologías

- React 18
- Vite
- Tailwind CSS
- Lucide React (iconos)
- Google Fonts (Playfair Display, Inter)

## 📝 Scripts Disponibles

- `npm run dev` - Inicia servidor de desarrollo
- `npm run build` - Genera build de producción
- `npm run preview` - Vista previa del build

## 🌐 Despliegue

Para desplegar en producción:

1. Generar build:
```bash
npm run build
```

2. La carpeta `dist/` contendrá los archivos estáticos listos para desplegar en cualquier hosting (Netlify, Vercel, etc.)

## 📞 Contacto

Para cualquier consulta técnica o personalización, consulta la documentación de React y Tailwind CSS.
