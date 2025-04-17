# Utilidades de Desarrollo - IoTLink

## IDEs y Editores
- **Visual Studio Code**  
  - Extensiones: Remote - SSH, Docker, PlatformIO, Python, Markdown All in One
- **Arduino IDE 2.x**
- **Thonny (para Python en Raspberry Pi)**
- **Termux (para desarrollo Android sin entorno gráfico)**

## Lenguajes y versiones
- **Python**: 3.10
- **JavaScript**: ES6+
- **C/C++**: para desarrollo en ESP32
- **Bash**: para automatizaciones en Linux/Raspberry

## Librerías y herramientas clave
- **ESP-IDF y Arduino Core para ESP32**
- **OpenCV**: para visión artificial
- **MQTT** (PubSubClient en ESP y Mosquitto en servidor)
- **Node-RED** (para flujos locales de prueba)
- **Docker** (para contenedores de backend y ThingsBoard)
- **Nginx** (como proxy inverso con HTTPS)
- **Git** (seguimiento de código y versiones)

## Estructura de carpetas (por convención)
- `/firmware/`: código para microcontroladores
- `/scripts/`: automatizaciones en bash o python
- `/documentacion/`: todo lo relacionado a configuración y soporte
- `/dashboards/`: archivos exportados de dashboards de ThingsBoard
- `/backups/`: respaldos JSON de configuraciones

## Buenas prácticas
- Siempre documentar nuevas dependencias o comandos relevantes.
- Subir cambios con mensajes de commit claros.
- Preferir nombres en inglés para carpetas/código y español para la documentación.

