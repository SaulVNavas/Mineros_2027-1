# <center> Practica 3: Medidas de Heterogeneidad y Concentración.</center>

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

El objetivo de esta práctica es que el alumno, partiendo del dataset ENDIREH 2021 ya preprocesado en la Práctica 3 (data/data-processed/), calcule e interprete correctamente medidas de localización, medidas de variabilidad, medidas de heterogeneidad y medidas de concentración, incluyendo específicamente el coeficiente de Gini y la entropía de Shannon, y las comunique mediante visualizaciones de datos adecuadas. Más allá del cálculo mecánico, se busca que el alumno reflexione críticamente sobre lo que estas medidas revelan –y lo que ocultan– acerca del fenómeno de la violencia contra las mujeres, y sobre cómo estos hallazgos deben orientar decisiones posteriores del proyecto (mejoras al preprocesamiento, selección de variables para modelado, comunicación responsable de resultados).

##  Fuente de los datos

La fuente de datos  oficial se obtuve del gobierno mexicano sobre violencia contra las mujeres, que esta disponible en este [enlace](https://www.inegi.org.mx/programas/endireh/2021/), en la sección de Microdatos, donde se descargó la base de datos en formato _csv_  y se juntó todos los archivos en un solo archivo csv, así como tambien se descargo el descriptor de archivos en formato _pdf_.

## Instalación del entorno

Para poder instalar el entorno para ejecutar el programa es necesario ejecutar en la terminal
lo siguiente:

### Instalación de requerimientos
Dirigirse a la dirección `Mineros\2027-1/practica4`, acoplar el entorno de ejecución:

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
## Ejecutar el pipeline
Desde `Mineros\2027-1/practica4/proyecto-endireh-violencia`, ejecutar el codigo de Preprocesamiento:

#### Windows:
```
python -m config.rutas
python -m src.cleaning.preprocessing 
```
#### Mac o Linux:
```
python3 -m config.rutas
python3 -m src.cleaning.preprocessing
```

Para ver que hacen los Jupyter notebook, basta con abrirlos con VSCode o con cualquier otro lector de Jupyter notebook.

En el reporte se encuentra todos los Jupyter notebooks con sus respectivos resultados de cada codigo ejecutado.
