# telecom-analysis
# Objetivo del proyecto

Observar los datos de la empresa de telecomuniaciones ConnectaTel e identificar patrones de uso, detectar comportamientos atípicos y comprender qué segmentos de clientes muestran necesidades diferenciadas, con el fin de optimizar la oferta comercial y mejorar la experiencia del usuario.

Mediante técnicas de exploración, limpieza, transformación y visualización de datos, se busca identificar patrones relevantes en los usuarios, analizar diferencias entre los planes y comprender variables relacionadas con la permanencia o cancelación del servicio.

El análisis permitirá obtener conclusiones basadas en los datos y desarrollar habilidades prácticas en el proceso completo de análisis de datos.

# Datasets utilizados

## plan 
los planes actuales (precio, minutos incluidos, GB incluidos, costo por extra).

## users
información de clientes: edad, ciudad, fecha de registro, plan contratado.

## usage
el detalle de uso real: llamadas (duración) y mensajes (longitud).

# Etapas del análisis realizadas
## Exploración inicial

Se realizó una revisión de cada dataset para conocer:

Número de filas y columnas.
Nombres de las variables.
Tipos de datos.
Valores ausentes.
valores atipicos
Estadísticas descriptivas.

## Limpieza y preparación de los datos

Se identificaron inconsistencias y valores ausentes.

En el dataset users se encontraron valores nulos principalmente en:

city: 469 valores nulos.
churn_date: 3534 valores nulos.

Los valores ausentes fueron analizados teniendo en cuenta el significado de cada variable antes de decidir el tratamiento correspondiente.

En el caso de churn_date, los valores nulos representan usuarios que no registran una fecha de cancelación, por lo que no deben ser reemplazados automáticamente por un valor artificial.

Para city, se evaluó la cantidad de valores faltantes y su posible impacto sobre el análisis antes de determinar el tratamiento adecuado.

## Limpieza de datos

Se realizaron las transformaciones necesarias para facilitar el análisis, incluyendo:

Conversión de variables a los tipos de datos apropiados.
Creación de variables derivadas cuando fue necesario.
Organización de la información para realizar agrupaciones y comparaciones.
Preparación de los datos para la construcción de gráficos.

## Análisis exploratorio

Se analizaron diferentes variables para comprender el comportamiento de los usuarios.

Entre los análisis realizados se encuentran:

-Distribución de usuarios según el plan.
-Comparación entre planes.
-Distribución de las variables numéricas.
-Identificación de posibles valores atípicos.
-Análisis de la distribución de los datos.
-Comportamiento de los usuarios según diferentes características.

Se utilizaron estadísticas descriptivas como media, mediana, desviación estándar y percentiles cuando fueron pertinentes.

## Visualización de datos

Para facilitar la interpretación de los resultados se utilizaron diferentes tipos de gráficos, entre ellos:

Histogramas.
Gráficos de barras.
Diagramas de caja (boxplots).

Las visualizaciones permitieron identificar diferencias entre los planes, concentraciones de datos, posibles valores atípicos y sesgos en algunas distribuciones.

## Interpretación y conclusiones

Finalmente, se interpretaron los resultados obtenidos a partir de las tablas y visualizaciones.

Las conclusiones se formularon teniendo en cuenta únicamente los patrones observados en los datos, evitando asumir comportamientos que no pudieran ser respaldados por la información disponible.

# Herramientas utilizadas

El proyecto fue desarrollado principalmente con Python y las siguientes herramientas:

Pandas: manipulación, limpieza y análisis de datos.
NumPy: operaciones numéricas.
Matplotlib: creación de visualizaciones.
Jupyter Notebook / Google Colab: desarrollo y ejecución del proyecto.

# Cómo ejecutar el notebook

El proyecto puede ejecutarse fácilmente en Google Colab.

## Paso 1. Abrir Google Colab

Ingresar a Google Colab y seleccionar:

Archivo → Abrir cuaderno → Subir

Luego seleccionar el archivo .ipynb del proyecto.

## Paso 2. Cargar los datasets

Cargar en el entorno de Colab los archivos .csv utilizados en el proyecto.

Es importante conservar los nombres de los archivos o modificar las rutas dentro del código para que coincidan con los archivos cargados.

## Paso 3. Ejecutar el notebook

Ejecutar las celdas en el orden en que aparecen.

También se puede utilizar:

Entorno de ejecución → Ejecutar todas

## Paso 4. Revisar los resultados

Al ejecutar el notebook se generarán:

-Tablas de exploración.
-Estadísticas descriptivas.
-Resultados de la limpieza.
-Gráficos.
-Análisis de las variables.
-Conclusiones del proyecto.

# Guía breve para reproducir el análisis

Para reproducir correctamente el proyecto se debe seguir el siguiente flujo:

1. Cargar los datasets

2. Explorar la información

3. Revisar tipos de datos y valores ausentes

4. Limpiar y preparar los datos

5. Transformar las variables necesarias

6. Realizar el análisis exploratorio

7. Construir las visualizaciones

8. Interpretar los resultados

9. Elaborar las conclusiones

# Resultado esperado

Al finalizar la ejecución se obtiene un análisis estructurado del comportamiento de los usuarios, acompañado de tablas, estadísticas y visualizaciones que permiten identificar patrones y diferencias entre los planes y las características analizadas.

Este proyecto hace parte del proceso de formación en Analista de Datos de TripleTen y permite aplicar conocimientos de limpieza, exploración, análisis y visualización de datos utilizando Python.
