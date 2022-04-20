# TopoTron

## Un display volumétrico de baja resolución 

### Concepto

**TopoTron** es un display volumétrico que utiliza LEDs direccionables **2812** para crear una matriz tridimensional. En este proyecto se exploran las posibilidades y capacidades que un dispositivo de este tipo ofrece para crear no solo topografías sino efectos visuales, animaciones etc.

Se asemeja en concepto a los conocidos **cubos LED**, pero en este caso el factor de forma es diferente, es un prisma de poca altura y bastante base. De este modo se pueden mostrar topografías mas fácilmente. También se presta atención a los difusores de luz de los LED . En un cubo LED normalmente no se emplean por lo que vemos una matriz de puntos luminosos que pueden crear efectos visuales pero no dan una buena sensación de volumen. En Topotron los difusores buscan un compromiso entre recrear un volumen y no entorpecer visualmente los LED que se encienden al frente con los que se encienden por detrás. Asi que el tipo de material del difusor, su tamaño y forma, y la distancia entre los mismos influyen en el efecto a conseguir.

En esta imagen de concepto vemos el objetivo ideal. Se ha realizado mediante el programa opensource **MagicaVoxel.**

![TopoTron](TopoTron.png)

### Características principales del prototipo:

- Primer prototipo con 5x8x7 voxels (píxeles volumétricos).

- Tiras LED del tipo WS2812.

- Difusores impresos en 3D para crear el efecto adecuado.

- Microcontrolador basado en ESP8266.

La versión que se entregará como recompensa tiene las características indicadas pero tendrá un mejor acabado que el prototipo que permitirá su uso y transporte. 

### Modelo grande (objetivo del proyecto): 

- Matriz mas grande con 24x16x8 vóxeles o similar.

- Bastidor robusto para alojar el dispositivo y facilitar su uso y transporte.

- Optimización del software para ampliar los efectos disponibles.

### Lista de materiales (BOM):

El enlace está **[aquí](BOM.xlsx)** (en construcción):

### Crowdfunding y cofinanciadores:

Este proyecto se inicio como concepto y se prototipó en el marco del concurso internacional **Hackaday Prize** realizado en 2021. 

El enlace a ese proyecto (en inglés) está **[aquí](https://hackaday.io/project/180204-topotron).**

Se presentó a concurso y no quedó seleccionado, pero la idea me gustó y quise seguir trabajando con ella, con el fin de construir una unidad mas grande y ver así las posibilidades que ofrecía. Por ello me presenté a crowdfunding con la **Fundación Goteo** y a final de 2021 conseguí los fondos necesarios. 

Asi que este proyecto no hubiera sido posible sin el apoyo de las personas y colectivos que lo han cofinanciado. 

La ficha del proyecto en la **Plataforma Goteo** lo tienes **[aquí](https://www.goteo.org/project/topotron).**

La lista de personas y colectivos que han contribuido a la financiación la tienes **[aquí](Cofinanciadores.md).**

## Creditos

**TopoTron** es un concetpo desarrollado por **Victor Barahona** en **[Egokitek](https://www.egokitek.com/)**.

Se ha inspirado en los **cubos LED** y otros conceptos de display volumétricos.

En este proyecto estoy utilizando las librerías FASTLED y mi propio contenido. Ver mas en **[FastLED](https://github.com/FastLED/FastLED).**

## Licencia

**GPL3.0**

Renderizados hechos con **MagicaVoxel**

![TopoTron2](TopoTron2.png)



