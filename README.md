# 🎓 Maestría en Inteligencia Artificial (MIA)

Bienvenido al repositorio central de trabajos, tareas, laboratorios, proyectos de investigación y código desarrollados a lo largo de la **Maestría en Inteligencia Artificial**.

---

## 👤 Información del Estudiante

- **Autor:** Rafael Arana
- **Programa:** Maestría en Inteligencia Artificial (MIA)
- **Institución:** Universidada Autonoma de Yucatan (UADY)
- **Propósito:** Registro académico, control de versiones y portafolio de proyectos de posgrado.

---

## 🗂️ Estructura del Repositorio

La organización del repositorio está estructurada por semestres y asignaturas para mantener un orden modular y claro:

```text
master_ai/
├── Primer_Semestre/
│   ├── [Nombre_Materia_1]/
│   │   ├── tareas/
│   │   ├── proyectos/
│   │   └── notebooks/
│   └── [Nombre_Materia_2]/
├── Segundo_Semestre/
│   └── ...
├── Tercer_Semestre/
│   └── ...
├── Cuarto_Semestre/
│   └── ...
├── Investigacion_Tesis/
│   ├── datos/
│   ├── experimentos/
│   └── documentacion/
├── .gitignore
└── README.md
```

---

## 🔬 Áreas de Estudio y Temáticas

- 🧠 **Aprendizaje Automático (Machine Learning):** Modelos supervisados, no supervisados y ensamble.
- ⚡ **Aprendizaje Profundo (Deep Learning):** Redes neuronales convolucionales (CNN), recurrentes (RNN), Transformers y modelos generativos.
- 👁️ **Visión por Computadora (Computer Vision):** Detección de objetos, segmentación y clasificación de imágenes.
- 🗣️ **Procesamiento de Lenguaje Natural (NLP):** LLMs, embeddings, análisis de sentimientos y recuperación de información.
- 📊 **Matemáticas y Optimización para IA:** Álgebra lineal, probabilidad, estadística multivariada y algoritmos de optimización.
- ⚙️ **MLOps & Despliegue:** Pipelines de datos, experiment tracking y despliegue de modelos.

---

## 🛠️ Tecnologías y Herramientas

| Categoría | Tecnologías / Librerías |
| :--- | :--- |
| **Lenguajes** | Python, R, C++ |
| **Deep Learning & ML** | PyTorch, TensorFlow / Keras, Scikit-Learn, XGBoost, LightGBM |
| **Procesamiento de Datos** | NumPy, Pandas, Polars, SciPy |
| **Visualización** | Matplotlib, Seaborn, Plotly |
| **NLP & LLMs** | Hugging Face (`transformers`), LangChain, LlamaIndex, NLTK, spaCy |
| **Visión Artificial** | OpenCV, torchvision, Albumentations |
| **Entorno & Herramientas** | Jupyter Notebook / Lab, Google Colab, Conda / Poetry, Docker, Git |

---

## 🚀 Guía de Inicio y Configuración

### 1. Clonar el repositorio
```bash
git clone https://github.com/alcatere/master_ai.git
cd master_ai
```

### 2. Configurar el entorno virtual

Con **Python `venv`**:
```bash
python -m venv .venv
source .venv/bin/activate  # En macOS / Linux
# .venv\Scripts\activate   # En Windows
pip install -r requirements.txt
```

O con **Conda**:
```bash
conda create -n master_ai python=3.11
conda activate master_ai
```

---

## 📌 Convención de Commits y Trabajo

- `feat:` Nuevos algoritmos, modelos o implementación de tareas.
- `fix:` Corrección de errores en scripts o notebooks.
- `docs:` Actualización de documentación, notas o reportes.
- `refactor:` Optimización y limpieza de código.
- `data:` Adición o scripts de preprocesamiento de datasets.

---

## 📜 Licencia y Uso Académico

Este repositorio tiene fines primordialmente académicos y formativos. El código y los documentos aquí contenidos reflejan el trabajo individual y colaborativo desarrollado durante el posgrado.