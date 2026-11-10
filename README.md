# Análisis de fraude bancario con Python y Power BI

**Autora:** Lucía Florencia Coppa  
**Curso:** Curso de Herramientas básicas para el Análisis de Datos – UTN  
**Proyecto:** Trabajo Final Integrador  
**Dataset:** PaySim – Transacciones financieras simuladas

## Motivación y elección del dataset

Elegí trabajar con un dataset de fraude bancario porque actualmente me desempeño en el rubro bancario y me interesa comprender cómo el análisis de datos puede contribuir a identificar riesgos y mejorar los procesos de prevención.

Desde mi experiencia laboral, considero importante comprender no solo las operaciones financieras, sino también los patrones y comportamientos que pueden representar situaciones de riesgo.

Este proyecto me permitió relacionar mi experiencia profesional con los conocimientos adquiridos durante el curso, aplicando herramientas de análisis y visualización para transformar datos en información útil para la toma de decisiones.

## Objetivo del proyecto

El objetivo de este trabajo es analizar transacciones financieras para identificar patrones asociados al fraude bancario y evaluar indicadores que puedan contribuir a la detección de operaciones sospechosas.

La pregunta principal es: **¿Qué características presentan las operaciones fraudulentas y qué indicadores permiten identificar situaciones de mayor riesgo?**

### Preguntas de análisis

Para orientar el análisis exploratorio, se plantearon las siguientes preguntas:

1. ¿Qué tipos de transacciones presentan mayor cantidad de fraudes?
2. ¿Cuál es la tasa de fraude por tipo de operación?
3. ¿Cuál es el importe promedio de las operaciones fraudulentas frente a las legítimas?
4. ¿En qué días de la simulación se registra mayor cantidad de fraudes?
5. ¿Qué porcentaje de las operaciones fraudulentas fue identificado por el sistema de alertas?

## Dataset utilizado

Se utilizó PaySim, un conjunto de datos de transacciones financieras simuladas, disponible en [Kaggle](https://www.kaggle.com/datasets/ealaxi/paysim1).

El dataset contiene 6.362.620 operaciones y variables como tipo de transacción, importe, saldos de origen y destino, período de simulación e indicadores de fraude.

Debido al tamaño del archivo original, se proporciona el enlace a la fuente en lugar de incorporarlo directamente al repositorio.

## Metodología

El análisis se desarrolló utilizando **Python en Google Colab**, con Pandas para la exploración y limpieza de datos, y Matplotlib y Seaborn para las visualizaciones.

Se verificaron tipos de datos, valores nulos, registros duplicados y valores atípicos. Posteriormente, se analizaron los fraudes según tipo de operación, importe y período de simulación.

Finalmente, se construyó un dashboard en **Power BI**, incorporando indicadores principales, gráficos comparativos y un filtro interactivo por tipo de operación.

## Principales resultados

- Se identificaron **8.213 operaciones fraudulentas**, equivalentes al **0,13 %** del total.
- Los fraudes se concentraron en CASH_OUT (4.116 casos) y TRANSFER (4.097 casos).
- TRANSFER presentó una tasa de fraude del **0,77 %**, superior a CASH_OUT (**0,18 %**).
- El indicador `isFlaggedFraud` detectó solamente 16 de los 8.213 fraudes, lo que evidencia una cobertura muy limitada en este conjunto de datos.

## Conclusión

Los resultados muestran que la cantidad absoluta de fraudes no es suficiente para evaluar el riesgo. Es necesario considerar también la proporción de operaciones fraudulentas y complementar las alertas con otros indicadores.

Los hallazgos corresponden a datos simulados y no deben interpretarse como resultados de entidades bancarias reales.

## Archivos del proyecto

- [Notebook del análisis en Python](notebooks/Analisis_Fraude_Bancario_Entrega%20%281%29.ipynb)
- [Captura del dashboard de Power BI](Dashboard_Fraude_Bancario.png)
- [Fuente original del dataset PaySim](https://www.kaggle.com/datasets/ealaxi/paysim1)

## Herramientas y fuentes

Python, Google Colab, Pandas, Matplotlib, Seaborn, Power BI y GitHub.

Fuente de datos: PaySim, dataset de transacciones financieras simuladas, publicado en Kaggle.
