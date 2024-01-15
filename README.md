# ML-clasificacion-mushrooms

Este código realiza una serie de pasos comunes en la construcción y evaluación de un modelo de clasificación utilizando un conjunto de datos de hongos (mushrooms).

Carga de datos y exploración:

El código utiliza un conjunto de datos de hongos desde el repositorio de datos de la UCI.
Se examina la información de las variables y se muestra la información básica del DataFrame, incluyendo la presencia de valores nulos.
Tratamiento de valores nulos:

Se identifica la cantidad de valores nulos en la columna 'stalk-root' y se muestra una descripción de esta columna.
Se reemplazan los valores nulos en 'stalk-root' con la moda de esa columna.
Se muestra un gráfico de barras antes y después del tratamiento de valores nulos.
Análisis visual de variables:

Se muestra un gráfico de barras para la variable 'stalk-root' con respecto a la clase 'poisonous'.
Eliminación de variables:

La columna 'stalk-root' se elimina del DataFrame debido a la presencia de una gran cantidad de valores nulos.
División del conjunto de datos:

Se divide el conjunto de datos en conjuntos de entrenamiento y prueba.
Preprocesamiento de variables categóricas:

Se utiliza ColumnTransformer para aplicar codificación one-hot a las variables categóricas.
Entrenamiento del modelo de árbol de decisión:

Se entrena un modelo de árbol de decisión con ciertos hiperparámetros.
Evaluación del modelo en el conjunto de prueba:

Se realizan predicciones en el conjunto de prueba y se evalúa el modelo utilizando métricas como precisión, F1-score y accuracy.
Validación cruzada:

Se realiza validación cruzada con 10 folds y se muestra la precisión de cada fold y la precisión media.
Búsqueda de hiperparámetros:

Se realiza una búsqueda de hiperparámetros para encontrar el mejor valor de ccp_alpha (parámetro de complejidad del modelo) utilizando GridSearchCV.
Evaluación del modelo final:

Se evalúa el modelo final en el conjunto de prueba después de la búsqueda de hiperparámetros.
En resumen, el código aborda la carga de datos, tratamiento de valores nulos, visualización, entrenamiento de un modelo de árbol de decisión, evaluación del modelo, validación cruzada, búsqueda de hiperparámetros y evaluación del modelo final. Este flujo es típico en el proceso de construcción y evaluación de modelos de aprendizaje automático.






