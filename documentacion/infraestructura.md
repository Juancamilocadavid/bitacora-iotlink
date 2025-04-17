# Infraestructura de la Plataforma IoTLink

## Servidor principal
- **Dispositivo**: Raspberry Pi 4 (4GB RAM)
- **Sistema operativo**: Raspberry Pi OS Lite
- **Dominio**: iotlink.com.co
- **Conexión**: Red local con acceso DMZ desde el router

## Software instalado
- **ThingsBoard CE**: Plataforma principal de gestión IoT
- **Nginx**: Servidor proxy para redirección segura
- **Certbot**: Para generación y renovación automática de certificados SSL
- **Docker y Docker Compose**: Para facilitar despliegue de servicios adicionales

## Seguridad
- **Puerto expuesto**: 443 (HTTPS)
- **Protecciones activas**:
  - Fail2Ban
  - UFW configurado
  - Contraseñas robustas para todos los accesos

## Respaldo
- **Frecuencia**: Diario
- **Ubicación de backup**: Disco externo y Google Drive mediante rclone

## Monitoreo
- **Herramienta**: Netdata
- **Alertas configuradas**: Temperatura, uso de CPU/RAM, espacio en disco

## Plan de escalado
- Servidor secundario con balanceo de carga (futuro)
- Nodo MQTT replicado
- Dashboard replicado vía ThingsBoard en otro dispositivo o VPS
