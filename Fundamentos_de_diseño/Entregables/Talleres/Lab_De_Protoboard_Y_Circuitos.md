## INFORME: 2

# Resolución del laboratorio de manejo de protoboard y circuitos útiles: Fundamentos de Diseño

1. **INTRODUCCION**
   
En este laboratorio, nos sumergimos en el manejo de protoboard para la creación de circuitos tanto en serie como en paralelo. El enfoque fue construir de manera práctica sistemas eléctricos basándonos en la guía del laboratorio y las recomendaciones proporcionadas por los docentes durante la sesión. Previo a la implementación práctica, dedicamos tiempo al estudio detallado de cada componente y parte que conforma un circuito eléctrico. Es esencial comprender el funcionamiento de los elementos involucrados antes de su aplicación. En el caso de un circuito en serie, se analizó que el voltaje es la suma de cada voltaje encontrado en cada resistencia, mientras que la intensidad permanece constante. En cambio, para un circuito en paralelo, se consideró que la intensidad es la suma de cada intensidad encontrada en cada resistencia, mientras que el voltaje es constante.
Para poder hubicarnos de forma ordenada identificamos los valores de cada una de las resistencias, se siguió los códigos de colores para obtener un mejor resultado.

<img width="400" height="400" src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/28129d6d-8994-4efb-aabd-dbf0d2cccc62" alt="Descripción de la imagen"> 

Fuente: https://www.areatecnologia.com/electricidad/codigo-de-colores-de-resistencias.html


## 2. EJERCICIO NIVEL POLLITO-GATO:
### 2.1. Ejercicio en serie:

Las resistencias R1 y R2, ambas con un valor de 100kΩ, están conectadas en serie, lo que nos lleva a realizar una suma directa y obtener un resultado de 200 kΩ. Posteriormente, al sumar la inversa de este valor con la resistencia R3 (también de 100kΩ), obtenemos una resistencia equivalente de 66.67 kΩ
La elección de valores específicos para las resistencias, en este caso, 100kΩ, se ha realizado con el propósito de facilitar el cálculo y confirmar la precisión del circuito al medirlo con un multímetro y obtener valores cercanos.

<img width="600" height="300" src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/fd5c8ace-5073-4000-981f-91258ce54451" alt="Descripción de la imagen">

<img width="600" height="300" src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/876e565a-95a3-4a22-9bf3-70bdbe512163" alt="Descripción de la imagen">

### 2.2 Ejercicio en paralelo:

En este ejercicio, comenzamos por examinar detenidamente la imagen de la guía y luego procedimos a modificar la representación original para determinar si el circuito estaba configurado en serie o en paralelo.
Al analizar la imagen, observamos que el circuito presentaba una combinación de configuraciones en serie y en paralelo. En consecuencia, sumamos las resistencias R1 y R2, ambas con un valor de 100kΩ, obteniendo un resultado de 200kΩ.
Posteriormente, sumamos las resistencias restantes que estaban en paralelo con R1 y R2. Para obtener este valor, aplicamos el cálculo considerando la inversa.
Después de realizar los cálculos, verificamos la validez del ejercicio utilizando un multímetro.
Los valores medidos se aproximaron a los teóricos, confirmándose así la precisión del circuito.

<img width="600" height="300" src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/ccb77db1-3104-43b0-ab7a-338319b8b2a7" alt="Descripción de la imagen">

<img width="600" height="300" src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/bcc3eda9-3430-4393-97da-c1f55d489904" alt="Descripción de la imagen">


## 3. EJERCICIO NIVEL DRAGON:

En esta sección, procedemos a calcular el equivalente de la figura. 
Primero, dividimos la figura original para facilitar el cálculo conforme se indica en el ejercicio. Utilizamos las resistencias en serie, las cuales presentan un único camino por el cual la corriente puede fluir.
Seguidamente, sumamos las resistencias R1 y R3, luego, sumamos R2 con R4 y finalmente, sumamos R5 y R6 en circuitos en serie, lo que nos proporciona un valor de 200 kΩ en cada caso.
Posteriormente, tomamos la inversa de cada suma y calculamos la resistencia equivalente.

<img width="600" height="300" src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/44733fb1-2d79-4a38-b4cc-4ff7fbc93fe6" alt="Descripción de la imagen">

