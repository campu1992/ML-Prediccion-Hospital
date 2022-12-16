
# Proyecto Individual Lab-02 Machine Learning

El siguiente proyecto consiste en dar solución a un problema propuesto por un hospital.

Nos proporcionan dos archivos, uno para Train y otro para Test. Ambos archivos contienen información relevante acerca de los pacientes que ingresan al hospital.


## Objetivo

El objetivo del proyecto es en primer lugar afianzar los conceptos que se vieron en el módulo de Machine Learning en Henry.

En segundo lugar es incentivarnos a investigar más acerca de Machine Learning y tener un acercamiento práctico del desarrollo de modelos de aprendizaje automático y tener un acercamiento a lo que podría ser un entorno de trabajo real.

## Problema

El problema que se nos entrega, consiste en un hospital que tiene unos altos costos al tener pacientes con estancias prolongadas y un problema que también puede ser de salud pública, ya que, la saturación en un hospital puede traer grandes consecuencias.

Como solución a este problema debemos proponer una forma de predecir con una alta probabilidad si un paciente estará en una estancia prolongada y permitirle al hospital tomar decisiones acertadas.

## Información para el desarrollo del modelo

La Información que tenemos para el desarrollo del modelo son dos datasets con Información relevante acerca de cada paciente y variables que nos pueden indicar una relación con la cantidad de tiempo que puede estar un paciente hospitalizado en una estancia prolongada.

Las dimensiones que nos proporcionan son las siguientes:

- Available Extra Rooms in Hospital: Habitaciones adicionales disponibles en el hospital. Una habitación no es igual a un paciente, pueden ser individuales o compartidas.
- Department: Área de atención a la que ingresa el paciente. 
- Ward_Facility_Code: Código de la habitación del paciente.
- doctor_name: Nombre de el/la doctor/a a cargo del paciente.
- staff_available: Cantidad de personal disponible al momento del ingreso del paciente.
- patientid: Identificador del paciente.
- Age: Edad del paciente.
- gender: Género del paciente.
- Type of Admission: Tipo de ingreso registrado según la situación de ingreso del paciente.
- Severity of Illness: Gravedad de la enfermedad/condición/estado del paciente al momento del ingreso.
- health_conditions: Condiciones de salud del paciente. 
- Visitors with Patient: Cantidad de visitantes registrados para el paciente.
- Insurance: Indica si la persona posee o no seguro de salud. 
- Admission_Deposit: Pago realizado a nombre del paciente, con el fin de cubrir los costos iniciales de internación. 
- Stay (in days): Días registrados de estancia hospitalaria.

## Pasos para el desarrollo del modelo

1. Se hace un análisis exploratorio de la información provista para poder analizar con qué información se cuenta y si realmente ésta información podría llegar a arrojarnos un resultafos satisfactorio.
2. Se procede a visualizar a través de la libreria pandas la información de todo el dataset de forma detallada, se verifican si hay nulos, se verifica si hay filas repetidas.
3. Se visualiza a través de librerias como Numpy y Seaborn de manera gráfica la distribución de variables en particular y la correlación existente entre las dimensiones dadas con la columna objetivo para establecer cuáles son las columnas que se deben borrar.
4. Se procede a categorizar las variables para convertirlas a binarias , para de esta forma poder trabajar con los algoritmos de predicción.
5. Se procede a realizar una selección estable de variables independientes con RFE, realizamos un ranking de las variables y seleccionamos las que vamos a trabajar.
6. Divido el dataset con train_test_split.
7. Selecciono el modelo de regresión logistica debido a que se quiere predecir la probabilidad de que un evento ocurra en base a una serie de variables predictoras.
8. Entreno el modelo y realizo la predicción.
9. Realizo una matriz de confusión, mido el accuracy y el recall.
10. Uso RandomizedSearch con un arbol de decisión.
11. Entreno el modelo y hago la predicción.
12. Hago una matriz y reviso el accuracy y el recall para ver si hubo una mejora con respecto a la regresión lineal.
13. Exporto las diferentes predicciones en una columna pred para enviar a dashboard y medir en diferentes ocasiones el cambio en las metricas de rendimiento.

## Librerias y herramientas utilizadas en el proyecto

- Python
- Sci-kit learn
- Pandas 
- Numpy 
- Seaborn
- Matplotlib
- Github
- Colab

## Conclusiones 

Tener un acercamiento a Machine Learning a través de éste proyecto ha sido muy importante, ya que, he visto principalmente la gran utilidad que tiene para resolver problemas. ésto me reto y me hizo investigar demasiado y sobretodo me divertí bastante tratando de mejorar el modelo y compitiendo con mis compañeros. De lejos puedo decir que es la parte que mas me ha gustado de el bootcamp y a pesar de no haber podido subir las métricas me han quedado bastantes conocimientos.

Una conclusión muy importante en cuanto a lo técnico es que se le debe dedicar bastante tiempo al analisis exploratorio, ya que, se pueden usar diferentes algoritmos, entrenar redes neuronales pero si la información que se está usando no es la mas óptima va a ser muy dificil encontrar un resultado exploratorio.
