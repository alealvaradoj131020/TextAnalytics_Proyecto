# Text Analytics: Proyecto Final
## Master en Business Intelligence and Analytics - UVG

### Integrantes
* Carlos Rivera - 251518
* Daniel Cabrera - 252136
* Alejandra Alvarado - 18263

---

### Descripción del Proyecto
Este proyecto desarrolla un pipeline avanzado aplicado a la retroalimentación de clientes de Amazon. La solución es integral, combinando tres enfoques metodológicos:
1.  **Análisis basado en reglas léxicas:** Uso de **VADER** como modelo base (baseline).
2.  **Aprendizaje Supervisado:** Comparativa entre **Naive Bayes** y **Regresión Logística** para clasificación de sentimiento.
3.  **Aprendizaje No Supervisado:** Descubrimiento de temas mediante **Modelado de Tópicos (LDA)**.

El flujo incluye desde la limpieza profunda hasta la interpretabilidad de modelos y análisis de métricas avanzadas (Curva ROC).


---


### El Dataset y Fuente de Datos

Los datos utilizados para este estudio provienen de un repositorio público de **Amazon Reviews**, una fuente estándar en la industria para el entrenamiento de modelos de procesamiento de lenguaje natural.

*   **Fuente:** [PyCaret Public Datasets](https://github.com/pycaret/pycaret/blob/master/datasets/amazon.csv)
*   **Volumen de datos:** El dataset original cuenta con miles de registros. Para este análisis, hemos procesado una muestra de **20,000 reseñas**, asegurando una representatividad estadística adecuada.
*   **Contenido:** Incluye el texto íntegro de la reseña (`reviewText`) y una etiqueta de sentimiento pre-definida (`Positive`), lo que permite el entrenamiento y validación de modelos de clasificación binaria.


---


### Caso de Negocio: Inteligencia de Clientes en Amazon

En un ecosistema global como el de Amazon, el volumen de retroalimentación diaria es masivo, haciendo imposible la lectura manual de cada comentario. El problema resuelto es la falta de visibilidad accionable sobre el volumen masivo de retroalimentación diaria. 

**Este análisis permite:**
1.  **Detección Automática:** Clasificar sentimientos con una precisión superior al 88%.
2.  **Identificación de Tópicos Críticos:** Determinar si la satisfacción o quejas se derivan del hardware (Kindle), software (Apps) o contenido (Juegos/Libros).
3.  **Interpretabilidad:** Identificar qué palabras específicas (coeficientes) impulsan la percepción positiva o negativa del usuario.

---

### Cómo ejecutar este proyecto
Para garantizar la reproducibilidad y facilitar la revisión, el proyecto se encuentra listo para ser ejecutado en **Google Colab**.

1. Haz clic en el siguiente enlace para abrir el notebook:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/alealvaradoj131020/TextAnalytics_Proyecto/blob/main/ProyectoTextAnalytics.ipynb)

2. Ejecuta las celdas en orden. El código gestiona automáticamente la descarga del dataset y las librerías necesarias.

---

### Tecnologías y Librerías Utilizadas
* **Lenguaje:** Python 3.12+
* **Procesamiento de Texto:** NLTK (Tokenización, Stopwords, Lemmatization, VADER), Regex.
* **Modelado y ML:** Scikit-learn (TF-IDF, Naive Bayes, Logistic Regression, ROC Curve).
* **NLP Avanzado:** Gensim (LDA para Topic Modeling).
* **Visualización:** Matplotlib, Seaborn, WordCloud.

---

### Estructura del Repositorio
* `Proyecto_Final_Text_Analytics.ipynb`: Notebook principal con todo el pipeline de datos, desde la limpieza hasta la inferencia.
* `README.md`: Descripción técnica del repositorio.

> **Nota:** El análisis detallado del caso de negocio, las métricas comparativas finales y las conclusiones estratégicas se encuentran detalladas en el **Resultados_Proyecto** entregado por separado.
