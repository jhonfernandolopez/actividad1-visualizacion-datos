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

[`tablero/index.html`](tablero/index.html) — tablero de indicadores sobre la misma población: distribución por sexo, grupo etario, estamento, parentesco, etnia y evolución de afiliaciones por año (1990–2026). Abrir el archivo directamente en el navegador, o servirlo con GitHub Pages para un enlace público.
