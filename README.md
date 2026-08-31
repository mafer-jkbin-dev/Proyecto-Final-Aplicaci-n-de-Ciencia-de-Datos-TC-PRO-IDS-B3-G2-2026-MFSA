# 📊 Insurance Cost Predictions App
Aplicación móvil desarrollada en MIT App Inventor para análisis, depuración y predicción de costos de seguros médicos mediante regresión lineal e integración con IA.

<p align="center">
  <img src="docs/App.png" width="200" alt="Preview de la App">
</p>
![Preview de la App](docs/App.png)

![Status](https://img.shields.io/badge/Status-Active-success)
![MIT App Inventor](https://img.shields.io/badge/MIT-AppInventor-blue)
![Google Sheets](https://img.shields.io/badge/Cloud-Google%20Sheets-green)
![Kaggle Dataset](https://img.shields.io/badge/Kaggle-Dataset-blue)
![Author](https://img.shields.io/badge/Author-María%20Fernanda%20Sánchez%20Alvarez-purple)

<h2><strong><em>📑 Tabla de Contenidos</em></strong></h2>
Descripción General

Características Principales

Dataset

Arquitectura de la Aplicación

Modelo Matemático

Retos Técnicos y Soluciones

Conclusiones

Tecnologías Utilizadas

Estructura del Proyecto

Autor

<h2><strong><em>🚀 Descripción General</em></strong></h2>
Pequeño resumen en viñetas para que se vea limpio:

Herramienta analítica para evaluar cómo edad, BMI y tabaquismo influyen en el costo de una póliza médica.

Consume datos en tiempo real desde Google Sheets.

Ejecuta limpieza de datos atípicos.

Traza la línea de mejor ajuste.

Genera predicciones financieras con apoyo de IA.

<h2><strong><em>✨ Características Principales</em></strong></h2>
🔐 Autenticación (Screen0)
Validación de credenciales

Control de acceso

🧭 Navegación Modular (Screen1)
Panel centralizado

Acceso a cada etapa analítica

🧹 Depuración de Datos (cleanDataScreen)
Filtrado de anomalías

Eliminación de registros inconsistentes

📈 Modelado Matemático (drawLOBFscreen)
Cálculo dinámico de M, B y R

🤖 Predicciones e IA (makePredictionsScreen)
Escenarios en tiempo real

Chatbot integrado

<h2><strong><em>📂 Dataset</em></strong></h2>
Fuente: Kaggle

Integración: Google Sheets

Muestra: 300 registros

Variables Clave
Variable	Descripción
age	Edad del usuario
bmi	Índice de Masa Corporal
charges	Prima del seguro
smoker	Indicador de tabaquismo


<h2><strong><em>🛠️ Arquitectura de la Aplicación</em></strong></h2>
Código
[Screen0: Login] ──> [Screen1: Menú Principal]
                           ├──> [cleanDataScreen: Limpieza de Datos]
                           ├──> [drawLOBFscreen: Modelo Matemático]
                           └──> [makePredictionsScreen: Predicciones e IA]
<h2><strong><em>🧮 Modelo Matemático</em></strong></h2>
Modelo de Regresión Lineal:

Código
Y_estimada = M * X + B
Y_estimada: Costo proyectado

X: Edad o BMI

M: Pendiente

B: Intersección

R: Confiabilidad del ajuste

<h2><strong><em>🛠️ Retos Técnicos y Soluciones</em></strong></h2>
1️⃣ Optimización del Datagrid
Renderizar 1,338 registros saturaba el lienzo

Se redujo la muestra a 300 registros

2️⃣ Compatibilidad Numérica
Problemas con separadores decimales

Solución: replace all text + conversión explícita

3️⃣ Depuración de Anomalías
Registros nulos afectaban métricas

Solución: algoritmo de Data Cleaning

<h2><strong><em>📌 Conclusiones</em></strong></h2>
✔️ Viabilidad Técnica
Conexión a la nube

Limpieza de datos

Cálculo estadístico

Integración de IA

✔️ Impacto Biométrico
Correlación positiva entre BMI, edad y incremento en primas

<h2><strong><em>💻 Tecnologías Utilizadas</em></strong></h2>
MIT App Inventor 2

Google Sheets

CSV Parsing

Bloques de lógica y matemáticas

UI/UX con Poppins-Regular.ttf y paleta pastel

<h2><strong><em>📁 Estructura del Proyecto</em></strong></h2>
Código
src/      → Archivo fuente (.aia)
assets/   → Tipografías, vectores e imágenes
docs/     → Capturas, diagramas y documentación
<h2><strong><em>👤 Autor</em></strong></h2>
María Fernanda Sánchez Alvarez  
Desarrollo e Implementación
