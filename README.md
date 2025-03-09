# PredicciónMeteorológica
> Proyecto 3 Master IABD 
Video del funcionamiento del modelo: https://youtu.be/3THhk-Xl0go
## Que hace este proyecto?
El objetivo de este proyecto es extraer los datos de diferentes fuentes mediante descargas o web scrapping, modificación y homogenización de los datos para su uso en los modelos, el uso de herramientas de visualización como PowerBI o Tableau y el manejo de series temporales y como hacer predicciones sobre ellas. 

## Estructura del proyecto
El proyecto está dividido en diferentes carpetas y archivos que guardan desde los datos para entrenar y probar los modelos, la documentación y los diferentes archivos con código sobre modelos.  
- Carpeta Data:  
    Carpeta que contiene los datos raw, homogenizados y transformados que se utilizarán a lo largo del proyecto.  
    * Carpeta raw:    
          Esta carpeta contiene los datos sacados y sin modificar de cada una de las fuentes usadas, las subcarpetas corresponden a las fuentes utilizadas y dentro de estas están los datos.  
    * Carpeta homgenized:    
          Esta carpeta contiene los datos despues de los primeros cambios, ahora los datos han sido alterados para solo tener las columnas necesarias de base.  
          Las subcarpetas dividen los datos por diarios o horarios, y dentro de cada una estarán los datos guardados en formato parquet, esto se hace automaticamente desde un archivo jupyter.  
    * Carpeta transformed:    
          Esta carpeta contiene los datos que han sido transformados y usados en los diferentes modelos de predicción.  
          Las subcarpetas dividen los datos por diarios o horarios, y dentro de cada una estarán los datos guardados en formato parquet, esto se hace automaticamente desde un archivo jupyter.   
- Carpeta Doc:  
      Contiene los archivos de documentación del proyecto tanto en formato docx como en pdf para poder leer desde github.
- Carpeta Src:  
    * Carpeta EDA:  
            Carpeta que contiene los 2 archivos usados como Analisis Exploratorio de los Datos (EDA).
    * Carpeta ETL:  
            Carpeta que contiene los archivos utilizados para la homogeneización y transformación de los datos.  
            Estos archivos estan hechos con PySpark y tambien se encargan de guardar los datos en formato parquet.
    * Carpeta modeling:  
            Carpeta que contiene los archivos jupyter con los modelos que se han utilizado para las predicciones de datos.
    * Carpeta pruebas:  
            Esta carpeta contiene los primeros archivos que empezamos a crear cuando se inició el proyecto.  
            Estos estan llenos de pequeñas pruebas que algunas se han transladado a otros ficheros.
