## Modelo System

El módulo System se encarga de procesar los eventos generados por el sensor (botón) y controlar el estado de la barrera.

En esta implementación simplificada, el sistema utiliza únicamente un pulsador como entrada y un LED como salida, representando la barrera.

### Eventos de entrada

EV_SYS_BTN_PRESSED  
EV_SYS_BTN_RELEASED  

Estos eventos son generados por el módulo Sensor.

### Acciones

EV_ACT_BARRIER_OPEN  
EV_ACT_BARRIER_CLOSE  

Estas acciones son enviadas al módulo Actuator, donde el LED representa el estado de la barrera.

### Estados

ST_SYS_IDLE  
ST_SYS_BARRIER_OPEN  

### Descripción del comportamiento

El sistema comienza en el estado ST_SYS_IDLE, con la barrera cerrada (LED apagado).

Cuando se recibe el evento EV_SYS_BTN_PRESSED, el sistema genera la acción de apertura de barrera y transiciona al estado ST_SYS_BARRIER_OPEN.

Cuando se recibe el evento EV_SYS_BTN_RELEASED, el sistema genera la acción de cierre de barrera y vuelve al estado inicial ST_SYS_IDLE.
