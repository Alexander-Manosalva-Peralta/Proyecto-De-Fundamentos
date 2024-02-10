<img width="600" height="200" src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/4cccbe2c-22fd-438e-b736-262de9138cef" alt="Descripción de la imagen">

## INTRODUCCION 

Los circuitos electrónicos constituyen la columna vertebral de la tecnología moderna, abarcando desde dispositivos simples como interruptores de luz hasta complejos sistemas informáticos. Estos circuitos, compuestos por componentes electrónicos interconectados, permiten el flujo de corriente eléctrica para desempeñar funciones específicas.

## Importancia del Esquemático del Circuito Electrónico

Un diagrama esquemático de un circuito electrónico es esencial ya que proporciona una representación visual clara de cómo están interconectados los componentes en un circuito. Esta representación gráfica facilita la comprensión del diseño del circuito, permitiendo a ingenieros y técnicos visualizar rápidamente la disposición y conexión de los componentes.

## Ejercicio 1: Creación de un Sistema para Encender un LED

Para conectar un Arduino MKR WiFi 1010 con un botón pulsador y tierra (Ground), seguimos los siguientes pasos:

1. Seleccionamos un Arduino MKR WiFi 1010, Push Button y Ground.

<img src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/blob/main/Imagenes/tierra.png" alt="Vista Previa en 2D" style="height: 200px;"> <img src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/blob/main/Imagenes/boton.png" alt="Vista Previa en 2D" style="height: 200px;"> <img src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/blob/main/Imagenes/ArduinoMKR.png" alt="Vista Previa en 2D" style="height: 200px;">

2. Conectamos un extremo del botón pulsador a un pin digital del Arduino MKR WiFi 1010 y el otro extremo a tierra (Ground).

3. Nos aseguramos de que el pin digital del Arduino esté configurado como entrada.

4. Conectamos el Arduino MKR WiFi 1010 a la computadora mediante un cable USB.

<img src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/blob/main/Imagenes/Cir_boton.png">

Una vez realizadas las conexiones, podemos visualizar el proyecto en una vista previa en 2D para luego mejorarla y verla en 3D.

<img src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/blob/main/Imagenes/Placa.png">

Finalmente, en una vista 3D, podemos apreciar que nuestro circuito está correctamente ejecutado.


## EJERCICIO 2 :  

## ELABORACIÓN DE UN ESQUEMÁTICO DEL CIRCUITO ELECTRÓNICO BASADO EN NUESTRO PROYECTO

En esta sección el docente a cargo nos solicitó implementar como mínimo 6 componentes para armar nuestro circuito electrónico, para ello iniciamos  diseñando circuitos para complementar y potenciar los objetivos de nuestro proyecto principal.

Para la construcción de este circuito, hemos seleccionado cuidadosamente los siguientes componentes, cada uno desempeñando un papel importante en el funcionamiento del sistema: 

## Arduino MKR Wifi 1010 (U1): 
Este es el microcontrolador que actúa como el cerebro de tu circuito. Lee las entradas, como el estado del botón, procesa esta información y controla las salidas, como el estado de los LED o los mensajes en la pantalla LCD, en función de la programación que realiza en él.

## LED rojo (LED1, LED2): 
Estos son diodos emisores de luz que emiten luz roja cuando se les aplica un voltaje. En tu circuito, estarán controlados por el Arduino y se pueden encender o apagar dependiendo del estado del botón. Su estado (encendido o apagado) también se muestra en la pantalla LCD.

## Resistencias (R1, R2): 
Su objetivo principal es limitar la cantidad de corriente que fluye a los LED para evitar que se quemen.

## Pantalla LCD LM016L:
Esta pantalla mostrará el estado de los LED (encendido o apagado). Además está controlado por el Arduino y se actualiza cuando cambia el estado del LED.

## Botón:  
Este componente proporciona una entrada al usuario para controlar el comportamiento del circuito. Se utilizó para encender o apagar los LED.

Seguidamente pasamos a ensamblar estos componentes en el circuito, durante el proceso prestamos mucha atención a la calidad de las conexiones eléctricas, evitando falsos contactos que puedan afectar el rendimiento del sistema. Quedando el circuito de la siguiente manera:


Vista Preliminar en 2D







## EVIDENCIAS DEL DESARROLLO

<img width="600" height="500" src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/8b168c86-5ec3-4f8b-8740-34a0810c1bfa" alt="Descripción de la imagen">

## CONCLUSIÓN:

Finalmente, al integrar un Arduino MKR WiFi 1010 con componentes como un botón pulsador, un LED, un sensor de temperatura, un sensor de luz y un servomotor, junto con sensores adicionales para medir el pH, la turbidez y la conductividad eléctrica, se puede crear un proyecto aún más completo y sofisticado. Esta combinación de componentes permite monitorear y controlar no solo aspectos físicos como la temperatura y la luz, sino también parámetros químicos y físicos del entorno como el pH, la turbidez y la conductividad eléctrica. 

