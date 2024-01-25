## INFORME 3: 

# Resolución del laboratorio de manejo de IoT el internet de las cosas: Fundamentos de Diseño

## 1. INTRODUCCIÓN
 En el presente informe se dará a conocer lo que se desarrolló en el laboratorio N° 04, Donde se usó el kit de Arduino IoT. En esta sección, conoceremos el Arduino MKR WIFI 1010, el Arduino Web Editor y la MKR IoT Carrier. Además, se realizaron algunos proyectos básicos como medir la temperatura, la humedad y la visualización de datos. En este proyecto aprenderemos cómo registrar la temperatura y la humedad con la ayuda del sensor HTS221 lo cual está incluido en el MKR IoT Carrier. Los códigos se editan en el Arduino Web Editor, así como en el Arduino IDE, estos datos registrados se envían del ordenador al Arduino a través del puerto serial y se ejecuta el programa, pero también los datos se muestran en la pantalla del ordenador. El programa ejecutado se puede ver su funcionalidad en la pantalla donde muestra los resultados, por ejemplo, los colores y temperatura, estos resultados se pueden controlar cambiando los códigos de ejecución y utilizando los botones capacitivos que están conectados al MKR IoT Carrier.

Imagen
 
**Fuente si es que hay**

## 2. PROCEDIMIENTO
### 2.1 Características y componentes de Internet de las cosas (IoT)
### 2.2 Pones lo demás
### 2.3 Colocas lo demás y sigues aumentando si hay más

## 3. Ejercicios
### 3.1 Ejecutar el código de la sección "Conoce el kit"
**LECTURA DE TEMPERATURA** 

Para leer los valores del sensor de temperatura, incluimos una biblioteca específica llamada Arduino_MKRIoTCarrier.
El rango de temperatura oscila entre -40 y +120 (° C) y la precisión es de ± 0,5 ° C en el rango de 15 a +40 ° C.

**LECTURA DE HUMEDAD** 

La medida de humedad hecha de esta manera es el resultado de la presión y la temperatura del agua. Para ello utilizamos el método llamado  `readHumidity ()`  que devuelve la humedad en porcentaje. El rango de humedad oscila entre ± 3.5% rH (humedad relativa), a 20 (°C) y +80% rH. La sensibilidad de la rH es de 0.004% rH.

**VISUALIZACIÓN Y CONSTRUCCIÓN DEL CODIGO**

Incluimos una biblioteca específica llamada `Arduino_MKRIoTCarrier. ` 
Se declaran variables de temperatura y humedad. 
La función setup, se inicia con una velocidad de 9600, se configura la variable CARRIER_CASE que podemos cambiarlo por true para indicar que usa la capsula.

```cpp
#include <Arduino_MKRIoTCarrier.h>
MKRIoTCarrier carrier;

float temperature = 0;
float humidity = 0;

void setup() {

  Serial.begin(9600);
  CARRIER_CASE = false;

  carrier.begin();
}
```
En la función `loop()`, se leen los valores de temperatura y humedad del sensor, además se actualizan los botones táctiles con `carrier.Buttons.update()`.
Se verifica si se ha tocado alguno de los botones táctiles (TOUCH0 o TOUCH1) y se llama a la función correspondiente.

```cpp
void loop() {
  // Lee los valores del sensor de temperatura y humedad
  temperature = carrier.Env.readTemperature();
  humidity = carrier.Env.readHumidity();

  // Actualiza los botones táctiles
  carrier.Buttons.update();

  // Imprime cada uno de los valores del sensor en el monitor serial
  Serial.print("Temperature = ");
  Serial.print(temperature);
  Serial.println(" °C");

  Serial.print("Humidity = ");
  Serial.print(humidity);
  Serial.println(" %");

  // Funciones para imprimir los valores en la pantalla táctil al tocar los botones
  if (carrier.Buttons.onTouchDown(TOUCH0)) {
    printTemperature();
  }

  if (carrier.Buttons.onTouchDown(TOUCH1)) {
    printHumidity();
  }
}
```


`printTemperature()`  esta configurada para que la pantalla pueda mostrar la temperatura en un fondo rojo y texto blanco. Luego imprime el valor de la temperatura en la pantalla.
`printHumidity()` configura la pantalla para mostrar la humedad en un fondo azul y texto blanco. Luego imprime el valor de la humedad en la pantalla.
```cpp
void printTemperature() {
  // Configuración de la pantalla: fondo rojo, texto blanco, tamaño de texto grande
  carrier.display.fillScreen(ST77XX_RED);
  carrier.display.setTextColor(ST77XX_WHITE);
  carrier.display.setTextSize(6);

  // Posiciona el cursor y imprime la temperatura en la pantalla
  carrier.display.setCursor(30, 50);
  carrier.display.print("Temp: ");
  carrier.display.setTextSize(4);
  carrier.display.setCursor(40, 120);
  carrier.display.print(temperature);
  carrier.display.print(" C");
}

void printHumidity() {
  // Configuración de la pantalla: fondo azul, texto blanco, tamaño de texto mediano
  carrier.display.fillScreen(ST77XX_BLUE);
  carrier.display.setTextColor(ST77XX_WHITE);
  carrier.display.setTextSize(2);

  // Posiciona el cursor y imprime la humedad en la pantalla
  carrier.display.setCursor(20, 110);
  carrier.display.print("Humi: ");
  carrier.display.print(humidity);
  carrier.display.println(" %");
}
```

