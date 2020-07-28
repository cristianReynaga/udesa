---
layout: default
title: Exportar en Premiere Pro
parent: Premiere Pro
grand_parent: Tutoriales
nav_order: 2
has_children: false
---

# Exportar en Premiere Pro
{: .no_toc }

![alt text](/assets/tutoriales/portada exportar premiere.png "Exportar con Premiere Pro")

Exportar es el último paso que realizamos al editar video, es la etapa en la que transformamos nuestra línea de tiempo en un archivo. Adobe nos brinda dos posibilidades: hacerlo desde nuestro proyecto en Premiere Pro, o realizarlo desde Adobe Media Encoder. Esta segunda opción nos permite realizar la exportación en un programa separado liberando Premiere Pro de esta tarea y pudiendo continuar editando, entre otros beneficios. En este tutorial nos centraremos en la opción más sencilla que es exportar desde Premiere Pro.
  

## Contenidos
{: .no_toc }

- TOC
{:toc}


## Parte 1: Cómo exportar en Premiere Pro
La exportación se realiza desde el panel de Exportación.

1. Tener una **Proyecto** y una **Secuencia** configuradas y asegurarse que el panel de la línea de tiempo este activo.
2. Ir a **Archivo > Exportar > Medios**, o con la línea de tiempo activa apretar CTRL + M (en Windows) o CMD + M (en Mac).


## Parte 2: Configuraciones según el formato 

Cada soporte y dispositivo de reproducción tiene su propia configuración óptima. Esto incluye formato, códec, bit rate, resolución y sample rate y bit rate para el audio. No es lo mismo reproducir en una notebook o pc que tendrá una gran capacidad de procesamiento, por lo que no tendríamos limitaciones en el tamaño del archivo ya que tendríamos a disposición una computadora para reproducir nuestro archivo, que si es un video para YouTube, que al momento de la subida re-procesa el archivo para que su reproducción sea lo más rápida posible, que si reproducimos desde una web.

Es importante consultar para cada situación de exhibición con qué dispositivo se reproducirá y a qué tamaño. No es lo mismo un video reproducido en un TV LED de 46" que un proyector que amplifica la imagen 4 metros de ancho (en este caso nuestros píxeles estarían midiendo mucho más que en una pantalla). Tampoco si se piensa para Instagram tanto en formato cuadrado o vertical, y no sólo por la relación de aspecto, sino por el tamaño de las tipografías y la composición en general.

![alt text](/assets/tutoriales/resoluciones_exportar.png "Comparativa de resoluciones")


## Parte 3: Exportar para el simulador 3D  

Exportar a formato .mp4 con códec .h264 en resolución 1510 x 200px

<iframe width="100%" height="400" src="https://www.youtube.com/embed/loU0AEbsef0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Parte 3: Exportar para la pantalla 270  

Exportar a formato .mov con códec DXV3 en resolución 6036 x 800px.

### IMPORTANTE: 
Para exportar con el códec DXV3 es necesario instalar antes Resolume Arena y/o Alley. Esto nos instalará automáticamente el códec DXV3 que no es standard y sólo se usa con el sistema de la pantalla 270.

<iframe width="100%" height="400" src="https://www.youtube.com/embed/44AxXSpLraw" modestbranding="1" rel="0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


