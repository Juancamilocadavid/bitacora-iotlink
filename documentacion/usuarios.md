# Documentación - Usuarios de IoTLink

## Descripción
Este archivo contiene la información relevante sobre los usuarios y sus roles dentro del sistema IoTLink, incluyendo las funciones asignadas a cada uno y los permisos del sistema.

---

## Roles de Usuario

### 1. **Administrador**
   - **Descripción**: Usuario con acceso total a todas las funcionalidades del sistema, incluyendo la gestión de dispositivos, usuarios y configuraciones avanzadas.
   - **Permisos**:
     - Gestionar usuarios
     - Acceder a todos los informes
     - Configurar y administrar dispositivos IoT
     - Realizar copias de seguridad del sistema

### 2. **Usuario Básico**
   - **Descripción**: Usuario con acceso limitado a la visualización de datos y dispositivos. No tiene permisos para modificar configuraciones del sistema.
   - **Permisos**:
     - Ver los datos de los dispositivos
     - Recibir alertas
     - Controlar dispositivos básicos (encender/apagar)

### 3. **Técnico**
   - **Descripción**: Usuario con permisos para acceder a la configuración de dispositivos IoT y gestionar alertas.
   - **Permisos**:
     - Ver y gestionar dispositivos IoT
     - Configurar alertas
     - Ver reportes de diagnóstico

### 4. **Invitado**
   - **Descripción**: Usuario con permisos muy limitados, únicamente para visualizar datos en tiempo real sin acceso a configuraciones.
   - **Permisos**:
     - Visualizar datos de dispositivos en tiempo real
     - Recibir notificaciones de alerta

---

## Proceso de Registro

### 1. **Registro de Usuario**
   - Los usuarios deben registrarse mediante un formulario con validación de correo electrónico.
   - Una vez registrado, se enviará un correo de confirmación para activar la cuenta.

### 2. **Asignación de Roles**
   - Los administradores asignan los roles a los usuarios al momento de su registro o después de la activación de la cuenta.
   - Los usuarios podrán ver sus permisos en su perfil.

---

## Seguridad

- **Autenticación**: Los usuarios deben iniciar sesión con credenciales únicas (correo y contraseña).
- **Autorización**: Los roles determinan los permisos del usuario dentro del sistema.
- **Cifrado**: Toda la información sensible es cifrada utilizando HTTPS y JWT.

---

**📅 Última actualización:** Abril 2025