![temperatura.jpg](https://1drv.ms/i/s!ApQ0BTGQNUaJoxmsdzf-5Bt441Gk?e=ySSb5D)

### 3.2 Cambiar datos de Celsius, Fahrenheit y Kelvin

En este ejercicio, se solicitó la visualización de las temperaturas en Fahrenheit, Celsius y Kelvin recopiladas por el sensor HTS221 (sensor de humedad y temperatura) en la pantalla del MKR IoT Carrier al precionar uno de los touch, en este caso nosotros utilizamos el touch0. Inicialmente, se implementaron líneas de código en Arduino para mostrar la temperatura solo en Celsius. La función inicial se presenta a continuación:

### *Código*

```cpp
#include <AirQualityClass.h>
#include <Arduino_MKRIoTCarrier.h>
// Otras librerías incluidas...

MKRIoTCarrier carrier;
float temperature = 0;
float humidity = 0;
enum TemperatureUnit { UNIT_CELSIUS, UNIT_KELVIN, UNIT_FAHRENHEIT };
TemperatureUnit currentUnit = UNIT_CELSIUS;

void setup() {
  // Inicializaciones...
}

void loop() {
  temperature = carrier.Env.readTemperature();
  humidity = carrier.Env.readHumidity();
  carrier.Buttons.update();

  // Lectura y procesamiento de la temperatura y humedad...

  if (carrier.Buttons.onTouchDown(TOUCH0)) {
    switchTemperatureUnit();
    printTemperature();
    printGroupMessageWithDesign();
  }

  if (carrier.Buttons.onTouchDown(TOUCH1)) {
    printHumidity();
  }
}

void switchTemperatureUnit() {
  // Cambio de la unidad de temperatura actual...
}

void printTemperature() {
  // Impresión de la temperatura en la pantalla...
}

void printHumidity() {
  // Impresión de la humedad en la pantalla...
}

void printGroupMessageWithDesign() {
  // Mostrar mensaje "Grupo 9" con diseño específico...
}
```
|   **Análisis del Código**   | **Cambiar unidad de temperatura** | **Mostrar Temperatura** | **Mostrar Mensaje con Diseño** |
|--------------------------|----------------------------------|--------------------------|--------------------------------|
| En esta sección del código, se realizan las inicializaciones necesarias y se procede a la lectura de la temperatura y la humedad en el bucle principal (`loop()`). Las variables `temperature` y `humidity` se actualizan con los valores del sensor HTS221. | La función `switchTemperatureUnit()` es responsable de cambiar la unidad de temperatura actual entre Celsius, Kelvin y Fahrenheit. Este cambio se activa al tocar el botón táctil `TOUCH0`. | La función `printTemperature()` se encarga de imprimir la temperatura en la pantalla del MKR IoT Carrier. Utiliza un `switch` para adaptar la visualización según la unidad seleccionada (Celsius, Kelvin o Fahrenheit). Se han definido variables adicionales como `temperatureF` y `temperatureK` para las conversiones entre unidades. | `printGroupMessageWithDesign()` muestra el mensaje "Grupo 9" con un diseño específico en la pantalla al tocar `TOUCH0`. |

[![Mi Video](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/raw/main/Imagenes/mi_video_thumbnail.png)](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/raw/main/Imagenes/mi_video.mp4)

### 3.3 Cambiar el nivel de temperatura

Al verificar la función de arduino, decidimos seguir los pasos de la guía Explore loT para cambiar el nivel de la temperatura, el programa detectó la diferencia de nivel usando cambios de colores led integradas mostrando color rojo y verde dependiendo de la temperatura que mantenga el ambiente. 
EL código que se colocó fue la siguiente:

Void loop() {
    // read the sensor values
    temperatura = carrier.Env. readHumidity();

    //update touch buttons
    carrier.Buttons.update();
    //print each of the sensor value
    serial.print("temperatura = ");
    serial.print(temperatura);
    serial.print("A ° C");

    Serial.print("Humidity= ");
    serial.print(humidity);
    serial.println(" % ")

    //function to print out values
    if (carrier.Buttons.onTouchDown(TOUCH0)) {
        print Temperature();

    )
Al verificar el código se subió al arduino para que nos de valores de la temperatura, como se puede observar en las dos imágenes son diferentes colores lo cual nos dice si es frio o calor.


## 4. Conclusiones

