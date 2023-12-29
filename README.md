# Seduccion algoritmica: Explorando las fronteras del flirteo entre modelos de lenguaje y humanos en el ciberespacio
Trabajo Fin de Master de Ciencia de Datos de la UOC - 2023

Este trabajo explora la intersección entre la inteligencia artificial (IA) y la interacción
humana en el terreno de las citas en línea, cuestionando si un modelo de lenguaje
natural (LLM) puede “ligar” de manera eficaz en una plataforma de citas. El modelo
LLM utiliza aprendizaje por refuerzo en el contexto de un juego, el modelo aprende
al recibir “recompensas” cuando la acción que realiza es correcta. Este concepto se
puede aplicar en el contexto de las citas online, donde la recompensa es un “match”.
La metodología se centra en el diseño y optimización de prompts para que el modelo
tenga éxito en la plataforma. Para ello, se parte de un análisis previo de una base de
datos de citas, que se utiliza para enseñar al modelo cómo se presentan las personas
y en qué casos tienen éxito. Estos datos se usan para refinar las prompts con el
objetivo que el modelo genere perfiles no-humanos para presentarse en la
plataforma. El mismo modelo evaluará qué perfil le resulta más atractivo, si el humano
o el generado por la Inteligencia Artificial. Este estudio pretende arrojar luz sobre las
capacidades y limitaciones de la inteligencia artificial en el ámbito de las interacciones
humanas, así como plantear preguntas filosóficas sobre la autenticidad, la emulación
del afecto y el futuro de las relaciones humanas en una era cada vez más
automatizada.

## Contenido

Este repositorio contiene varios ficheros con formato ipnyb:

* Seduccion_algoritmica_1.ipynb - contiene la parte del Análisis Exploratorio de Datos y se debe ejecutar en Jupyter Notebook usando el fichero environment.yml
* Seduccion_algoritmica_2.ipynb - contiene todo el trabajo realizado con LLMs. Debido a la alta carga de procesamiento se recomienda utilizar Google Colab
* Seduccion_algoritmica_GPT-NEO 1.3B.ipynb - contiene las pruebas realizadas con GPT-NEO
* Seduccion algoritmica_Mistral.ipynb - contiene las pruebas realizadas con Mistral 7B
* Seduccion algoritmica_Zephyr.ipynb - contiene las pruebas realizadas con Zephyr 7B

En la carpeta files se encuentran varios de los ficheros de salida de este proceso:

* final_results.csv - contiene los resultados finales del procesamiento
* ngram_frequencies_by_cluster.csv - contiene los cuatrigramas por columna de essay y clúster BERT
* ngram_results.csv - contiene los cuatrigramas por columna de essay y clúster categórico
* profiles_per_cluster_2.csv - contiene los perfiles destilados y el output del LLM

Debido al tamaño del conjunto de datos utilizado, la mayoría de los ficheros no se pueden copiar en este repositorio, pero se pueden obtener todos ellos ejecutando los notebooks adjuntos.

## Instalación del Entorno
Para instalar y activar el entorno para ejecutar seduccion_algoritmica_1.ipynb, use los siguientes comandos:

conda env create -f environment.yml
conda activate mi_entorno

Para la ejecución del resto de notebooks se recomienda una máquina A100 de Google Colab con alta capacidad de memoria, lo que requeriría una suscripción Pro como mínimo.
