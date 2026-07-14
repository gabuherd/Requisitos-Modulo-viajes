# Requisitos Módulo Viajes

## Requisitos No Funcionales

* **Seguridad:** Encriptación de datos de extremo a extremo utilizando protocolo HTTPS/TLS (Cifrado SSL) para evitar la filtración o robo de información de los usuarios.
* **Rendimiento y Concurrencia:** La aplicación debe soportar una carga simultánea de al menos 1,000 personas al mismo tiempo sin trabarse.
* **Actualizaciones en Tiempo Real:** Latencia de red mínima para la actualización de geolocalización de los choferes y viajes cercanos.

## Historias de Usuario (US)

### US-01: Visualización de Viajes Cercanos en Tiempo Real
* **COMO:** Chofer de la aplicación.
* **QUIERO:** Ver las solicitudes de viajes que se encuentran cerca de mi ubicación actual en tiempo real.
* **PARA:** Poder seleccionar y aceptar servicios de manera rápida y eficiente.

#### Criterios de Aceptación (Gherkin):
* Dado que el chofer ha iniciado sesión y tiene activa su ubicación GPS
* Cuando ingresa a la pantalla principal de solicitudes
* Entonces el sistema debe mostrar un mapa con los viajes disponibles dentro de un radio cercano en tiempo real.

### US-02: Cálculo de la Ruta Óptima al Aceptar un Viaje
* **COMO:** Chofer de la aplicación.
* **QUIERO:** Que si acepto un servicio, la aplicación me diga la ruta más corta hacia el destino de manera automática.
* **PARA:** No gastar gas de forma innecesaria y optimizar el tiempo del viaje.

#### Criterios de Aceptación (Gherkin):
* Dado que el chofer visualiza una solicitud de viaje en la pantalla
* Cuando el chofer presiona el botón "Aceptar Viaje"
* Entonces el sistema debe trazar y mostrar en pantalla la ruta vial más corta y eficiente. mapa con los viajes disponibles dentro dA