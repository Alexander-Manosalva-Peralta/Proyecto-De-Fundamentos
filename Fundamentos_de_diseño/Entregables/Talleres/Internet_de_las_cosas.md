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

