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
LECTURA DE TEMPERATURA

Para leer los valores del sensor de temperatura, incluimos una biblioteca específica llamada Arduino_MKRIoTCarrier.

#include <Arduino_MKRIoTCarrier.h>

La biblioteca muestra el sensor con el método llamado readTemperature() al que se puede llamar a través del objeto carrier que se construye y expone al inicializar la biblioteca.

Se puede acceder a todos los sensores del MKR IoT Carrier llamando a la línea de comando carrier.readSensor () donde readSensor () tiene que corresponder con el sensor real que se está verificando. En nuestro caso, es la temperatura, por lo que el método se llama readTemperature ().

### 3.2 Cambiar datos de Celsius, Fahrenheit y Kelvin

# Ejercicio de Conversión de Temperaturas en MKR IoT Carrier

En este ejercicio, se solicitó la visualización de las temperaturas en Fahrenheit, Celsius y Kelvin recopiladas por el sensor HTS221 (sensor de humedad y temperatura) en la pantalla del MKR IoT Carrier. Inicialmente, se implementaron líneas de código en Arduino para mostrar la temperatura solo en Celsius. La función inicial se presenta a continuación:

El objetivo del código es mostrar la temperatura y humedad en diferentes unidades (Celsius, Fahrenheit, Kelvin) en la pantalla del MKR IoT Carrier. Se implementaron funciones para cambiar entre unidades y mostrar la información en el formato deseado.

## Código Original

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

# Análisis del Código

## Inicialización y Lectura
En esta sección del código, se realizan las inicializaciones necesarias y se procede a la lectura de la temperatura y la humedad en el bucle principal (`loop()`). Las variables `temperature` y `humidity` se actualizan con los valores del sensor HTS221.

## Cambiar Unidad de Temperatura
La función `switchTemperatureUnit()` es responsable de cambiar la unidad de temperatura actual entre Celsius, Kelvin y Fahrenheit. Este cambio es activado al tocar el botón táctil `TOUCH0`.

## Mostrar Temperatura
La función `printTemperature()` se encarga de imprimir la temperatura en la pantalla del MKR IoT Carrier. Utiliza un `switch` para adaptar la visualización según la unidad seleccionada (Celsius, Kelvin o Fahrenheit). Se han definido variables adicionales como `temperatureF` y `temperatureK` para las conversiones entre unidades.

## Mostrar Humedad
La función `printHumidity()` imprime la humedad en un formato específico en la pantalla cuando se toca el botón `TOUCH1`.



### 3.3 Cambiar el nivel de temperatura


## 4. Conclusiones

