---
layout: default
title: 'Color Digital: Introducción'
nav_exclude: true
categoria: capsula
---

# {{ page.title }}
{: .no_toc }

**Contenidos de la cápsula**  

- TOC
{:toc}

---

## Parte 1: Sistemas y modos de color

`
"Un modelo de color es un modelo matemático abstracto que describe la forma en la que los colores pueden   representarse como tuplas de números, normalmente como tres o cuatro valores o componentes de color (p.e. RGB y CMYK son modelos de color). Sin embargo, un modelo de color que no tiene asociada una función de mapeo a un espacio de color absoluto es más o menos un sistema de color arbitrario sin conexión a un sistema de interpretación de color."
`

Fuente: [Wikipedia](https://es.wikipedia.org/wiki/Espacio_de_color)

Con esta definición (entre las diversas existentes para distintos campos de aplicación) vamos a desarrollar lo específico del color en el diseño digital audiovisual. Esto será la base para comprender las transformaciones de color en video, llamado _color grading_.


### Sistemas Aditivo y Sustractivo   

En video e imagen digital el sistema utilizado es el **Sistema Aditivo**, que lleva su nombre porque en este sistema los colores se suman cuando se superponen. En tanto, en la producción gráfica y plástica (pinturas acrílicas, óleos, témperas) se utiliza el **Sistema Sustractivo**

![alt text](../../../assets/images/color_sistemas.png "Sistemas de color")

Si tenemos la oportunidad de experimentar con luces o linternas de colores o un proyector, podríamos ver como los distintos colores se reflejan en una superficie y se van suporponiendo, "se van sumando" sus colores. Esta es la base del sistema aditivo, siendo el blanco la mezcla de mayor valor de los colores primarios de este sistema. Los colores primarios en el sistema aditivo son **Rojo, Verde y Azul**.

En el dominio digital quienes poseen los colores son los píxeles, la unidad mínima en pantalla que tienen dos propiedades básicas: ubicación y color. Los componentes de color de cada píxel se representa, como menciona la primera definición elegida, como secuencias de números. En el caso del modo de color **RGB (R=Red; G=Green; B=Blue)**, usualmente cada color o componente tiene un rango de 8 bits (ya profundizaremos), lo que otorga 256 valores posibles para cada canal, siendo 0 es el valor mínimo y 255 su valor máximo.  

### Ejemplo interactivo de color aditivo  
En este ejemplo podemos deslizar los sliders para variar el valor de cada círculo. En este caso cada círculo tiene un solo color de 0 a 255. **0 es total ausencia de color y 255 es total presencia del color**.  
Vemos entonces que en el centro, en la superposición de los tres canales, se observa la suma. También es importante notar la codificación de los colores en dos sistemas: RGB, usado en todas las aplicaciones y herramientas de diseño, y Hexadecimal, más frecuente en la programación y diseño web.

<div class="video-container">
    <iframe src="https://editor.p5js.org/cristianreynaga/embed/6koGdZ_DH" height="406" width="720" frameborder="0">
    </iframe>
</div>  

<br>

### Modos de color  
El sistema aditivo, como observamos, se compone de la suma de tres colores primarios, pero esa no es la única forma de generar colores. Existen distintos modelos matemáticos con los que pueden conseguirse los mismos colores. Estos se llaman modos de color, o espacios de color, que según el caso, pueden ofrecer mayores facilidades para realizar la composición resultante.

**Modelo de color RGB**   
Los colores aparecen con sus componentes primarias de rojo, verde y azul. Los valores de R, G, y B se encuentran a lo largo de tres ejes, basados en el sistema Euclideano de tres vectores y un mismo origen. En otras palabras, en el eje del rojo, en el eje del verde y en el eje del azul se encuentran las intensidades de cada color. El cián está situado en el vértice del cubo en donde el color verde y el azul tienen su máximo valor, y el valor del rojo es cero; las coordenadas son (R, G, B) = (0, 1, 1). Análogamente, el magenta que es la combinación del rojo y el azul está situado en las coordenadas (R, G, B) = (1, 0, 1); y el amarillo (mezcla de verde con rojo) se situa en (R, G, B) = (1, 1, 0). El negro está posicionado en el origen del sistema y el blanco en el vértice opuesto al origen. La escala de grises se encuentra en la diagonal que va del negro al blanco, los colores restantes se encuentran dentro del cubo.  

Todos los valores de R, G y B están en el intervalo [0,1]. En el caso de imágenes digitales los valores de R, G y B son números enteros y van de 0 a 255, lo cual permite generar 16.777.216 colores.  

![alt text](../../../assets/images/color_rgb_cube.png "RGB Color")


**Ejemplo interactivo RGB**  
Cada slider representa el valor de 0 a 255 de cada canal del color del rectángulo.  

<iframe src="https://editor.p5js.org/cristianreynaga/embed/NRrqOBY3w" height="200" width="720" frameborder="0"></iframe>
  
<br>

**Modelo de color HSV/HSB**  
En el caso del sistema HSV (HUE, SATURATION, VALUE) o HSB (HUE, SATURATION, BRIGTHNESS) los valores de cada canal no son 0 - 255. Como se observa en el gráfico, el modelo matemático en este caso es un cono, por lo que el HUE tiene un giro de 360º y SATURATION y VALUE tienen valores de 0% a 100%.

**Brillo** encarna la noción acromática de intensidad. **Tono** (Hue) representa el color dominante según lo percibe un observador. Así, cuando llamamos a un objeto rojo, naranja o amarillo, nos referimos a su tono. La **Saturación** se refiere a la pureza relativa o la cantidad de luz blanca mezclada con un tono. Los colores del espectro puro están completamente saturados. Los colores como el rosa (rojo y blanco) y el lavanda (violeta y blanco) están menos saturados, siendo el grado de saturación inversamente proporcional a la cantidad de luz blanca añadida.

![alt text](../../../assets/images/color_hsv_cone.png "HSV Color")

**Ejemplo interactivo HSB**  
Cada slider representa el valor de HSB del color del rectángulo.  

<iframe src="https://editor.p5js.org/cristianreynaga/embed/OKf-r9MY8" height="200" width="720" frameborder="0"></iframe>

Es posible experimentar en este modelo de color que con solo modificar un parámetro, el HUE, es más simple cambiar de color, a diferencia del modelo RGB que es necesario modificar los tres parámetros para encontrar colores interesantes. A la hora de programar el sistema HSB permite mayor control con menos programación en la mayoría de los casos.  

## Parte 2: Color Depth y Color Sampling
Los bits son la unidad de medida de la computación en su más mínima expresión. Cada bit puede tener solo dos valores y son el famoso 0 y 1 del que tanto se habla. En el caso de las imágenes, podemos pensar que cada uno de los pixeles que la forman pueden tener sólo 2 valores: blanco o negro.  

![alt text](../../../assets/images/1_bit.png "1 Bit Depth")


Si aumentamos los bits, supongamos que a 4 bits, tendremos 16 variaciones, y con 8 bits tendremos 256 posibilidades. La cantidad de bits utilizados para representar el componente de color de cada píxel se denomina **profundidad de píxel** (_color depth_). Esto se visualiza en el ejemplo con escalas de grises, pero funciona del mismo modo para los colores:   

![alt text](../../../assets/images/bit_depth.png "Bit Depth")

![alt text](../../../assets/images/bit_depth_samples.png "Bit Depth Samples")

Considere una imagen RGB en la que cada una de las imágenes roja, verde y azul es una imagen de 8 bits. En estas condiciones, se dice que cada píxel de color RGB [es decir, un triplete de valores (R, G, B)] tiene una profundidad de 24 bits (3 planos de imagen por el número de bits por plano). El término imagen a _full color_ se utiliza a menudo para denotar una imagen en color RGB de 24 bits. Como señalamos antes, el número total de colores en una imagen RGB de 24 bits (8 bits por cada color= 256 * 256 * 256) = 16.777.216 posibilidades de color. 

En este ejemplo se observa en el cubo de la izquierda como se mapea cada color en 5 valores posibles, y en a la derecha la diferencia entre un gradiente de 8 bits y el mismo gradiente con 10 bits de profundidad.  

![alt text](../../../assets/images/bit_mapping.png "Color Bit")

Todo esto nos permite entender cómo es posible comprimir imágenes y degradarlas si no somos conscientes de las distintas posibilidades de formatos, códecs y compresión.  

![alt text](../../../assets/images/color_sampling.png "Color Sampling")

## Parte 3: Herramientas on line 

**Creación de paletas de color**  

- [Adobe Kuler](https://color.adobe.com/create/color-wheel){:target="_blank"}
- [Herramienta de paleta de color CANVA](https://www.canva.com/colors/color-wheel/){:target=_"blank"}
- [Color Schemer](https://www.colorschemer.com/color-picker/){:target="_blank"}
- [Palleton](http://paletton.com/#uid=1000u0kllllaFw0g0qFqFg0w0aF){:target="_blank"}

## Referencias

- [Digital Image Processing. GONZALEZ, Rafael y WOODS, Richard. 2008.](../../../assets/bibliografia/DigitalImageProcessing.pdf){: target="_blank"}
- [Espacios de Color RGB, HSI y sus Generalizaciones a n-Dimensiones. ALONSO PÉREZ, Marco Antonio. 2009.](../../../assets/bibliografia/AlonsoPeMA-color.pdf){: target="_blank"}
- [El arte del color. ITTEN, Johannes.](../../../assets/bibliografia/arte-del-color-itten.pdf){: target="_blank"}




<!-- https://www.provideocoalition.com/blend_modes_in_adobe_premiere_pro/ -->

<!-- https://blogs.adobe.com/creativecloud/color-correction-and-color-grading-tutorials-from-karl-soule-and-andrew-devis/?segment=dva -->