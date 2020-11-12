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

## Parte 3: Formatos y códecs
