# 📋 Detalle de Historias de Usuario — Reviste

En este documento se detallan las Historias de Usuario (US) principales del proyecto, organizadas por Épicas y Features, incluyendo sus criterios de aceptación y estimaciones.

---

## 🔐 Épica 1: Gestión de Usuarios y Cuentas

### Feature 1.1: Autenticación y Acceso

#### US-01 — Registro de cuenta tradicional
**Como** usuario nuevo  
**Quiero** registrarme utilizando mi correo electrónico y una contraseña  
**Para** crear una cuenta personal y acceder a la plataforma  

* **Criterios de Aceptación:**
  - El usuario debe ingresar nombre completo, correo electrónico válido y contraseña.
  - La contraseña debe tener al menos 8 caracteres, incluyendo un número y una letra mayúscula.
  - El sistema debe validar que el correo no esté registrado previamente.
  - El sistema debe almacenar la contraseña de forma encriptada.
* **Prioridad:** 🔴 Alta
* **Estimación:** 5 puntos

---

#### US-02 — Inicio y cierre de sesión
**Como** usuario registrado  
**Quiero** iniciar y cerrar sesión de forma segura  
**Para** proteger la privacidad de mi información y mis transacciones  

* **Criterios de Aceptación:**
  - El usuario ingresa su correo y contraseña registrados.
  - El sistema genera un token de autenticación (JWT) seguro al autenticar.
  - En caso de credenciales incorrectas, el sistema muestra un mensaje de error claro sin especificar cuál dato falló.
  - La opción de cierre de sesión invalida el token y regresa al usuario a la pantalla de bienvenida.
* **Prioridad:** 🔴 Alta
* **Estimación:** 3 puntos

---

#### US-03 — Recuperación de contraseña
**Como** usuario  
**Quiero** solicitar la recuperación de mi contraseña mediante mi correo  
**Para** restablecer el acceso a mi cuenta si llego a olvidarla  

* **Criterios de Aceptación:**
  - El usuario ingresa su correo en la opción "Olvidé mi contraseña".
  - El sistema envía un código o enlace con tiempo de expiración (15 minutos).
  - El usuario ingresa el código y define una nueva contraseña que cumpla con las políticas de seguridad.
* **Prioridad:** 🔴 Alta
* **Estimación:** 5 puntos

---

### Feature 1.2: Perfil Personal y Reputación

#### US-04 — Gestión del perfil personal
**Como** usuario registrado  
**Quiero** editar mi nombre, foto de perfil, biografía y ubicación  
**Para** personalizar mi presencia en la comunidad y generar confianza  

* **Criterios de Aceptación:**
  - El usuario puede subir o cambiar su foto de perfil desde la galería o cámara.
  - La ubicación permite definir ciudad/barrio de referencia para encuentros.
  - Los cambios se guardan e impactan de inmediato en la vista pública del perfil.
* **Prioridad:** 🔴 Alta
* **Estimación:** 3 puntos

---

## 📦 Épica 2: Publicación y Búsqueda de Prendas

### Feature 2.1: Gestión de Publicaciones

#### US-07 — Publicar una prenda
**Como** vendedor  
**Quiero** subir una prenda con fotos, título, descripción, precio, talla, estado y categoría  
**Para** ponerla a la venta en el catálogo  

* **Criterios de Aceptación:**
  - El formulario requiere al menos 1 foto obligatoria (máximo 5).
  - Se debe seleccionar una categoría predefinida (ej. Chaquetas, Camisetas, Pantalones).
  - Se debe definir el estado de la prenda (ej. Nuevo con etiqueta, Excelente estado, Usado).
  - El precio debe ser un número mayor a cero.
  - La prenda queda publicada en estado "Disponible".
* **Prioridad:** 🔴 Alta
* **Estimación:** 8 puntos

---

### Feature 2.2: Descubrimiento y Filtros

#### US-09 — Búsqueda y filtros avanzados
**Como** comprador  
**Quiero** buscar prendas por texto y filtrar por talla, precio, categoría y ubicación  
**Para** encontrar exactamente la ropa que me interesa  

* **Criterios de Aceptación:**
  - La barra de búsqueda realiza coincidencias por título y descripción.
  - Se pueden aplicar múltiples filtros simultáneamente.
  - Permite ordenar los resultados por: "Más reciente", "Menor precio" y "Mayor precio".
* **Prioridad:** 🔴 Alta
* **Estimación:** 8 puntos

---

#### US-10 — Detalle de la prenda
**Como** comprador  
**Quiero** ver la galería de imágenes completas y los detalles de la prenda  
**Para** evaluar la compra y conocer la información del vendedor  

* **Criterios de Aceptación:**
  - Muestra un carrusel interactivo con todas las fotos cargadas.
  - Muestra la información completa (talla, estado, descripción, precio, ubicación).
  - Muestra el perfil básico del vendedor y su reputación.
  - Incluye el botón principal "Quiero esta prenda".
* **Prioridad:** 🔴 Alta
* **Estimación:** 5 puntos

---

## 🤝 Épica 3: Compra, Venta y Comunicación

### Feature 3.1: Solicitudes de Compra y Estado

#### US-12 — Enviar y gestionar solicitud de compra
**Como** comprador  
**Quiero** enviar una solicitud de compra al vendedor sobre una prenda específica  
**Para** notificarle mi interés y coordinar la adquisición  

* **Criterios de Aceptación:**
  - El comprador presiona "Quiero esta prenda" para enviar la solicitud.
  - El vendedor recibe una notificación con la opción de "Aceptar" o "Rechazar".
  - Si el vendedor acepta, el estado de la prenda cambia automáticamente a "Reservada" y se habilita el canal de chat.
  - Si se rechaza, la prenda se mantiene "Disponible".
* **Prioridad:** 🔴 Alta
* **Estimación:** 8 puntos

---

### Feature 3.2: Chat y Comunicación

#### US-13 — Chat en tiempo real
**Como** usuario  
**Quiero** chatear en tiempo real con la contraparte de una transacción  
**Para** coordinar detalles de entrega, punto de encuentro o resolver dudas  

* **Criterios de Aceptación:**
  - El chat se habilita únicamente cuando existe una solicitud de compra aceptada o en proceso.
  - Los mensajes se entregan de forma instantánea.
  - Permite enviar texto y compartir ubicación de punto de encuentro.
  - Muestra el historial anterior de la conversación.
* **Prioridad:** 🔴 Alta
* **Estimación:** 8 puntos