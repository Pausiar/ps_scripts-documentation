# 📚 Script Documentation

Una elegante página web para documentar tus scripts con una interfaz moderna y funcional.

## 🚀 Ver la documentación

Visita: `https://tu-usuario.github.io/nombre-repositorio`

## ✨ Características

- **Diseño moderno** con efectos glassmorphism y animaciones suaves
- **Responsive** - Se adapta a todos los dispositivos
- **Búsqueda en tiempo real** de scripts
- **Modal interactivo** para ver el código completo
- **Syntax highlighting** con Prism.js
- **Tema oscuro** profesional
- **Fácil de personalizar**

## 📁 Estructura del proyecto

```
.
├── index.html          # Página principal
├── README.md          # Este archivo
├── _config.yml        # Configuración de Jekyll (opcional)
└── scripts/           # Directorio para tus scripts (opcional)
    ├── backup.py
    ├── monitor.sh
    └── ...
```

## 🛠️ Configuración

### 1. Activar GitHub Pages

1. Ve a la configuración de tu repositorio
2. Scroll hasta "Pages" en el sidebar
3. En "Source", selecciona "Deploy from a branch"
4. Selecciona la rama `main` y folder `/ (root)`
5. Guarda los cambios

### 2. Personalizar el contenido

Edita `index.html` para:
- Cambiar el título y descripción
- Agregar/modificar tus scripts
- Actualizar los enlaces de GitHub
- Personalizar los colores y estilos

### 3. Agregar nuevos scripts

Para agregar un nuevo script, sigue este formato en el HTML:

```html
<div class="script-card" data-tags="python automation">
    <h3>🔥 Tu Script</h3>
    <p>Descripción de tu script...</p>
    <div class="script-meta">
        <span class="tag">Python</span>
        <span class="tag">Tag2</span>
    </div>
    <div class="script-actions">
        <button class="btn btn-primary" onclick="showModal('tu-script-id')">Ver Código</button>
        <a href="#" class="btn btn-secondary">Descargar</a>
    </div>
</div>
```

Y agrega los datos del script en el objeto `scriptsData` en JavaScript.

## 🎨 Personalización

### Colores
Modifica las variables CSS en `:root` para cambiar la paleta de colores:

```css
:root {
    --primary: #6366f1;        /* Color primario */
    --secondary: #10b981;      /* Color secundario */
    --dark: #0f172a;          /* Fondo principal */
    /* ... más variables */
}
```

### Fuentes
Para cambiar la fuente, actualiza la importación y la familia de fuentes:

```css
@import url('https://fonts.googleapis.com/css2?family=TuFuente:wght@400;500;600;700;800&display=swap');

body {
    font-family: 'TuFuente', sans-serif;
}
```

## 📱 Responsive

La página está optimizada para:
- 📱 Móviles (320px+)
- 📱 Tablets (768px+)  
- 💻 Desktop (1024px+)
- 🖥️ Large screens (1200px+)

## 🔧 Tecnologías utilizadas

- **HTML5** - Estructura semántica
- **CSS3** - Estilos modernos con CSS Grid y Flexbox
- **JavaScript** - Interactividad y funcionalidad
- **Prism.js** - Syntax highlighting
- **GitHub Pages** - Hosting gratuito

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - mira el archivo [LICENSE](LICENSE) para más detalles.

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Si tienes ideas para mejorar la documentación:

1. Fork el proyecto
2. Crea tu rama de feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📞 Contacto

**Tu Nombre** - [@tu-usuario](https://github.com/tu-usuario)

Project Link: [https://github.com/tu-usuario/nombre-repositorio](https://github.com/tu-usuario/nombre-repositorio)

---

⭐ ¡No olvides dar una estrella al repo si te gusta el proyecto!
