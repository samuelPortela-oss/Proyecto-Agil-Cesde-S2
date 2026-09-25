# Sprint 1 — Sprint Backlog

## 🎯 Objetivo del Sprint
Implementar las bases de la aplicación: flujo de autenticación tradicional de usuarios, gestión del perfil básico y la capacidad de publicar y buscar prendas dentro del catálogo[cite: 2, 3].

---

## 📋 Historias Seleccionadas y Tareas

### 🔐 Feature 1.1: Autenticación y Acceso (Fase 1)
#### US-01.1: Registro de cuenta con correo
- [ ] Diseñar interfaz de registro en la app móvil
- [ ] Crear endpoint de creación de usuario en backend[cite: 3]
- [ ] Implementar encriptación de contraseñas
- [ ] Validar formato de correo y duplicados

#### US-02.1: Inicio de sesión con correo y contraseña
- [ ] Diseñar formulario de login[cite: 3]
- [ ] Generar tokens de autenticación (JWT)
- [ ] Manejo de errores por credenciales incorrectas

#### US-02.2: Cierre de sesión
- [ ] Implementar opción para cerrar sesión y limpiar sesión local[cite: 3]

---

### 👤 Feature 1.2: Perfil Personal (Fase 1)
#### US-04: Perfil personal básico
- [ ] Crear pantalla para editar nombre, foto, biografía y ubicación[cite: 3]
- [ ] Guardar cambios del perfil en la base de datos

---

### 📦 Feature 2.1: Gestión de Publicaciones (Fase 1)
#### US-07: Publicar una prenda
- [ ] Diseñar formulario para subir fotos, precio, talla, estado y categoría[cite: 3]
- [ ] Configurar almacenamiento de imágenes en la nube
- [ ] Guardar la publicación asociada al usuario vendedor

#### US-08: Vista previa antes de publicar
- [ ] Implementar pantalla modal con la vista previa de la prenda antes de confirmar[cite: 3]

---

### 🔍 Feature 2.2: Descubrimiento y Búsqueda
#### US-09: Búsqueda por texto y filtros avanzados
- [ ] Diseñar barra de búsqueda y filtros (talla, precio, ubicación, categoría)[cite: 3]
- [ ] Crear endpoint de búsqueda filtrada en backend

#### US-10: Página de detalle de la prenda
- [ ] Crear vista para ver galería de fotos e información completa de la prenda[cite: 3]

---

## ℹ️ Información del Sprint
- **Duración:** 2 semanas (Semanas 1–2)[cite: 2]
- **Historias de Usuario:** 7 historias seleccionadas[cite: 3]
- **Estimación total:** ~30 Puntos de Historia
- **Versión esperada al finalizar:** `v0.1.0`[cite: 2]