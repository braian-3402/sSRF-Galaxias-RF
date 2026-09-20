# Predicción de la sSFR de galaxias con Random Forest

Este proyecto estudia la predicción de la tasa de formación estelar específica de galaxias mediante modelos de Random Forest y evalúa el efecto de incorporar redshift e información espectroscópica comprimida.

## Descripción

La tasa de formación estelar específica (`sSFR = SFR/M★`) indica cuán activa es la formación estelar de una galaxia respecto de su masa estelar. Es un parámetro clave para estudiar la evolución de las galaxias y el apagado de su formación estelar.

Los modelos de Machine Learning permiten evaluar cuánta información sobre la sSFR aportan distintos conjuntos de variables observacionales.

## Objetivos

- Estimar la sSFR utilizando únicamente datos fotométricos.
- Evaluar la precisión adicional obtenida al incorporar redshift.
- Evaluar el aporte de información espectroscópica comprimida.
- Comparar el desempeño de cuatro conjuntos de variables.
- Analizar cómo cambia la importancia de las variables entre los modelos.

## Datos

Se utilizó una muestra de galaxias basada en el catálogo MPA-JHU de SDSS dentro del rango:

`0.02 < z < 0.30`

La variable objetivo es la sSFR. Además de la fotometría y el redshift, se emplearon los coeficientes Cα del catálogo PCA de Wisconsin, que resumen de forma comprimida la información espectroscópica de cada galaxia.

El archivo utilizado durante el análisis fue:

`dr7MPA_WISE_WISC.fits`

Los datos originales no se incluyen en este repositorio debido a su tamaño y a que pertenecen a fuentes externas.

## Modelos

Se analizaron cuatro combinaciones de variables:

- **M0:** Fotometría.
- **M1:** Fotometría + redshift.
- **M2:** Fotometría + coeficientes Cα.
- **M3:** Fotometría + coeficientes Cα + redshift.

## Metodología

El procedimiento general consistió en:

1. Preparar y seleccionar la muestra de galaxias.
2. Dividir los datos en conjuntos de entrenamiento y prueba.
3. Entrenar los modelos de regresión.
4. Evaluar su desempeño mediante métricas de regresión.
5. Analizar la importancia de las variables.

## Fuentes

- [SDSS SkyServer DR16](https://skyserver.sdss.org/dr16/en/home.aspx)
- [Wisconsin PCA - SDSS](https://www.sdss.org/dr16/spectro/galaxy_wisconsin/)
- [Kauffmann et al. (2003)](https://ui.adsabs.harvard.edu/abs/2003MNRAS.341...33K/abstract)

## Autores

- R. Parra
- B. Balmaceda
- E. Luz
- T. Luna
- E. Donoso

## Instituciones

- Departamento de Geofísica, Astronomía y Física, Universidad Nacional de San Juan, Argentina.
- Consejo Nacional de Investigaciones Científicas y Técnicas, Argentina.

Trabajo presentado en la 68.ª Reunión Anual de la Asociación Argentina de Astronomía, 2026.
