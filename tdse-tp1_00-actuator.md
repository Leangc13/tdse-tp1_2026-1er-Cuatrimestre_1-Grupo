## Modelo Actuator

El módulo Actuator se encarga de ejecutar las acciones indicadas por el módulo System, controlando el comportamiento del LED, que representa la barrera, el cual posee 4 estados ON, OFF, PULSE y BLINK. Además, contempla comportamientos temporizados como pulsos y titilado mediante el uso de una variable de tiempo. Un  led, o diodo emisor de luz, es un dispositivo semiconductor que emite luz cuando se le aplica una corriente eléctrica. Un led  puede estar encendido , apagado, titilando O un pulso/pulsos(N). 

### Eventos entrada

EV_ACT_LED_ON  
EV_ACT_LED_OFF  

### Eventos salida

EV_LED_XX_ON  
EV_LED_XX_OFF 

### Estados

ST_ACT_LED_OFF  
ST_ACT_LED_ON  
ST_ACT_LED_BLINK  

### Atributo 

modelo botón timer => tick // 0, DEL_LED_XX_MAX

<img width="669" height="299" alt="image" src="https://github.com/user-attachments/assets/cf080dfa-e8f2-49fd-8c83-15664609a7f4" />



