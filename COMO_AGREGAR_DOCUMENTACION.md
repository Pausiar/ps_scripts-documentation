# 📚 Cómo Agregar Documentación de un Nuevo Script

Esta guía te mostrará paso a paso cómo añadir documentación para un nuevo script en este repositorio.

## 🎯 Pasos para Agregar un Nuevo Script

### 1️⃣ Crear el Archivo HTML de Documentación

1. Copia el archivo `TEMPLATE.html` y renómbralo según tu script:
   ```bash
   cp TEMPLATE.html nombre_script.html
   ```
   Por ejemplo: `ps_blackmarket.html`, `ps_inventory.html`, etc.

2. Abre el archivo y reemplaza los siguientes marcadores:
   - `[NOMBRE_SCRIPT]` - Nombre de tu script (ej: "BlackMarket", "Inventory")
   - `[EMOJI]` - Emoji representativo (ej: 🛒, 📦, 🚗)
   - `[DESCRIPCIÓN CORTA DEL SCRIPT]` - Una descripción breve de 1-2 líneas
   - Actualiza la versión en `<span class="version">v1.0.0</span>`

3. Completa las secciones:
   - **Características Principales**: Lista las funcionalidades clave
   - **Requisitos**: Framework, base de datos, dependencias
   - **Instalación**: Pasos detallados para instalar
   - **Configuración**: Ejemplos del archivo config.lua
   - **Uso**: Comandos, permisos, ejemplos de uso
   - **Solución de Problemas**: Problemas comunes y soluciones

### 2️⃣ Agregar el Script al Index

Abre `index.html` y añade una nueva tarjeta dentro de la sección `<section class="scripts-grid" id="scripts">`:

```html
<!-- Tu Nuevo Script -->
<div class="script-card" data-tags="fivem [tags relevantes]">
    <h3>[EMOJI] [NOMBRE DEL SCRIPT]</h3>
    <p>[Descripción corta del script de 2-3 líneas]</p>
    <div class="script-meta">
        <span class="tag">FiveM</span>
        <span class="tag">[Tag 1]</span>
        <span class="tag">[Tag 2]</span>
    </div>
    <div class="script-actions">
        <a href="nombre_script.html" class="btn btn-primary">Ver Documentación</a>
        <a href="https://github.com/Pausiar/ps_nombre_script" class="btn btn-secondary">Ver en GitHub</a>
    </div>
</div>
```

**Importante:** Coloca la tarjeta en orden alfabético o por categoría junto a scripts similares.

### 3️⃣ Configurar los Tags Correctamente

Los tags son importantes para la función de búsqueda. Incluye en `data-tags`:
- Tipo de script: `fivem`, `standalone`, `esx`, `qbcore`
- Categoría: `security`, `admin`, `vehicles`, `inventory`, `roleplay`
- Características: `mysql`, `nui`, `ui`, `anticheat`
- Palabras clave relevantes en español e inglés

Ejemplo:
```html
data-tags="fivem esx inventory mysql nui inventario"
```

### 4️⃣ Verificar el Resultado

1. Abre `index.html` en tu navegador
2. Busca tu script usando la barra de búsqueda
3. Verifica que la tarjeta se muestre correctamente
4. Haz clic en "Ver Documentación" para revisar la página del script
5. Prueba la navegación entre páginas

## 🎨 Personalización Avanzada

### Cambiar el Esquema de Colores

En tu archivo HTML, puedes personalizar los colores en la sección `:root`:

```css
:root {
    --primary: #6366f1;      /* Color principal */
    --primary-dark: #4f46e5; /* Color principal oscuro */
    --secondary: #10b981;    /* Color secundario */
    /* ... */
}
```

### Añadir Imágenes o Videos

Para incluir capturas de pantalla:

```html
<div class="content-section">
    <h2>📸 Capturas de Pantalla</h2>
    <img src="images/screenshot1.png" alt="Descripción" style="max-width: 100%; border-radius: 10px; margin: 1rem 0;">
</div>
```

Para incluir videos de YouTube:

```html
<div class="content-section">
    <h2>🎥 Video Demostración</h2>
    <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin: 1rem 0;">
        <iframe 
            style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; border-radius: 10px;" 
            src="https://www.youtube.com/embed/VIDEO_ID" 
            allowfullscreen>
        </iframe>
    </div>
</div>
```

## ✅ Checklist de Verificación

Antes de publicar tu documentación, verifica:

- [ ] El archivo HTML está nombrado correctamente (minúsculas, guiones)
- [ ] Todos los marcadores `[PLACEHOLDER]` fueron reemplazados
- [ ] La tarjeta fue añadida al `index.html`
- [ ] Los tags son relevantes y útiles para búsquedas
- [ ] Los enlaces funcionan correctamente
- [ ] La navegación "Volver" funciona
- [ ] El código de ejemplo está correctamente formateado
- [ ] No hay errores de ortografía
- [ ] Las imágenes/videos (si hay) cargan correctamente

## 📝 Ejemplo Completo

Aquí hay un ejemplo de cómo se vería una tarjeta completa en el index:

```html
<!-- BlackMarket System -->
<div class="script-card" data-tags="fivem esx blackmarket illegal shop tienda mercado">
    <h3>🛒 PS BlackMarket</h3>
    <p>Sistema completo de mercado negro con integración ESX, ox_inventory y ox_target. Incluye sistema de reputación, productos ilegales y misiones especiales.</p>
    <div class="script-meta">
        <span class="tag">ESX</span>
        <span class="tag">ox_inventory</span>
        <span class="tag">MySQL</span>
        <span class="tag">Roleplay</span>
    </div>
    <div class="script-actions">
        <a href="blackmarket.html" class="btn btn-primary">Ver Documentación</a>
        <a href="https://github.com/Pausiar/ps_blackmarket" class="btn btn-secondary">Ver en GitHub</a>
    </div>
</div>
```

## 🆘 Ayuda

Si necesitas ayuda para añadir documentación:
- **Discord:** @pausiar
- **GitHub Issues:** [Crear un issue](https://github.com/Pausiar/ps_scripts-documentation/issues)

---

¡Gracias por contribuir a la documentación de Pausiar Scripts! 🎉
