# 📁 Estructura del Portafolio - Guía para Estudiantes

Esta es la estructura de carpetas que debes seguir para organizar tus proyectos:

```
portafolio/
│
├── index.html              ← Página principal (menú de proyectos)
├── estilos.css             ← Estilos de la página principal
├── README.md               ← Este archivo
│
├── proyecto-ejemplo/       ← Carpeta del proyecto 1
│   └── index.html
│
├── proyecto2/              ← Carpeta del proyecto 2
│   ├── index.html
│   └── estilos.css         (si tiene sus propios estilos)
│
├── proyecto3/              ← Carpeta del proyecto 3
│   └── index.html
│
└── proyecto4/              ← Carpeta del proyecto 4
    └── index.html
```

---

## 🚀 Cómo subir tu portafolio a GitHub Pages

### Paso 1: Crear una cuenta en GitHub
1. Ve a [github.com](https://github.com)
2. Haz clic en "Sign up" y crea tu cuenta

### Paso 2: Crear un nuevo repositorio
1. Inicia sesión en GitHub
2. Haz clic en el **+** (esquina superior derecha) → "New repository"
3. Ponle un nombre: `portafolio` (o el que gustes)
4. Marca la opción **"Public"**
5. Haz clic en "Create repository"

### Paso 3: Subir tus archivos
Elige una de estas dos formas:

#### Opción A: Subir archivos desde el navegador (Más fácil)
1. En tu repositorio nuevo, haz clic en "uploading an existing file"
2. Arrastra tu carpeta `portafolio` completa o sus archivos
3. En "Commit changes", escribe un mensaje como "Mi primer portafolio"
4. Haz clic en "Commit changes"

#### Opción B: Usar Git (Más profesional)
```bash
# 1. Abre una terminal en tu carpeta portafolio
cd "ruta/a/tu/portafolio"

# 2. Inicia git
git init

# 3. Agrega todos los archivos
git add .

# 4. Haz tu primer commit
git commit -m "Mi primer portafolio"

# 5. Conecta con tu repositorio (copia tu URL desde GitHub)
git remote add origin https://github.com/TU_USUARIO/portafolio.git

# 6. Sube los archivos
git push -u origin main
```

### Paso 4: Activar GitHub Pages
1. En tu repositorio, ve a **Settings** (pestaña superior)
2. En el menú lateral, busca **Pages**
3. En "Source", selecciona:
   - **Branch**: `main` o `master`
   - **Folder**: `/ (root)`
4. Haz clic en **Save**

### Paso 5: ¡Ver tu sitio en línea!
Después de 1-3 minutos, tu sitio estará disponible en:
```
https://TU_USUARIO.github.io/portafolio/
```

---

## 📌 Importante: Enlaces Relativos

Cuando creas enlaces desde el `index.html` principal hacia tus proyectos:

```html
<!-- ✅ Correcto - Enlace a carpeta -->
<a href="proyecto-ejemplo/index.html">Ver Proyecto</a>

<!-- ❌ Incorrecto - Enlace absoluto -->
<a href="C:/Usuarios/...">Ver Proyecto</a>
```

Cuando creas un enlace de "Volver" desde un proyecto hacia el índice:

```html
<!-- ✅ Correcto - .. sube un nivel -->
<a href="../index.html">Volver</a>

<!-- ✅ También correcto - a la raíz -->
<a href="/index.html">Volver</a>
```

---

## 🎯 Agregar un nuevo proyecto

1. **Crea una carpeta nueva** para tu proyecto (ej: `mi-nuevo-proyecto/`)
2. **Dentro de esa carpeta**, crea un archivo `index.html`
3. **En el index principal**, agrega una nueva tarjeta copiando el bloque de un proyecto existente
4. **Cambia** el `href` para que apunte a tu nueva carpeta

Ejemplo:
```html
<a href="mi-nuevo-proyecto/index.html" class="proyecto-card">
    <div class="proyecto-imagen">
        <img src="ruta-de-tu-imagen.jpg" alt="Mi Nuevo Proyecto">
        ...
    </div>
</a>
```

---

## 💡 Consejos

- **Nombres de carpetas**: Usa minúsculas y guiones (ej: `mi-proyecto`, no `Mi Proyecto`)
- **Imágenes**: Puedes crear una carpeta `img/` dentro de cada proyecto para sus imágenes
- **Siempre index.html**: GitHub Pages busca automáticamente archivos llamados `index.html`

---

¿Dudas? Consulta con tu instructor 👨‍🏫
