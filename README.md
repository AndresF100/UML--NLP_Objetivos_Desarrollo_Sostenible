## Alcanzando los objetivos de desarrollo sostenible. Un aporte desde el machine learning.

### Introducción

En este proyecto se explora la aplicación de técnicas avanzadas de machine learning y procesamiento del lenguaje natural (NLP) para la clasificación automática de textos en los 16 Objetivos de Desarrollo Sostenible (ODS) de las Naciones Unidas. El objetivo principal es contribuir al monitoreo y evaluación de estos objetivos mediante el análisis automatizado de grandes volúmenes de texto.

### Descripción del proyecto

El proyecto se divide en las siguientes etapas:

**1. Preparación de datos:**

   - Se carga el conjunto de datos "OSDG Community Dataset" en formato Excel.
   - Se realiza una limpieza y preprocesamiento de los textos, incluyendo la eliminación de caracteres especiales, la conversión a minúsculas, la tokenización, la eliminación de stopwords y la lematización.
   - Se transforma el texto en una representación numérica utilizando la técnica CountVectorizer y TF-IDF para capturar la frecuencia y la importancia de las palabras en cada texto.
   - Se reduce la dimensionalidad de la matriz de representación de texto utilizando TruncatedSVD para mejorar la eficiencia computacional y evitar el overfitting.

**2. Modelado:**

   - Se implementa un pipeline de preprocesamiento que incluye las etapas descritas anteriormente.
   - Se entrenan y evalúan tres modelos de clasificación multiclase: Random Forest, SVM y XGBoost.
   - Se utiliza la técnica GridSearchCV para optimizar los hiperparámetros de cada modelo.
   - Se selecciona el modelo con mejor rendimiento en términos de precisión, recall y F1-score.

**3. Evaluación y análisis de resultados:**

   - Se compara el rendimiento de los diferentes modelos utilizando métricas como la precisión, el recall y la F1-score.
   - Se analiza la matriz de confusión del modelo seleccionado para identificar posibles errores de clasificación.
   - Se genera un reporte de clasificación detallado para cada modelo.

**4. Conclusiones y discusión:**

   - Se presentan los resultados obtenidos y se discuten los hallazgos del proyecto.
   - Se destacan las fortalezas y limitaciones del enfoque propuesto.
   - Se proponen direcciones futuras de investigación para mejorar el rendimiento de los modelos y ampliar su aplicabilidad.

### Tecnologías utilizadas

- Lenguajes de programación: Python
- Librerías: Pandas, Numpy, nltk, sklearn, matplotlib, seaborn

### Datos utilizados

- Conjunto de datos "OSDG Community Dataset" versión 2023, disponible en [https://github.com/sgugger/hf_examples/blob/main/text_classification.ipynb](https://github.com/sgugger/hf_examples/blob/main/text_classification.ipynb)


### Pasos para ejecutar el proyecto

1. Clonar el repositorio del proyecto en su ordenador.
2. Instalar las librerías requeridas utilizando el comando `pip install -r requirements.txt`.
3. Ejecutar el script `main.py` para ejecutar el proyecto completo.
4. Analizar los resultados generados en los archivos `report.csv` y `confusion_matrices.pdf`.

### Referencias

- OSDG Community Dataset
- [NLTK](https://www.nltk.org/)
- [scikit-learn](https://scikit-learn.org/)
- [Matplotlib](https://matplotlib.org/)
- [Seaborn](https://seaborn.pydata.org/)

### Nota

Este proyecto se encuentra en desarrollo y se espera que sea mejorado y ampliado en el futuro. Se invita a la comunidad a colaborar en este proyecto aportando ideas, sugerencias y código.
