📊 Insurance Cost Predictions App
Aplicación móvil desarrollada en MIT App Inventor enfocada en el análisis, depuración de datos y predicción de costos de primas de seguro médico utilizando modelos de regresión lineal e integración con Inteligencia Artificial.

📑 Tabla de Contenidos
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

🚀 Descripción General
Esta herramienta analítica permite examinar cómo influyen variables biométricas y demográficas (como la edad y el índice de masa corporal) en el costo de una póliza de seguro médico.
La aplicación:

Consume datos en tiempo real desde Google Sheets.

Ejecuta algoritmos de limpieza de datos atípicos.

Traza la línea de mejor ajuste (Line of Best Fit).

Genera proyecciones financieras apoyadas por un asistente de IA.

✨ Características Principales
Autenticación y Control de Acceso (Screen0): Validación de credenciales.

Navegación Modular (Screen1): Panel centralizado para acceder a cada etapa analítica.

Depuración de Datos (cleanDataScreen): Algoritmo de filtrado e identificación de anomalías.

Modelado Matemático (drawLOBFscreen): Cálculo dinámico de pendiente (M), intersección (B) y coeficiente de correlación (R).

Predicciones e IA (makePredictionsScreen): Evaluación de escenarios en tiempo real con soporte de chatbot.

📂 Dataset
Nombre: Medical Cost Personal Datasets (Miri Choi)

Fuente: Kaggle Dataset

Integración: Google Sheets (sincronización en la nube).

Muestra Seleccionada: 300 registros representativos para optimizar rendimiento.

Variables Clave
age: Edad del usuario

bmi: Índice de Masa Corporal

charges: Prima del seguro

smoker: Factor de riesgo por tabaquismo

🛠️ Arquitectura de la Aplicación
text
[Screen0: Login] ──> [Screen1: Menú Principal]
                           ├──> [cleanDataScreen: Limpieza de Datos]
                           ├──> [drawLOBFscreen: Modelo Matemático]
                           └──> [makePredictionsScreen: Predicciones e IA]
🧮 Modelo Matemático
Se utiliza un modelo de Regresión Lineal:

Código
Y_estimada = M * X + B
Y_estimada: Costo proyectado del seguro
X: Variable predictora (Edad o BMI)
M: Pendiente (incremento por unidad)
B: Intersección en Y (valor base)
R: Coeficiente de correlación (confiabilidad del ajuste)

🛠️ Retos Técnicos y Soluciones
1. Optimización del Datagrid y Visualización Gráfica
Desafío: Renderizar 1,338 registros generaba saturación visual y latencia.
Solución: Acotar la muestra a 300 registros para trazados limpios y ejecución fluida.

2. Compatibilidad Numérica
Desafío: Incompatibilidad entre separadores decimales (punto/coma).
Solución: Normalización con replace all text y conversión explícita a número.

3. Depuración de Anomalías
Desafío: Registros nulos o atípicos distorsionaban las métricas del modelo.
Solución: Algoritmo de filtrado (Data Cleaning) previo al cálculo de la regresión.

📌 Conclusiones
Viabilidad Técnica
MIT App Inventor demostró capacidad para:

Conectarse a servicios en la nube

Depurar datos

Calcular modelos matemáticos

Integrar componentes de IA

Impacto Biométrico
Se confirma una correlación positiva entre:

BMI

Edad

Incremento en el costo de las primas

💻 Tecnologías Utilizadas
Desarrollo Móvil: MIT App Inventor 2

Base de Datos / Cloud: Google Sheets

Lógica: Bloques de App Inventor (listas, condicionales, operaciones matemáticas)

UI/UX: Tipografía Poppins-Regular.ttf y paleta pastel

📁 Estructura del Proyecto
Código
src/      → Archivo fuente (.aia)
assets/   → Tipografías, vectores e imágenes
docs/     → Capturas, diagramas y documentación
👤 Autor
María Fernanda Sánchez Alvarez  
Desarrollo e Implementación
