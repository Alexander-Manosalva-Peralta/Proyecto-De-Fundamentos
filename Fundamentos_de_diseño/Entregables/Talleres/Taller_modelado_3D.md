## INFORME DE LABORATORIO N.º 05: DISEÑO 3D


## 1. Introducción

En el presente informe de nuestro laboratorio sobre impresiones 3D, exploraremos las capacidades y aplicaciones prácticas de la impresión 3D. El objetivo principal de este laboratorio fue recibir información para una comprensión práctica de cómo utilizar la tecnología de impresión 3D y explorar sus aplicaciones en el mundo real. Durante la sesión, nos enfocamos en comprender los procesos de diseño, configuración de impresión y los resultados obtenidos. Comenzamos en el diseño tridimensional mediante el uso de software Onshape. Aprendimos a crear modelos digitales, considerando aspectos como la geometría, la resolución y la estructura de soporte para garantizar que las impresiones sean exitosas. En Onshape los colores proporcionan una guía útil facilitando e identificando los ajustes necesarios que se necesita, en el caso del color rojo, resalta que las medidas geométricas no esta correcto en nuestro diseño, si bien en el color azul las medidas geométricas están bien construidas no se encuentran bien definidas y el color negro indica que las medidas y la geometría está bien definida por podemos seguir con el moldeado de nuestro diseño. Una vez que los diseños estuvieron listos, nos sumergimos en la configuración de las impresoras 3D. Desde la selección de materiales hasta la calibración de la impresora, cada paso fue crucial para garantizar la precisión y la calidad de los resultados finales. Durante el laboratorio, cada uno de nosotros tuvo la oportunidad de diseñar su propio objeto tridimensional. Empezando por un cilindro, diseñando un vaso y por último en grupo se realizó el desarrollo y la impresión de un soporte de Arduino 1, esta actividad muestra nuestro desarrollo desde lo más simple hasta estructuras más complejas, exploramos la versatilidad de la impresión 3D. Este informe detallará nuestras experiencias, los desafíos encontrados y las lecciones aprendidas durante el laboratorio de impresión 3D. Además, proporcionaremos una visión general de las aplicaciones prácticas de la tecnología y cómo puede integrarse en diversos campos, así como en el desarrollo de nuestro prototipo que vamos desarrollando.


## 2. Ejercicio 1

1.1 Al realizar el primer ejercicio de un cilindro 3D, con un diámetro de 80 mm. Se inició con la base inferior “Top” centrando la base en el  medio. 

1.2 Después se creó un boceto de “sketch” para dar una forma cilíndrica de una proporción extensa de 100 mm de altura.

1.3 Después se agregó 3 mm de grosor del cilindro.

1.4 luego para ver en 3 dimensiones se presionó el anticlic y finalmente terminamos nuestro primer ejercicio.

| Top | Sketch |
|-----------|-----------|
| ![Descripción de la imagen](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/f0533903-6a30-4363-997f-9664fa1d1aa9) | ![Descripción de la imagen](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/f8ed20c3-56c9-4e46-a0bd-717fa6409c83)|
| Groser | 3 dimenciones |
| ![Descripción de la imagen](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/84afbb69-0903-48c8-93dd-c1c569486dfc) | ![Descripción de la imagen](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/dd6fc705-5955-473a-9121-0d86fd8000ca)|


## 3. Ejercicio del vaso en 3D

Después de adquirir ciertos conocimientos sobre el desarrollo de dibujos en 3D, procedimos a realizar la siguiente actividad: la creación de un vaso utilizando la herramienta Onshape. Siguiendo el enfoque del ejercicio anterior, creamos un nuevo boceto para representar figuras en dos dimensiones. Este método nos permitió diseñar el vaso como si lo estuviéramos viendo directamente en un plano. Utilizando la herramienta "line", trazamos las líneas que conformarían la estructura del vaso. Establecimos una altura de 100 mm, con la parte superior del vaso midiendo 40 mm y la inferior 25 mm, esas medidas se realizarón con el apartado de "dimensión" que permite colocar las medidas que deseamos en cada linea trazada. Después de ello, para que todo este bien definido colocamos el "midpoint" para centrar la figura correctamente.

Una vez completado este proceso, aplicamos la función "revolve" para transformar el dibujo bidimensional en una figura tridimensional en 3D. Posteriormente, utilizamos la herramienta "shell" para retirar la parte superior del vaso, creando así un espacio hueco. Luego, aplicamos "fillet" para agregar una curvatura exterior al vaso, mejorando su estética. Como paso final, editamos la apariencia del vaso cambiando sus colores.

| Line | Dimension |
|-----------|-----------|
| ![Descripción de la imagen](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/blob/main/Imagenes/Line.png) | ![Descripción de la imagen](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/blob/main/Imagenes/Dimension.png)|
| Midpoint | Shell|
| ![Descripción de la imagen](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/blob/main/Imagenes/Midpoint.png?raw=true) | ![Descripción de la imagen](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/blob/main/Imagenes/Shell.png)|
| Dimensiones 2D | Dimensiones 3D |
| ![Descripción de la imagen](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/blob/main/Imagenes/Captura%20de%20pantalla%202024-02-02%20223107.png) | ![Descripción de la imagen](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/blob/main/Imagenes/Captura%20de%20pantalla%202024-02-02%20210252.png)|

