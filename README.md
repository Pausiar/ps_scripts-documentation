# ps_scripts - Documentación

Bienvenido a la documentación de **ps_scripts**.
Este repositorio contiene la web estática con guías de instalación, configuración y uso para los scripts desarrollados por **Pausiar / ps_scripts**.

---

## Documentación de scripts

Cada página de script incluye:

* Requisitos
* Instalación
* Configuración
* Comandos disponibles
* Ejemplos o notas de uso
* Showcase cuando está disponible

La portada principal está en [`index.html`](./index.html) y enlaza las páginas HTML de cada recurso.

---

## Scripts disponibles

* `ps_anticheat` - Anticheat con NUI, detección de cheats y base de datos.
* `ps_rental` - Sistema de alquiler de vehículos con panel para administradores.
* `ps_garage` - Sistema de garajes, transferencias y persistencia de tuneos.
* `ps_admin` - Menú avanzado de administración.
* `ps_race` - Sistema de carreras punto a punto.
* `ps_loadingscreen` - Pantalla de carga cinematográfica.
* `ps_antipg` - Sistema modular anti-PowerGaming.
* `ps_carcrash` - Sistema realista de daños por colisión.
* `ps_pausemenu` - Menú de pausa moderno para FiveM.
* `ps_ammurobery` - Robo al Ammunation con recompensas y alertas policiales.

---

## Desarrollo local

Este sitio es documentación HTML estática, por lo que no requiere dependencias de Node.js ni un proceso de build.

Para revisarlo localmente puedes abrir `index.html` directamente o servir la carpeta con un servidor estático:

```bash
python3 -m http.server 8080
```

Después abre `http://127.0.0.1:8080/index.html`.

---

## Sistema visual

La interfaz usa estilos compartidos en [`assets/docs-premium.css`](./assets/docs-premium.css) y un sprite SVG optimizado en [`assets/icons.svg`](./assets/icons.svg).

Este sistema sustituye los emojis usados como iconos por SVG consistentes, accesibles y sin dependencias externas.

---

## Despliegue

El repositorio está preparado para publicarse como sitio estático en GitHub Pages.

URL esperada si GitHub Pages está habilitado para este repositorio:

```text
https://pausiar.github.io/ps_scripts-documentation/
```

---

## Contacto

* Discord: `@pausiar`
* GitHub: [Pausiar](https://github.com/Pausiar)

---

Gracias por usar **ps_scripts**.