Una vez calculada la resistencia, pasamos armar el circuito completo en serie y comprobamos mediante nuestro multímetro el valor obtenido de la resistencia.

<img width="600" height="300" src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/34f4fc8e-24f8-4a9c-ad69-4f76fc84466c" alt="Descripción de la imagen">

<img width="600" height="300" src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/a7f699f9-8d61-4850-bdee-d628c2136773" alt="Descripción de la imagen">

Fuente: Elaborado en tinkercad 

## 3. Circuito Divisor de Tensión

Para obtener el resultado se tuvo que obtener la relación de la resistencia 1 con la resistencia 2.  En el protoboard para hallar la resistencia de 3.54k ohms se usó tres resistencias en serie y dos en paralelo, todas equivalentes a 1k ohmios. También el resistor 2 que equivale a 1 ohms.

**El voltaje de salida debe de ser de 1.1 en la siguiente figura:**

<img width="600" height="300" src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/823e5e5a-00a3-4f11-a235-f9f9074b241a" alt="Descripción de la imagen">


**Fórmula:**

$Vin = (R1 + R2) * I$

$I = \frac{Vin}{(R1 + R2)}$

$Vout = R2 * I = R2 * \frac{Vin}{(R1 + R2)}$

**Encontrar R1**

$R1 + R2 = R2 * \frac{Vin}{(R1 + R2)}$

$R1 + R2 = R2 * 4.54 ... ... ... (a)$

$Asumimos: R2 = 1KΩ$

$R1 = R2 * 4.54 - R2$

$R1 = 3.54KΩ$

**Simulación para verificar que la salida sea correcta**

Para verificar los resultados se realizó una simulación en tinkercad, que se muestra en la siguiente imagen.

<img width="600" height="300" src="https://github.com/Alexander-Manosalva-Peralta/Proyecto-De-Fundamentos/assets/156023729/a07427c6-9c67-45b4-951e-bef261868f16" alt="Descripción de la imagen">

Fuente: Elaborado en tinkercad 

## 4. Conclusiones:

En conclusión, el laboratorio de manejo de protoboard y circuitos útiles proporcionó una valiosa experiencia en la aplicación práctica de los conceptos fundamentales de circuitos eléctricos. A través de la construcción de circuitos en serie, paralelo y su combinación, se fortaleció nuestra comprensión de cómo el voltaje e intensidad se comportan en diferentes configuraciones. El enfoque detallado en el estudio previo de cada componente antes de su implementación práctica demostró ser esencial para el éxito de los experimentos.
En conjunto, este laboratorio no solo consolidó los fundamentos teóricos, sino que también enfatizó la importancia de la precisión en la implementación práctica de circuitos eléctricos. La combinación de teoría, cálculos, experimentación y simulación proporcionó una comprensión integral y aplicada de los conceptos clave en el diseño y análisis de circuitos eléctricos.





































































































































^G Help            ^O Write Out       ^W Where Is        ^K Cut             ^T Execute         ^C Location        M-U Undo           M-A Set Mark       M-] To Bracket     M-Q Previous       ^B Back            ^◂ Prev Word       ^A Home            ^P Prev Line       M-▴ Scroll Up      ^▴ Prev Block      M-( Begin of Paragr^Y Prev Page       M-\ First Line     M-◂ Prev File      ^I Tab             ^H Backspace       M-Bsp Chop Left    M-T Cut Till End   M-D Word Count     M-} Indent         M-3 Comment Lines  M-: Record         M-Del Zap          M-PgUp Up to anchorF12 Spell Check    M-F Formatter      ^L Center
^X Exit            ^R Read File       ^\ Replace         ^U Paste           ^J Justify         ^/ Go To Line      M-E Redo           M-6 Copy           ^Q Where Was       M-W Next           ^F Forward         ^▸ Next Word       ^E End             ^N Next Line       M-▾ Scroll Down    ^▾ Next Block      M-) End of Paragrap^V Next Page       M-/ Last Line      M-▸ Next File      ^M Enter           ^D Delete          ^Del Chop Right    M-J Full Justify   M-V Verbatim       M-{ Unindent       ^] Complete        M-; Run Macro      M-Ins Anchor       M-PgDn Down to anchM-B Linter         ^L Refresh         ^S Save

