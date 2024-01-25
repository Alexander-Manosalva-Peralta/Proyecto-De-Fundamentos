## INFORME 3: 

# Resolución del laboratorio de manejo de IoT el internet de las cosas: Fundamentos de Diseño

## 1. INTRODUCCIÓN

Imagen
 
**Fuente si es que hay**

## 2. PROCEDIMIENTO
### 2.1 Características y componentes de Internet de las cosas (IoT)
### 2.2 Pones lo demás
### 2.3 Colocas lo demás y sigues aumentando si hay más

## 3. Ejercicios
### 3.1 Ejecutar el código de la sección "Conoce el kit"


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

