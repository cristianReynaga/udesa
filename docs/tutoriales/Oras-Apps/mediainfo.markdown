---
layout: default
title: Inspector Media Info
parent: Otras Aplicaciones
grand_parent: Tutoriales
nav_exclude: true
has_children: false
tutorial: Otras
---

# Media Info  
{: .no_toc }  

![alt text](/assets/tutoriales/portada_mediainfo.png "Inspector Media Info")

MediaInfo es una aplicación que vsualiza los datos técnicos y de etiquetas más relevantes de archivos de video y audio. Permite inspeccionar todo tipo de archivos de video y sonido con un nivel de detalle adecuado para realizar una correcta gestión de nuestros proyectos audiovisuales. Presenta distintas formas de visualizar la información, tiene versiones gratuitas para Windows y Mac y es muy sencillo comenzar a utilizarla.  

[Sitio oficial para descargar](https://mediaarea.net/en/MediaInfo){:target="_blank"}
  

## Contenidos
{: .no_toc }

- TOC
{:toc}

---

## Parte 1: Cargar archivos en Media Info

1. Existen dos opciones:
     1.  Arrastrar un archivo sobre la interfaz.
     2.  Click en **Archivo/Abrir** y seleccionar nuestro archivo.

Luego de cargar un archivo veremos los campos de **General**, **Video** y **Audio** con datos del archivo en la visualización por defecto.

![alt text](/assets/tutoriales/mediainfo1.png "Inspector Media Info")  

## Parte 2: Elegir la visualización de los datos

Es conveniente cambiar la visualización por defecto si necesitamos mayor detalle. Hacemos click en **View** y se despliegan opciones: Easy, Text, HTML, entre otras. 

![alt text](/assets/tutoriales/mediainfoview.png "Inspector Media Info")

Una opción fácil de ver es HTML:

![alt text](/assets/tutoriales/mediainfohtml.png "Inspector Media Info Vista HTML")



## Parte 3: Analizar la información

Tomando como ejemplo la vista **Easy** encontramos 13 campos que describen los detalles más importantes del archivo.

![alt text](/assets/tutoriales/specsmediainfo.png "Datos Media Info")

1. Ruta del archivo
2. Formato y tamaño del archivo
3. Duración
4. Detalle del formato de video
5. Detalle del formato de audio
6. Bit Rate de video
7. Resolución en píxeles y relación de aspecto (Aspect Ratio)
8. Cuadros por segundo (Frames per second)
9. Bit Rate de audio
10. Sample Rate de audio en Hertz
11. Depth Rate 
12. Cantidad de canales
13. Formato de audio

**Es de importancia fundamental analizar:**

- Formato de video: para saber si es un formato editable.
- Bit Rate: para tener archivos con calidad suficiente y también estimar el tamaño final del video.
- Resolución: para entender si el tamaño de la imagen es adecuado o si será necesario escalar la imagen influyendo así en la pérdida de definición.
- Cuadros por segundo: para saber si es apropiado para el formato que deseamos exportar.
- Sample Rate: Un valor bajo equivale a una mala calidad del sonido.
- Depth Rate: Idealmente mayor a 16 bits.
- Canales: ya que si es mono tendremos que transformar el sonido para que suene stéreo o multicanal.