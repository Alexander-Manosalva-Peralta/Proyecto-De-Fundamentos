<img width="600" height="200" src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/4cccbe2c-22fd-438e-b736-262de9138cef" alt="Descripción de la imagen">

 ## 1. INTRODUCCION 

Los circuitos electrónicos constituyen la columna vertebral de la tecnología moderna, abarcando desde dispositivos simples como interruptores de luz hasta complejos sistemas informáticos. Estos circuitos, compuestos por componentes electrónicos interconectados, permiten el flujo de corriente eléctrica para desempeñar funciones específicas.

Importancia del Esquemático del Circuito Electrónico: Un diagrama esquemático de un circuito electrónico es esencial ya que proporciona una representación visual clara de cómo están interconectados los componentes en un circuito. Esta representación gráfica facilita la comprensión del diseño del circuito, permitiendo a ingenieros y técnicos visualizar rápidamente la disposición y conexión de los componentes.

## 2. EJERCICIOS REALIZADOS EN CLASE

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


## Vista Preliminar en 2D

![image](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023044/3688da89-cf1d-49c4-acfc-04278941dd4c)



![image](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023044/daaaf17d-262f-447c-a424-eb67f7dc6e59)


Su función primordial es activar un Led mediante un botón o pulsador, desempeñando un papel esencial en el logro de nuestros objetivos. Se ha asegurado una integración perfecta con la arquitectura general del proyecto, garantizando una sinergia fluida entre todos los componentes. Además, se ha prestado especial atención a la adaptabilidad de los componentes, lo que permite llevar a cabo la esquematización del circuito.

## Vista Preliminar en 3D

![image](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023044/0f390dc2-8f39-4de1-9d3a-83808c4f75fc)

Sistema en vista 3D del circuito en PCB (Bottom)


![image](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023044/bafb537a-22b0-4a66-9530-8568e108fdb4)

Sistema en vista 3D del circuito en PCB (Bottom)


![image](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023044/166c220e-e1fe-47a6-9568-aa46af153c9e)

Sistema en vista 3D del circuito en PCB (Bottom)



En esta sección se muestra el modelado 3D de nuestro circuito, es decir, como esta compuesto cada uno de los componentes de manera tridimensional, tanto en el TOP como en la parte BOTTOM el todo el circuito electrónico.


## Visualización en Flux.ai

https://www.flux.ai/michaelgavino/upper-cyan-ecto-goggles?editor=pcb_3d


## 3. CONCLUSIÓN:

Finalmente en el presente taller desarrollamos y experimentamos nuevas habilidades de formar  circuitos en la plataforma de Flux.ai, que nos proporciono el conocimiento nesesario para armar nuestro circuito. Al integrar un Arduino MKR WiFi 1010 con componentes como un botón pulsador, un LED, resistencias, y la pantalla para armar un circuito que controla y visualiza el estado de los leds, esto es una gran ayuda al momento de eimplemetar en nuestro proyecto junto a sensores adicionales para medir el pH, la turbidez y la conductividad eléctrica, se puede crear un proyecto aún más completo y sofisticado. Esta combinación de componentes permite monitorear y controlar no solo aspectos físicos como el estado de cada leds. Asimismo podemos controlar los parametros físicos del agua como el pH, la turbidez y la conductividad eléctrica y poder clasificar de acuerdo al nivel establecido de los estandares del agua para uso cotidiano.