## Ejercicio  N° 4: Representación de una estructura para Arduino UNO

Para esta actividad el docente encargado, nos pidió modelar una estructura en 3D para guardar y proteger el Arduino Uno. Para su elaboración se utilizaron diferentes sketchs y múltiples comandos extrude y shell. Para ello iniciamos ubicando el eje en la vista TOP y luego añadimos una imagen del Arduino con las medidas específicas.

Guía para dibujar la estructura del ARDUINO. Fuente: Google

![image](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023044/c76c6b05-008e-4da7-833b-cf1e274e0df2)


Seguidamente, aseguramos que la altura sea de 14 mm y el grosor sea de 3 mm, para que esté centrada en el plano. Luego, utilizamos la función "lineal" para crear el marco del Arduino y añadir las medidas correspondientes. Después, utilizamos la función "shelf" para crear la tapa del estuche. Finalmente, con la opción "Part 1" añadimos el color de preferencia al estuche para poder terminar dicho modelo.

![image](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023044/9c7d4983-e698-4af9-80f7-ea09033c1ff8)

Fuente: Elaboración propia

## 4.1 Proceso de la impresión de la estructura del Arduino 

Para llevar a cabo nuestra impresión, la Universidad nos brindó la facilidad de poder imprimir nuestro modelo de Arduino en una de las mejoras impresoras de última generación como es el (Ender 3 S1) y el ( Bambú Lab) esto debido al corto tiempo que  demoran en imprimir. 
En esta sección uno de los encargados, nos  brindó la información necesaria para comprender el correcto funcionamiento del proceso de impresión. 

![image](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023044/267d1977-9ee5-477a-87c6-d013391c6c03)

Fuente: Elaboración propia


Una vez recibida la información necesaria se pasó a imprimir el archivo solicitado, para este proceso se utilizó el formato  STL en impresión de 3D, también uno de los puntos a considerar es la altura de la capa, además el relleno es uno de los puntos más importantes, para este tipo de  pruebas se recomienda usar al mínimo debido al tiempo que tarda en imprimir ya que mientras mayor sea la impresión de la velocidad  menos resolución tendrá.

![image](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023044/23775995-bffa-4c8d-98a5-d93be48cb519)

Fuente: Elaboración propia


Finalmente, una vez laminado nuestra estructura, se calculó el tiempo de impresión de (53 minutos aproximadamente) para enviarlo a través de la nube a un servidor de la propia impresora permitiéndonos obtener un modelo de estructura o carcasa para Arduino UNO.

![image](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023044/4c517779-706a-4f2d-9e76-2b05e9b06ef0)
![image](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023044/89ed2929-1f10-4b32-b538-a3ca2b76ce0f)
![image](https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023044/e5cf01d5-3d8f-4a14-af1d-5ff4dbb28be1)
Fuente: Elaboración propia


## Conclusión 

En conclusión, este laboratorio sobre impresiones 3D nos ha proporcionado una oportunidad para explorar esta tecnología de manera práctica. A través de la experiencia directa en diseño, visualización de la configuración de impresión y de los resultados, hemos obtenido una comprensión más profunda de la impresión 3D y sus aplicaciones en el mundo real. Durante el laboratorio, se observó que la fase de diseño desempeña un papel importante en el éxito de la impresión. La medición cuidadosa a la geometría y la consideración de los requisitos específicos, como dejar 0.1 mm de espacio para la impresión, son esenciales para garantizar resultados precisos y satisfactorios. La configuración de la impresión también se destacó como un aspecto crucial. Desde los materiales que se utilizan hasta la calibración precisa de la impresora, cada ajuste influye directamente en la calidad y la integridad estructural de los objetos impresos. Una de las lecciones que destacamos de esta experiencia es la importancia de la paciencia y la atención a los detalles. Cada fase del proceso requiere de tiempo, cuidado y consideración. En nuestro caso para la impresión de nuestro diseño se utilizo la impresora 3D Bambu Lab P1P que cuenta con una mayor velocidad con un promedio de 200 milímetros por segundo(mm/s) y 500 mm/s. Además, hemos comprendido que la impresión 3D no solo es una herramienta de prototipado rápido, sino una tecnología que ayuda de transformar la fabricación en diversos campos, en nuestro caso nos será de mucha ayuda para el desarrollo de nuestro proyecto. Este laboratorio se ha demostrado que la impresión 3D más que una tecnología, es una herramienta poderosa que nos ayuda en la innovación. La capacidad de convertir nuestras ideas en objetos tangibles abre nuevas posibilidades para la creatividad y el desarrollo de nuestros proyectos. Asimismo, la exploración de esta tecnología en el laboratorio ha sido una experiencia beneficiosa que ha ampliado nuestro entendimiento de esta tecnología y la importancia del potencial que tiene en el mundo que nos rodea.
