# Mineria-grandes-volumenes
Repositorio para el trabajo final de mineria de grandes volumenes

## SISTEMA DE RECOMENDACIÓN DE CANCIONES

Este repositorio contiene el desarrollo y los resultados del trabajo final de mineria de grandes volumenes de datos para el semestre 2020-02 de la Maestria en ciencia de los datos y analítica de la universidad EAFIT.

Los estudiantes que presentan este trabajo son:

Álvaro Villa Vélez

Luis Rodrigo Vesga Vesga

Jorge Luis Rentería Roa

Edgar Leandro Jiménez Jaimes

Santiago Echeverri Calderón


Este trabajo consiste en identificar las canciones similares basados en los gustos de grupos y/o individuos parecidos a través de la aplicación de sistemas de recomendación sobre grandes volúmenes de datos.

Objetivos específicos:
-	Adecuar los ambientes técnicos de modelación y almacenamiento en AWS.
-	Analizar el comportamiento histórico de los datos y su distribución estadística.
-	Seleccionar una métrica de similaridad entre canciones.
-	Implementar un modelo para recomendar canciones relevantes para un usuario, dada la música que el usuario escucha.
-	Medir el desempeño del sistema de recomendación.

Para el proyecto se utilizaron 2 datasets del proyecto Million Songs Dataset (MSD, disponible en: http://millionsongdataset.com).  El primero es el dataset principal MSD, el cual contiene los metadatos para 1 millón de canciones.  El segundo consiste en el conjunto “Taste Profile subset”, el cual contiene información de reproducciones de canciones por usuario en tripletas (usuario-cancion-reproducciones).

Originalmente considerábamos que podíamos obtener más información del dataset de canciones, pues en la documentación se referenciaban 46 atributos.  Pero la distribución del dataset es a través de un snapshot de disco para una instancia EC2 de AWS y si bien pudimos adjuntar el snapshot a una instancia, no pudimos extraer la información para ponerla disponible en S3 o en otro medio que nos permitiera tener el almacenamiento distribuido para consumirlo desde el cluster.


## Carpetas del repositorio

Este repositorio cuenta con tres carpetas y un archivo en PDF.

* Carpeta Dataset: Se encuentran los datos que se utilizaron para la modelación, estos datos son una submuestra ya que el tamaño original es mas grande. Adicionalmente se encuentran los archivos en csv que resultaron de la partición de los datos.

* Carpeta Modelación: Contiene 3 libros de jupyter con los codigos que se utilizaron durante la solución del proyecto, el primero de partición de los datos, el segundo hace referencia a la modelación y el ultimo a la evaluacion del modelo.

* Carpeta Resultados Muestra: Contiene unos archivos resultados del modelo y la evaluación, esto es solo una muestra pequeña de todos los resultados, la totalidad de los resultados se encuentran almacenados en S3.

* Archivo PDF: Trabajo entregado con la solución y resultados del proyecto.
