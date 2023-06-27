## DESCRIPCIÓN:

El contenido de las carpetas es el siguiente:

* `1-preprocessing`: incluye los scripts utilizados para el preprocesado de los datos.

* `2-finite-element-model`: incluye el script desarrollado en PyMAPDL en el que se implementa el modelo de elementos finitos y se llevan a cabo las simulaciones. Incluye también los scripts (y algunos datasets que se han creado a modo de resumen) que permiten comparar las simulaciones con los perfiles de temperatura registrados por los pirómetros.

* `3-machine-learning-models`: incluye los scripts que implementan los modelos de ML basados en redes neuronales, a saber: el convolucional unidimensional, y el convolucional-recurrente. Además, contiene los modelos obtenidos en formato HDF5 y algunas de las gráficas usadas en la memoria.

* `4-energy-optimization`: incluye todo lo relativo al marco de trabajo de RL. En particular, se incluye el script utilizado para entrenar el agente (la DQN), los modelos obtenidos, así como algunas gráficas usadas en la memoria. También se incluyen los scripts en los que se aplica la política de toma de decisiones aprendida a los patrones de calentamiento de las palanquillas actualmente utilizados por GSW.
