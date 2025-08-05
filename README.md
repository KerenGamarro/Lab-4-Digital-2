# Laboratorio 4 – Señales de PWM
Utilizando el microcontrolador ESP32, VS Code y PlatformIO
Este laboratorio consiste en que el estudiante, mediate el uso del entorno
PlatformIO, el framework de Arduino y el microcontrolador ESP32, practique la
configuración de señales PWM.
El objetivo de este laboratorio es realizar un sistema en el que mediante
pushbuttons y señales PWM puedan controlarte tanto la posición de un servo
motor como el brillo de un led RGB (configurando cada color de forma
independiente). Finalmente deberá implementarse una rutina en la que según la
posición del servo motor se defina el color del del RGB estará encendido.
# Materiales:
- 1 protoboard
- 1 microcontrolador ESP32
- 4 pushbuttons
- 1 servo motor
- 1 LED RGB (o 3 LEDs, uno rojo, uno verde y uno azul)
- Puntas de osciloscopio
#Parte A: Controlador LED RGB (40pts) – Entregable en Clase
Diseñe e implemente tres señales PWM para controlar un LED RGB o en su
defecto 3 leds de color Rojo, Verde y Azul utilizando dos botones.
El primer botón (B3) nos servirá para seleccionar cuál de los tres colores
queremos modificar. El segundo botón (B4) modificará el brillo del LED
seleccionado (mínimo 4 niveles de brillo distintos), al presionar debe aumentar el
brillo, cuando llegue al brillo máximo, si se vuelve a presionar empieza desde
apagado y se va incrementando de nuevo con cada vez que se presione el botón.
Botón B3 Operación
1 Cambio de brillo LED Rojo
2 Cambio de brillo LED Verde
3 Cambio de brillo LED Azul

# Parte B: Controlador Servo Motor (30pts)
Implemente una señal PWM para controlar un servomotor utilizando dos botones.
El primero botón (B1) servirá para mover el motor hacia la derecha y el botón (B2)
servirá para mover el motor hacia la izquierda. El motor debe tener 5 posiciones
distintas (como se muestra en la siguiente imagen) y si el motor ya se encuentra
en alguno de los extremos y se presiona el botón correspondiente a ese extremo
este debe permanecer en la misma posición. REVISAR que el servo motor esté bien
conectado y no haga ruidos raros
Funcionamiento de Servo Motor

# Parte C: Rutina de Integración (30pts)
Implemente una rutina la cual se seleccione con el mismo botón (B3), en donde
dependiendo de la posición del servo, cambie el color del LED RGB, como se
muestra en la siguiente figura. (en las 2 posiciones de los extremos todos los
colores deben permanecer apagados).
