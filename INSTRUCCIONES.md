# 📋 Instrucciones para Configurar Kuwü Tejidos

## Paso 1: Preparar las Imágenes

### Logo
Coloca tu archivo `logo.png` (con la araña y palillos de tejer) en:
```
d:\kuwütejidos\public\logo.png
```

### Imágenes de la Página
Coloca las siguientes imágenes en `d:\kuwütejidos\public\images\`:

1. **hero-placeholder.jpg** - Foto principal de la artesana tejiendo o sus manos en acción
2. **about-placeholder.jpg** - Foto para la sección "Sobre Mí"
3. **product-1.jpg** - Foto del primer chaleco/tejido
4. **product-2.jpg** - Foto del segundo chaleco/tejido
5. **product-3.jpg** - Foto del tercer chaleco/tejido
6. **product-4.jpg** - Foto del cuarto chaleco/tejido
7. **product-5.jpg** - Foto del quinto chaleco/tejido
8. **product-6.jpg** - Foto del sexto chaleco/tejido

**Nota:** Si no tienes las imágenes todavía, la página usará imágenes temporales de internet.

## Paso 2: Configurar WhatsApp

Abre estos archivos y cambia el número de WhatsApp:

### En `src/components/Catalog.jsx` (línea ~54):
```javascript
const whatsappNumber = '56912345678'  // Cambia por tu número
```

### En `src/components/Footer.jsx` (línea ~4):
```javascript
const whatsappNumber = '56912345678'  // Cambia por tu número
```

**Formato del número:** Código de país + número (sin espacios, sin +)
- Ejemplo Chile: `56912345678`
- Ejemplo Argentina: `5491123456789`

## Paso 3: Instalar y Ejecutar

Abre una terminal en `d:\kuwütejidos` y ejecuta:

```bash
# Instalar dependencias
npm install

# Iniciar servidor de desarrollo
npm run dev
```

El navegador se abrirá automáticamente en `http://localhost:3000`

## Paso 4: Personalizar Contenido

### Actualizar Texto "Sobre Mí"
Edita `src/components/About.jsx` (líneas 20-35) con tu historia personal.

### Cambiar Productos del Catálogo
Edita `src/components/Catalog.jsx` (líneas 3-48) para actualizar:
- Nombres de productos
- Descripciones
- Rutas de imágenes

### Actualizar Contactos en Footer
Edita `src/components/Footer.jsx` (líneas 52-75) para actualizar:
- Email
- Instagram
- Facebook

## Paso 5: Generar Versión para Publicar

Cuando todo esté listo para publicar:

```bash
npm run build
```

Esto creará una carpeta `dist/` con todos los archivos listos para subir a un servidor web.

## 🆘 Solución de Problemas

### El logo no aparece
- Verifica que `logo.png` esté en la carpeta `public/`
- Refresca el navegador (Ctrl + F5)

### Las imágenes de productos no aparecen
- Colócalas en `public/images/`
- Verifica que los nombres coincidan exactamente
- La página mostrará imágenes temporales si no encuentra las tuyas

### Error al ejecutar npm
- Asegúrate de tener Node.js instalado (versión 16 o superior)
- Intenta eliminar `node_modules` y ejecutar `npm install` nuevamente

## ✨ Listo!

Tu sitio web está configurado y listo para usar. Solo necesitas:
1. ✅ Agregar tus imágenes
2. ✅ Configurar tu número de WhatsApp
3. ✅ Personalizar el contenido
4. ✅ ¡Publicar!
