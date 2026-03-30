## Modelo System

El módulo System se encarga de procesar los eventos generados por el sensor (botón) y envia la accion a tomar por el módulo del Actuador. En esta implementación simplificada, el sistema utiliza únicamente un pulsador como entrada y un LED como salida, representando la barrera.

### Eventos de entrada

EV_SYS_XX_DOWN  
EV_SYS_XX_UP

Estos eventos son generados por el módulo Sensor.

### Acciones

EV_ACT_LED_ON  
EV_ACT_LED_OFF  

### Estados

ST_SYS_LED_ON  
ST_SYS_LED_OFF  

### Descripción del comportamiento

El sistema comienza en el estado ST_SYS_LED_OFF, con la barrera cerrada (LED apagado).Cuando se recibe el evento EV_SYS_BTN_DOWN, el sistema genera la acción de apertura de barrera y transiciona al estado ST_SYS_LED_ON.Cuando se recibe el evento EV_SYS_BTN_UP, el sistema genera la acción de cierre de barrera y vuelve al estado inicial ST_SYS_LED_OFF.
