El sensor será representado con un botón el cual posee 4 estados UP, DOWN, Falling, y Rising. Además cuenta con una variable contadora
llamada timer.
Un Sensor (un solo botón) del tipo binario genera 2 (dos) Eventos (reflejan el valor binario) asociados a su Posición y
al menos 2 (dos) Acciones (reflejan que hubo un cambio de Posición del botón)
Las Acciones del modelo Sensor pueden ser signals (Eventos) para el modelo System o bien ejecutar funciones o
bien “inicialización/modificación” de variables de control (timer); variables que pueden usarse como guard para condicionar
transiciones (trigger [guard] / effect).

Convención de identificadores

Hay 2 eventos entrada:  
event => EV_BTN_XX_UP  
event => EV_BTN_XX_DOWN  

Hay 4 estados  
state => ST_BTN_XX_UP  
state => ST_BTN_XX_DOWN  
state => ST_BTN_XX_FALLING  
state => ST_BTN_XX_RISING  

Hay dos eventos de salida:  
signal => EV_SYS_XX_DOWN  
signal => EV_SYS_XX_UP  

Un atributo de modelo botón
timer => tick // 0, DEL_BTN_XX_MAX

<img width="700" alt="sensor statechart-state_transition_table" src="https://github.com/user-attachments/assets/6d5bab14-7788-400c-b6ff-96798d80daba" />


