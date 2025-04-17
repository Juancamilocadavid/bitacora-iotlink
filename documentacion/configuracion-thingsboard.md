# Configuración de ThingsBoard en IoTLink

## Instalación
- **Método**: Docker Compose
- **Repositorio base**: [thingsboard/thingsboard](https://github.com/thingsboard/thingsboard)
- **Versión instalada**: CE (Community Edition)

## Variables de entorno utilizadas
```env
TB_QUEUE_TYPE=in-memory
DATABASE_TS_TYPE=sql


Puerto de acceso
Local: http://localhost:8080

Redireccionado por Nginx a: https://iotlink.com.co

Usuarios creados
Admin: admin@iotlink.com.co

Integrador: integrador@iotlink.com.co

Lectura: usuario@iotlink.com.co

Configuraciones clave
Dashboard principal: "IoTLink Overview"

Tokens JWT activos: 3

Integración con nodos ESP32 mediante MQTT

Seguridad
Acceso limitado por IP

Autenticación en 2 pasos pendiente de implementación

Acceso por dominio HTTPS con certificado Let’s Encrypt

Respaldos
Configuraciones exportadas semanalmente en JSON

Ubicación local: /backups/thingsboard/

Frecuencia: semanal (script programado en cron)

Personalización pendiente
Cambiar logotipo y nombre de empresa en plataforma

Agregar manual del usuario y enlaces útiles en el dashboard

Completada configuracion de thingsboard
