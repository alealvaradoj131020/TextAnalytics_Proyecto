# Text Analytics: Proyecto Final
## Master en Business Intelligence and Analytics - UVG

### Integrantes
* Carlos Rivera - 251518
* Daniel Cabrera - 252136
* Alejandra Alvarado - 18263

---

### Descripción del Proyecto
Este proyecto consiste en el desarrollo de un pipeline inteligente para el procesamiento y análisis de grandes volúmenes de texto (NLP), aplicado a la retroalimentación de clientes en plataformas de e-commerce. Se diseñó una solución que combina **Aprendizaje Supervisado** (para clasificar emociones) y **Aprendizaje No Supervisado** (para descubrir temas ocultos), permitiendo una visión de 360 grados sobre la opinión del consumidor.


---


### El Dataset y Fuente de Datos

Los datos utilizados para este estudio provienen de un repositorio público de **Amazon Reviews**, una fuente estándar en la industria para el entrenamiento de modelos de procesamiento de lenguaje natural.

*   **Fuente:** [PyCaret Public Datasets](https://github.com/pycaret/pycaret/blob/master/datasets/amazon.csv)
*   **Volumen de datos:** El dataset original cuenta con miles de registros. Para este análisis, hemos procesado una muestra de **20,000 reseñas**, asegurando una representatividad estadística adecuada.
*   **Contenido:** Incluye el texto íntegro de la reseña (`reviewText`) y una etiqueta de sentimiento pre-definida (`Positive`), lo que permite el entrenamiento y validación de modelos de clasificación binaria.


---


### Caso de Negocio: Inteligencia de Clientes en Amazon

En un ecosistema global como el de Amazon, el volumen de retroalimentación diaria es masivo, haciendo imposible la lectura manual de cada comentario. El problema de negocio que resolvemos es la **falta de visibilidad accionable sobre la experiencia del usuario**.

**Este análisis permite:**
1.  **Detección Automática de Sentimiento:** Identificar reseñas negativas en tiempo real para activar protocolos de servicio al cliente de manera prioritaria.
2.  **Identificación de Tópicos Críticos:** A través del modelado LDA, la empresa puede descubrir si las quejas se deben a fallas en el hardware (Kindle), problemas de software (Apps) o deficiencias en el contenido (Libros/Juegos).
3.  **Optimización de Productos:** Al entender no solo *si* al cliente le gusta el producto, sino *por qué* (tópicos), la gerencia puede tomar decisiones informadas sobre futuras actualizaciones y lanzamientos.


---

### Cómo ejecutar este proyecto
Para garantizar la reproducibilidad y facilitar la revisión, el proyecto se encuentra listo para ser ejecutado en **Google Colab**.

1. Haz clic en el siguiente enlace para abrir el notebook:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/alealvaradoj131020/TextAnalytics_Proyecto/blob/main/ProyectoTextAnalytics.ipynb)

2. Ejecuta las celdas en orden secuencial. El código descarga automáticamente el dataset desde una fuente remota (no requiere carga de archivos locales).

---

### Tecnologías y Librerías Utilizadas
* **Lenguaje:** Python 3.x
* **Procesamiento de Texto:** NLTK (Tokenización, Stopwords, Lemmatization), Regex.
* **Modelado y ML:** Scikit-learn (TF-IDF, Naive Bayes, Logistic Regression).
* **NLP Avanzado:** Gensim (LDA para Topic Modeling).
* **Visualización:** Matplotlib, Seaborn, WordCloud.

---

### Estructura del Repositorio
* `Proyecto_Final_Text_Analytics.ipynb`: Notebook principal con todo el pipeline de datos, desde la limpieza hasta la inferencia.
* `README.md`: Descripción técnica del repositorio.

> **Nota:** El análisis detallado del caso de negocio, las métricas comparativas finales y las conclusiones estratégicas se encuentran detalladas en el **Documento de Resultados Formal** entregado por separado.
