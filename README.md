Predicción de la sSFR de galaxias con Random Forest

Efecto de incorporar redshift y coeficientes Cα

Autores: R. Parra, B. Balmaceda, E. Luz, T. Luna y E. Donoso
Instituciones: Departamento de Geofísica, Astronomía y Física, Universidad Nacional de San Juan (UNSJ), Argentina; Consejo Nacional de Investigaciones Científicas y Técnicas (CONICET), Argentina.
Presentado en: 68.ª Reunión Anual de la Asociación Argentina de Astronomía (2026).

Descripción

La tasa de formación estelar específica (sSFR = SFR/M★) indica cuán activa es la formación estelar de una galaxia respecto de su masa estelar. Es un parámetro clave para estudiar su evolución y el apagado de la formación estelar. Estimar la sSFR a partir de información observacional accesible permite caracterizar poblaciones de galaxias.

En este proyecto empleamos modelos de machine learning para evaluar cuánta información sobre la sSFR aportan distintos conjuntos de variables fotométricas y espectroscópicas.

Objetivos

Evaluar cuánta información de la sSFR puede predecirse utilizando únicamente datos fotométricos.

Cuantificar la precisión adicional obtenida al incorporar redshift e información espectroscópica comprimida.

Comparar el desempeño de cuatro conjuntos de variables, desde un modelo base hasta el modelo de mayor complejidad.

Analizar cómo cambian la importancia y el orden de las variables entre modelos.

Datos

Se utilizó una muestra de galaxias basada en el catálogo MPA-JHU de SDSS, restringida al intervalo de redshift:

0.02 < z < 0.30

La variable objetivo es la sSFR. Además de la fotometría y el redshift, se utilizaron los coeficientes Cα del catálogo PCA de Wisconsin, que condensan la información espectroscópica de cada galaxia.

El archivo de trabajo empleado por el equipo es:

dr7MPA_WISE_WISC.fits

Los datos originales no se incluyen actualmente en el repositorio debido a su tamaño y mientras se verifica el procedimiento adecuado para su redistribución. La documentación de las fuentes puede consultarse en:

SDSS SkyServer DR16

Wisconsin PCA — SDSS

Kauffmann et al. (2003)

Conjuntos de variables

Modelo

Variables

M0

Fotometría

M1

Fotometría + redshift

M2

Fotometría + coeficientes Cα

M3

Fotometría + coeficientes Cα + redshift

Metodología

División de la muestra en conjuntos de entrenamiento y prueba.

Entrenamiento de modelos de regresión Random Forest.

Evaluación mediante métricas de regresión.

Análisis de importancia de variables.

<!-- Añadir aquí los hiperparámetros definitivos cuando el equipo cierre el análisis. -->

Resultados

Los resultados definitivos, las métricas de evaluación y las figuras utilizadas en el póster se incorporarán cuando finalice el análisis del equipo.

<!-- Añadir aquí la tabla definitiva con MAE, RMSE, R² y bias. -->

<!-- Añadir aquí las figuras definitivas mediante: ![Descripción](figures/nombre.png) -->

Discusión y conclusiones

Esta sección se completará a partir de los resultados definitivos presentados en el póster.

<!-- Añadir aquí la comparación M0–M3, la interpretación de las variables y las limitaciones. -->

Estructura prevista del repositorio

├── README.md
├── data/
│   └── README.md
├── notebooks/
├── src/
├── figures/
│   └── poster/
├── results/
└── requirements.txt

Contacto

Para consultas sobre el proyecto, puede utilizarse la sección Issues de este repositorio.procedencia y licencia de redistribución. Se documentan las variables empleadas y el procedimiento completo de preprocesamiento para garantizar la transparencia metodológica.
