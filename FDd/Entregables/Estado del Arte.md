# Estado del Arte

## 💡 Contexto Científico

### 📚 Artículos Originales (3)
| #   | Título del Artículo                 | Detalles                                      | Enlace                                 |
| --- | ----------------------------------- | --------------------------------------------- | ---------------------------------------|
| 1   | Diseño Innovador                    | [Aquí](#diseno-innovador)                     | [Enlace al Artículo 1](https://pubmed.ncbi.nlm.nih.gov/35729914/) |
| 2   | Ensayos Clínicos                    | [Aquí](#ensayos-clinicos)                     | [Enlace al Artículo 1](URL_Articulo_1) |
| 3   | Revisiones Sistemáticas             | [Aquí](#revisiones-sistematicas)              | [Enlace al Artículo 1](URL_Articulo_1) |

## Diseño Innovador <a name="diseno-innovador"></a>

##  Diseño y análisis de un sistema de filtración y monitoreo de la calidad del agua para diferentes tipos de agua en Malasia.

Este artículo describe un proyecto destinado a abordar la contaminación del agua en Malasia mediante el desarrollo de un sistema de monitoreo y filtración de la calidad del agua controlado por Arduino. Se enfoca en la detección temprana de agua contaminada, especialmente en ríos, debido a actividades industriales, de construcción, agrícolas y domésticas.
El sistema, diseñado en Proteus y utilizando ThingSpeak para el monitoreo en tiempo real, mide parámetros como pH, temperatura, turbidez, conductividad eléctrica y potencial de oxidación-reducción. Si se detecta una calidad del agua insatisfactoria, la muestra se filtra a través del sistema de filtración.

<img src="../../Carpetas/Imagenes/Articulo1.png" alt="Texto Alternativo" width="500" height="300">

**Fuente:** Razman, N. A., Wan Ismail, W. Z., Abd Razak, M. H., Ismail, I., & Jamaludin, J. (2023). Design and analysis of water quality monitoring and filtration system for different types of water in Malaysia. *International Journal of Environmental Science and Technology: IJEST*, 20(4), 3789-3800. [https://doi.org/10.1007/s13762-022-04192-x](https://doi.org/10.1007/s13762-022-04192-x)

## Ensayos Clínicos <a name="ensayos-clinicos"></a>

## Intervenciones para mejorar la calidad del agua para prevenir la diarrea.

En este presente artículo se habla sobre la diarrea como una de las  problemáticas  graves especialmente en los países de bajos ingresos económicos, donde pueden provocar enfermedades incluso la muerte, especialmente en los niños. Muchos agentes infecciosos que causan diarrea se transmiten a través del agua contaminada en zonas remotas y empobrecidas, donde se pueden tomar medidas para mejorar la calidad del agua. Estas incluyen el uso de agua subterráneas o agua de lluvia recolectada en lugar de fuentes superficiales. También se puede llevar a cabo medidas de mejora de la calidad de agua en el punto de uso, como hervirla, clorarla, filtrar o desinfectarla. Estos procedimientos se realizan principalmente en los hogares (Clasen et al., 2015).

<img src="../../Carpetas/Imagenes/Prevenir.png" alt="Texto Alternativo" width="500" height="300">

**Fuente:** Colocar su fuente

## Revisiones Sistemáticas <a name="revisiones-sistematicas"></a>

## Sistema de monitoreo de calidad del agua basado en IOT.

Este artículo describe un dispositivo de interfaz de sensor reconfigurable para la monitorización de la calidad del agua con el entorno Iot para el desarrollo de un sistema inteligente de monitorización de la calidad del agua, de los cuales los parámetros que más me interesaron fueron el sensor de turbidez, que tiene la finalidad de detectar la calidad del agua midiendo el nivel de turbidez, así como la detección de partículas  en suspensión mediante la medición de la transmitancia de luz y los modos de salida de señal analógica y digital y también otro de los parámetro interesantes es el sensor de PH, que tiene la función de detectar el valor del PH de agua. Estas variables propuestas pueden ayudar a proteger el entorno ecológico de los recursos hídricos así como minimizar el tiempo y los costos en la detección de la calidad del agua de un embalse como parte de la gestión medioambiental. (Konde & Deosarkar, 2020).

<img src="../../Carpetas/Imagenes/Basado.png" alt="Texto Alternativo" width="500" height="300">

**Fuente:** Colocar su fuente

## 🌐 Contexto Comercial

### 🚀 Equipos o Dispositivos en el Mercado (3)
| #   | Producto                          | Enlace                                     |
| --- | ----------------------------------| ------------------------------------------ |
| 1   | Innovador Producto X              | [Enlace al Producto 1](URL_Producto_1)    |
| 2   | Avanzado Producto Y               | [Enlace al Producto 2](URL_Producto_2)    |
| 3   | Vanguardista Producto Z            | [Enlace al Producto 3](URL_Producto_3)    |

### 🛡️ Patentes (3)
| #   | Patente                          | Enlace                                 |
| --- | ---------------------------------| -------------------------------------- |
| 1   | Patente A                        | [Enlace a la Patente 1](URL_Patente_1) |
| 2   | Patente B                        | [Enlace a la Patente 2](URL_Patente_2) |
| 3   | Patente C                        | [Enlace a la Patente 3](URL_Patente_3) |

# Lista de Requerimientos

| Requerimientos Funcionales ✔️                 | Requerimientos No Funcionales ⚙️              |
| ---------------------------------------------| ---------------------------------------------|
| **Sensores de turbidez:** El sistema debe ser capaz de clasificar los niveles de turbidez en categorías como alto, bajo y apto para el consumo humano.El sistema debe ser capaz de clasificar los niveles de turbidez en categorías como alto, bajo y apto para el consumo humano.| **Fiabilidad:** El sistema debe ser altamente confiable, asegurando mediciones precisas y acciones correctas en todo momento.|
| **Un mecanismo, controlado por Arduino, para dirigir el flujo de agua:** Para dirigir el flujo de agua hacia tanques específicos según el nivel de turbidez detectado. | **Escalabilidad:** La arquitectura del sistema debe ser escalable para permitir futuras expansiones o mejoras.  |
| **Redirección Automática:** El sistema debe ser capaz de redirigir automáticamente el agua recolectada hacia un tanque adecuado para su uso (riego, consumo humano) según los resultados de la medición de turbidez.    | **Adaptabilidad:** El sistema debe ser capaz de adaptarse a cambios en las condiciones ambientales y de agua.  |
| **Eficiencia Energética:** El sistema debe ser eficiente en cuanto al consumo de energía para garantizar un funcionamiento sostenible, considerando la disponibilidad de energía en la ubicación.  | **Sostenibilidad:** El sistema debe ser diseñado para ser respetuoso con el medio ambiente y sostenible en términos de recursos y energía.|
| **Almacenamiento de Datos:** Implementar un sistema de almacenamiento de datos para registrar históricos de las mediciones de turbidez y la asignación de agua a lo largo del tiempo.    | **Accesibilidad:** La página web debe ser accesible desde diferentes dispositivos y navegadores para facilitar el acceso a la información a los usuarios. |
| **Notificaciones:** El sistema debe ser capaz de enviar notificaciones, ya sea por la página web o por otros medios, para informar a los usuarios sobre cambios significativos o problemas en el sistema.    | **Mantenimiento:** El sistema debe ser de fácil mantenimiento, con la capacidad de realizar actualizaciones y correcciones de manera eficiente.  
|**Interfaz de Usuario Intuitiva:** La interfaz de usuario en la página web debe ser intuitiva y fácil de entender para que los habitantes del lugar puedan verificar el estado del agua y las acciones realizadas.    |
**Compatibilidad con Energía Renovable:** Evaluar la posibilidad de utilizar energía renovable, como paneles solares, para alimentar el sistema y garantizar su funcionamiento continuo.


