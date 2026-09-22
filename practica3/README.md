# <center> Practica 3: Polars </center>

## <center>Integrantes <center>

<center>

| Nombre                         | Número de cuenta |
|:------------------------------:|:----------------:|
| Vega Navas Saúl                | 322088267        |
| Cimmino Yáñez Nicholas Joseph  | 322490712        |
| Benítez Pérez Kristian Leonel  | 322011346        |
| Herrera Cuamatla Jennifer Jade | 322255481        |

</center>

## Objetivo

En esta práctica se pondrá aprueba y a evaluación los siguientes puntos:

+ Aprender a estructurar correctamente un proyecto de mineria de datos
+ Seleccionar un framework de análisis de datos de manera correcta según el problema y los datos a analizar
+ Aplicar un preprocesamiento de los datos (normalización, eliminación de duplicados, conversión de tipos de datos e imputación) dados. 
+ Calcular e interpretar medidas de localización y variabilidad para un análisis exploratorio.

##  Fuente de los datos

La fuente de datos  oficial se obtuve del gobierno mexicano sobre violencia contra las mujeres, que esta disponible en este [enlace](https://www.inegi.org.mx/programas/endireh/2021/), en la sección de Microdatos, donde se descargó la base de datos en formato _csv_  y se juntó todos los archivos en un solo archivo csv, así como tambien se descargo el descriptor de archivos en formato _pdf_.

##  Instalación del entorno

Para poder instalar el entorno para ejecutar el programa es necesario ejecutar en la terminal
lo siguiente:

#### Windows:
```
python -m venv venv
pip install -r requirements.txt 
```

#### Mac o Linux:
```
python3 -m venv venv
pip install -r requirements.txt
```

## Ejecutar el  pipeline
Desde `proyecto-endireh-violencia`, para ejecutar el codigo de Preprocesamiento

#### Windows:
```
python -m src.cleaning.preprocessing 
```
#### Mac o Linux:
```
python3 -m src.cleaning.preprocessing
```

Para ver que hacen los Jupyter notebook, basta con abrirlos con VSCode o con cualquier otro lector de Jupyter notebook.

En el reporte se encuentra todos los Jupyter notebooks con sus respectivos resultados de cada codigo ejecutado.


# Cuestionario sobre la práctica

#### 1. 

#### 2.

#### 3.

#### 4. Se comparó la media simple de edad primer union contra la media ponderada por 'factor_expansion'. ¿Por qué pueden diferir? ¿Cuál de las dos deber ́ıa reportarse si el objetivo es describir a la población nacional y no solo a la muestra encuestada?

**R.**
    Las cifras difieren porque la media simple asume erróneamente que cada persona en la base de datos tiene exactamente la misma probabilidad de haber sido encuestada, lo que hace que todos los registros tengan la misma validez; no obstante, el factor de expansión añade valores de importancia para abarcar los efectos del encapsulamiento de sectores poblacionales completos en representaciones que, sin dicho factor, se consideran para una única persona.

    Es por esto que, al buscar describir no solo al conjunto de personas entrevistadas, sino a la población nacional, se debe reportar la media ponderada, pues las cantidades de personas consideradas que ésta engloba permiten reflejar al país completo con proporciones más acertadas.

#### 5. Si el coeficiente de variación de edad_primer_union resulta considerablemente más alto en el grupo que reportó violencia de pareja que en el que no, ¿qué hipótesis plantearíamos para explicarlo, y qué otra variable del dataset ayudaría a confirmarla o descartarla?

**R.**
    Si la situación es verdadera, entonces podemos plantear una hipótesis sobre la distribución, declarando que la concentración de situaciones de violencia de pareja no se da hacia un rango de edades concreto, sino que puede ser una mezcla entre las edades consideradas como tempranas, por causas derivadas de la alta vulnerabilidad de esos sectores; y las consideradas como comunes, por causas diferentes a las primeras mencionadas.

    Esto se puede respaldar o refutar con factores como estrato_socioeconomico y nivel_escolaridad, pudiendo confirmar si las uniones a edades tempranas se asocian con situaciones de bajos recursos y baja escolaridad, o si, por el contrario, dichos valores tienen baja heterogeneidad a lo largo del intervalo de edades.