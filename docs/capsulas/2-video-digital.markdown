---
layout: default
title: 'Video digital. Aspectos técnicos básicos'
nav_exclude: true
categoria: capsula
---

# {{ page.title }}
{: .no_toc }  

**Contenidos de la cápsula**  

- TOC
{:toc}

---

## Parte 1: Resolución

La resolución de un archivo, tanto de imagen fija como de una imagen en movimiento es la medida de sus dos dimensiones: ancho y alto. Suele confundirse con "calidad" o "definición", pero es importante comprender que no estamos hablando de cualidades subjetivas, sino objetivas. La resolución de una imagen se mide en píxeles y la "calidad" o "definición" es una percepción de la resolución del video/imagen y la superficie o dispositivo en el cual vemos esa imagen. Antes de llegar a esa situación profundicemos sobre la resolución.

Al producir video podemos elegir distintas resoluciones de edición y exportación. Existen estándares que a medida que se desarrollan nuevas tecnologías y dispositivos de reproducción se van incorporando. Actualmente las resoluciones en píxeles más comunes para video son (siempre en ancho x alto):

**HD**: 1280 x 720  
**FullHD**: 1920 x 1080  
**4K**: 3840 x 2160  

En el siguiente gráfico podremos ver la comparación de resoluciones.

<br>
![alt text](../../../assets/images/Video_Resolution_Chart.svg "Resoluciones de video tradicionales")

Ahora que sabemos qué significa la resolución podemos analizar ¿qué es la "calidad"?

La calidad de una imagen es un parámetro subjetivo. La frase más conocida para referirnos a una imagen de "baja calidad" es "se ve pixelado". Como mencioné anteriormente, la calidad o definición es una relación entre la resolución y el tamaño físico del soporte en donde se presenta la imagen.

En el siguiente ejemplo vemos en el mismo tamaño de imagen, un logo con distinta resolución. Esto mismo pasaría si proyectamos el mismo video en un teléfono y en una pared de 4 x 3 metros. El efecto "pixelado" es ver el detalle de los pixeles que componen la imagen y de esa forma sus bordes. En el caso de este ejemplo lo que vemos es una misma imagen en un mismo tamaño pero con resolución 16 x 16 hasta 512 x 512.


![alt text](../../../assets/images/Vimeo-Logo-Scale.jpg "Comparación de resoluciones")


## Parte 2: Cuadros por segundo (_Frame rate_)

Los cuadros por segundo corresponden al parámetro temporal de una imagen en movimiento: ¿Cuántos veces se actualiza la imagen a lo largo de un segundo?

Los cuadros por segundo, o frame rate (_fps_), se definen según la configuración o posibilidad de las cámaras al grabar, o de nuestros programas de edición en el caso que generemos imágenes con algún programa de animación. Luego, esa configuración debe mantenerse, o modificarse, al exportar el video. Y finalmente, la misma decisión pasa en los programas de reproducción si es que nos permite configurar el frame rate. La mayoría de los reproductores toman la configuración de cuadros por segundo el video.

En el siguiente video vemos la misma animación de un círculo con diferentes cuadros por segundos.


<div class="video-container">
    <iframe src="https://www.youtube.com/embed/pfiHFqnPLZ4" height="406" width="720" modestbranding="1" rel="0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
    </iframe>
</div>

## Parte 3: Formatos, contenedores y códecs

Es muy habitual confundirnos entre formatos, códecs y contenedores. Según la plataforma de reproducción, y el hardware de grabación/filmación, tendremos que elegir las opciones más adecuadas para que nuestros archivos se exporten de la forma más eficiente y con el menor tamaño posible.  

**¿Qué es un códec?**

El códec (palabra que viene de **cód**ificador/**dec**odificador) es un software o hardware capaz de procesar información, en este caso, video. Especificamente, comprimen y descomprimen los datos. Existen muchos en la actualidad, y en algunos casos muchos programas de reproducción incluyen, al instalarlos, códecs compatibles.

Algunos de los códecs más conocidos son:

H264  
Es el códec más usado en la actualidad. Incluso muchos dispositivos (smartphones por ejemplo) están diseñados para grabar y reproducir en este códec. Tiene una gran performance pero una limitación importante: sólo es posible reproducir videos de hasta 4096px x 2048px de resolución.

DXV  
Creado por la empresa Resolume para reproducir videos con la máxima compatibilidad para el software Resolume Arena. No es compatible con otros reproductores de video, por lo tanto, si tenemos videos en DXV sólo podremos verlos con aplicaciones de Resolume.

PhotoJPEG  
Es un códec que no tiene pérdida de calidad, almacena cada uno de los fotogramas como si se tratase de fotografías. Es ideal para su procesamiento en tiempo real en softwares de VJ ya que cada frame es un keyframe.


**¿Qué es un contenedor?**

Algunos de los contenedores más conocidos son:

AVI  
Es uno de los contenedores más famosos y antiguos. Compatible con muchísimos códecs, pero que en la actualidad no es tan recomendado su uso.

MP4  
Es el formato más conocido. Compatible con H264 y MPEG-4 (por lo tanto su resolución máxima es de 4096px x 2048px). Es el stándard para web (YouTube, Vimeo, Instagram).

MOV  
Es muy común entenderlo como el stándar de Apple, ya que todos sus dispositivos graban y almacenan en este formato. Pueden contener códecs con gran calidad (DXV o ProRes por ejemplo) y es uno de los ideales para almacenar videos de muchísimo tamaño y calidad.

## Parte 4: Conclusiones

En proyectos que se verán en web, o que tienen que ser videos de fácil reproducción, usar h264 y MP4. En los casos donde la reproducción requiera máxima calidad, usar ProRes y MOV. Si necesitamos utilizar software de VJ (Resolume Arena por ejemplo), elegir DXV o PhotoJPEG y MOV.
