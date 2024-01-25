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

```cpp
void printTemperature() {
  // Configura la pantalla, establece el color de fondo, el tamaño del texto y el color del texto
  carrier.display.fillScreen(ST77XX_RED); // fondo rojo
  carrier.display.setTextColor(ST77XX_WHITE); // texto blanco
  carrier.display.setTextSize(6); // texto grande

  carrier.display.setCursor(30, 50); // posición para imprimir (x y)
  carrier.display.print("Temp: ");
  carrier.display.setTextSize(4); // disminuye el tamaño del texto
  carrier.display.setCursor(40, 120); // nueva posición para imprimir (x y)
  carrier.display.print(temperature);
  carrier.display.print(" C");
}

// Función para mostrar la temperatura en Celsius
void showTemperatureCelsius() {
  // Implementación para mostrar temperatura en Celsius
}

// Función para mostrar la temperatura en Fahrenheit
void showTemperatureFahrenheit() {
  // Implementación para mostrar temperatura en Fahrenheit
}

// Función para mostrar la temperatura en Kelvin
void showTemperatureKelvin() {
  // Implementación para mostrar temperatura en Kelvin
}

// Resto de funciones para mostrar la humedad y otras escalas de temperatura


### 3.3 Cambiar el nivel de temperatura


## 4. Conclusiones

