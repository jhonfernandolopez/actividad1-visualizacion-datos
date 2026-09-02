# 📊 Proyecto final — Diplomado en Visualización de Datos y Creación de Tableros

**Universidad del Valle · Estudiante: Jhon Fernando López Tamayo**

Portafolio del proyecto final del diplomado: depuración de datos → análisis exploratorio → tablero, sobre un extracto anonimizado de afiliados activos de un servicio de salud universitario.

## 1. Depuración de datos

Script [`anonimizar.py`](anonimizar.py) sobre el extracto original del sistema de información:

- Filtra únicamente afiliados con estado **AC (activo)**.
- Corrige la codificación del archivo fuente y elimina una columna duplicada (`estado_afiliado_id`).
- Anonimiza el dataset antes de publicarlo: documento → hash consistente, nombres → seudónimos, contacto/dirección/correo → datos sintéticos.

Resultado: [`clase-2-eda/afiliados_activos_anonimo.csv`](clase-2-eda/afiliados_activos_anonimo.csv) — 5.454 afiliados activos, 39 columnas (edad, antigüedad de afiliación, estamento, plan, sexo, parentesco, etnia, entre otras).

## 2. Análisis exploratorio (EDA)

Notebook en R/tidyverse: [`clase-2-eda/Actividad1_JhonLopez.ipynb`](clase-2-eda/Actividad1_JhonLopez.ipynb)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jhonfernandolopez/actividad1-visualizacion-datos/blob/main/clase-2-eda/Actividad1_JhonLopez.ipynb)

## 3. Tablero

Tablero interactivo en **Gradio** (la herramienta del módulo 5) sobre la misma población: distribución por sexo, grupo etario, estamento, parentesco, etnia y evolución de afiliaciones por año (1990–2026).

Notebook: [`tablero_gradio/Tablero_Gradio_JhonLopez.ipynb`](tablero_gradio/Tablero_Gradio_JhonLopez.ipynb)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jhonfernandolopez/actividad1-visualizacion-datos/blob/main/tablero_gradio/Tablero_Gradio_JhonLopez.ipynb)

⚠️ Al abrir el notebook hay que **ejecutar todas las celdas** para que genere el enlace público (`*.gradio.live`) — ese enlace es temporal, vive solo mientras el notebook siga corriendo y expira solo a las 72 horas.

*(También queda disponible un tablero equivalente en HTML/JS puro, sin dependencias, como respaldo permanente: [`tablero/index.html`](tablero/index.html) — [en vivo aquí](https://jhonfernandolopez.github.io/actividad1-visualizacion-datos/tablero/).)*
