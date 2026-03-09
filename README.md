# IA
creación de una pagina web con ionic solo usando la ia de claude

# ⚙️ Gears of War 3 — Historia de Marcus Fenix

> Página web interactiva desarrollada con **Ionic Framework** que narra la historia completa de Marcus Fenix en orden cronológico, con tarjetas temáticas, espacios para imágenes y videos.

---

## 📋 Requisitos Previos

Antes de ejecutar el proyecto, verificar que tienes instalado lo siguiente:

| Herramienta | Versión mínima | Verificar con |
|-------------|---------------|---------------|
| Node.js | 16.x o superior | `node -v` |
| npm | 8.x o superior | `npm -v` |
| Ionic CLI | 7.x o superior | `ionic -v` |
| Git | cualquier versión | `git --version` |

---

## 🚀 Paso a Paso para Ejecutar el Proyecto

### 1. Clonar el repositorio

```bash
git clone https://github.com/TU_USUARIO/NOMBRE_DEL_REPO.git
cd NOMBRE_DEL_REPO
```

### 2. Instalar Ionic CLI (si no lo tienes)

```bash
npm install -g @ionic/cli
```

Verificar instalación:

```bash
ionic -v
# Debe mostrar algo como: 7.x.x
```

### 3. Instalar dependencias del proyecto

```bash
npm install
```

### 4. Ejecutar en modo desarrollo

```bash
ionic serve
```

El navegador se abrirá automáticamente en:

```
http://localhost:8100
```

---

## 📁 Estructura del Proyecto

```
gow-project/
├── src/
│   ├── css/
│   │   ├── variables.css       # Tokens de color y tipografía
│   │   ├── background.css      # Capa de fondo y efectos
│   │   ├── hero.css            # Sección hero principal
│   │   ├── cards.css           # Estilos de las tarjetas
│   │   ├── timeline.css        # Track y capítulos
│   │   ├── components.css      # Slots de imagen, video, quotes
│   │   └── animations.css      # Keyframes y transiciones
│   ├── js/
│   │   └── main.js             # Lógica e interacciones
│   ├── assets/
│   │   ├── images/             # Imágenes del juego (agregar aquí)
│   │   └── videos/             # Videos locales (agregar aquí)
│   └── index.html              # Página principal
├── package.json
└── README.md
```

---

## 🖼️ Agregar Imágenes y Videos

Cada tarjeta tiene espacios reservados. Para reemplazarlos:

**Imagen:**
```html
<!-- Buscar el placeholder correspondiente y reemplazar: -->
<div class="card-image-slot">
  <img src="assets/images/tu-imagen.jpg" alt="descripción" />
</div>
```

**Video de YouTube:**
```html
<div class="video-slot">
  <iframe
    src="https://www.youtube.com/embed/ID_DEL_VIDEO"
    allowfullscreen>
  </iframe>
</div>
```

---

## 🛠️ Posibles Errores y Soluciones

**Error: `ionic: command not found`**
```bash
npm install -g @ionic/cli
```

**Error: `node_modules not found`**
```bash
npm install
```

**Puerto 8100 ocupado:**
```bash
ionic serve --port 8200
```

**Fuentes de Google no cargan (sin internet):**
> Descargar las fuentes *Bebas Neue* y *Barlow* desde [Google Fonts](https://fonts.google.com) y referenciarlas localmente en `index.html`.

---

## 🌐 Build para Producción

```bash
ionic build --prod
```

Los archivos compilados quedarán en la carpeta `/www`, listos para subir a cualquier hosting estático (Netlify, Vercel, GitHub Pages).

---

## 👥 Colaboradores

Si encuentras un bug o quieres mejorar el contenido:

1. Haz un **fork** del repositorio
2. Crea una rama: `git checkout -b fix/nombre-del-fix`
3. Haz commit: `git commit -m "descripción del cambio"`
4. Abre un **Pull Request**

---

> *"Sobrevivir no es lo mismo que vivir. Pero a veces es todo lo que tienes."*
> — **Marcus Fenix**