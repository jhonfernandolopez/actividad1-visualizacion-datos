# Proyecto final — Diplomado en Visualización de Datos y Creación de Tableros

Universidad del Valle · Jhon Fernando López Tamayo

Depuración, análisis exploratorio y tablero sobre un extracto anonimizado de afiliados activos de un servicio de salud universitario.

## 1. Depuración

[`anonimizar.py`](anonimizar.py): filtra afiliados con estado AC (activo), corrige la codificación del archivo fuente y anonimiza el dataset (documento a hash, nombres a seudónimos, contacto a datos sintéticos).

Resultado: [`clase-2-eda/afiliados_activos_anonimo.csv`](clase-2-eda/afiliados_activos_anonimo.csv) — 5.454 registros, 39 columnas.

## 2. Análisis exploratorio (EDA)

Notebook en R: [`clase-2-eda/Actividad1_JhonLopez.ipynb`](clase-2-eda/Actividad1_JhonLopez.ipynb)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jhonfernandolopez/actividad1-visualizacion-datos/blob/main/clase-2-eda/Actividad1_JhonLopez.ipynb)

## 3. Tablero

Tablero en Gradio: [`tablero_gradio/Tablero_Gradio_JhonLopez.ipynb`](tablero_gradio/Tablero_Gradio_JhonLopez.ipynb)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jhonfernandolopez/actividad1-visualizacion-datos/blob/main/tablero_gradio/Tablero_Gradio_JhonLopez.ipynb)

Hay que ejecutar todas las celdas para generar el enlace público. Dura 72 horas.

Respaldo permanente en HTML: [`tablero/index.html`](tablero/index.html) — [en vivo](https://jhonfernandolopez.github.io/actividad1-visualizacion-datos/tablero/).
