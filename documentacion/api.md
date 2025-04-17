# Documentación - API de IoTLink

## Descripción
Este archivo describe las especificaciones de la API de IoTLink, que permite la comunicación entre el servidor, los dispositivos IoT y las aplicaciones de usuario.

---

## Endpoints Principales

### 1. **GET /api/devices**
   - **Descripción**: Obtiene la lista de dispositivos registrados en el sistema.
   - **Parámetros**: Ninguno
   - **Respuesta**: Lista de dispositivos con detalles (nombre, ID, estado).
   - **Ejemplo de respuesta**:
     ```json
     [
       {
         "id": "1",
         "name": "Sensor de Temperatura",
         "status": "activo"
       },
       {
         "id": "2",
         "name": "Sensor de Humedad",
         "status": "inactivo"
       }
     ]
     ```

### 2. **POST /api/devices**
   - **Descripción**: Registra un nuevo dispositivo en el sistema.
   - **Parámetros**:
     - `name`: Nombre del dispositivo.
     - `type`: Tipo de dispositivo.
   - **Respuesta**: Detalles del dispositivo registrado.
   - **Ejemplo de cuerpo de solicitud**:
     ```json
     {
       "name": "Sensor de Movimiento",
       "type": "sensor"
     }
     ```
   - **Ejemplo de respuesta**:
     ```json
     {
       "id": "3",
       "name": "Sensor de Movimiento",
       "status": "activo"
     }
     ```

### 3. **GET /api/notifications**
   - **Descripción**: Obtiene las notificaciones activas para el usuario.
   - **Parámetros**: Ninguno
   - **Respuesta**: Lista de notificaciones activas.
   - **Ejemplo de respuesta**:
     ```json
     [
       {
         "id": "101",
         "message": "Dispositivo Sensor de Temperatura está fuera de rango.",
         "status": "pendiente"
       }
     ]
     ```

---

## Autenticación
La API utiliza tokens JWT (JSON Web Token) para la autenticación. Se debe incluir el token en el encabezado de autorización de cada solicitud.

---

**📅 Última actualización:** Abril 2025
