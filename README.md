# Predicción de Tendencia de Bitcoin con Machine Learning
**Proyecto Final - Data Science II - Coderhouse**

### 1. Abstracto
Este proyecto representa la evolución de un análisis financiero descriptivo previo hacia la implementación de un sistema predictivo robusto basado en **Machine Learning**. Utilizando datos históricos de precios de activos (Bitcoin y Apple), el estudio modela la situación como un problema de **Clasificación Binaria** para anticipar si el precio de cierre de Bitcoin (BTC) en la siguiente jornada será superior o inferior al actual. Para maximizar la capacidad de aprendizaje de los algoritmos, el dataset original fue purificado y enriquecido con indicadores técnicos de momentum (Retornos Diarios), permitiendo pasar de la mera observación histórica a la generación de ventajas estadísticas accionables.

### 2. Motivación
La volatilidad extrema que caracteriza al mercado de las criptomonedas hace que las decisiones de inversión basadas puramente en la intuición o en gráficos estáticos conlleven un riesgo muy elevado. La motivación principal de este trabajo es dotar al proceso de toma de decisiones de un sustento estadístico riguroso. Al entrenar modelos de ensamble capaces de evaluar múltiples variables en simultáneo, buscamos transformar datos crudos en un sistema de alerta temprana que ayude a mitigar el riesgo.

### 3. Audiencia
Este análisis y las predicciones del modelo están diseñados para beneficiar a:
* **Inversores y Traders Particulares** que requieren herramientas técnicas para validar sus tesis de inversión antes de arriesgar capital.
* **Analistas de Riesgo Financiero** que buscan incorporar modelos cuantitativos para medir la probabilidad de movimientos adversos en carteras digitales.
* **Roles Ejecutivos y Gestores de Cartera** que necesitan una visión respaldada por datos sobre el comportamiento predictivo de los activos.

### Insights y Conclusiones Finales

Tras la implementación, optimización (mediante GridSearchCV) y evaluación de los modelos de Machine Learning, consolidamos los siguientes hallazgos:

1. **Poder Predictivo Confirmado:** El modelo ganador, **Random Forest**, superó el umbral del azar (50%), alcanzando una **precisión del 71%** para predecir la dirección del precio de Bitcoin al día siguiente. 
2. **Superioridad del Random Forest frente a XGBoost:** Aunque XGBoost suele ser el estándar, en este dataset particular y tras la validación cruzada, Random Forest demostró ser más robusto y menos propenso al sobreajuste (*overfitting*).
3. **Interpretabilidad (SHAP):** La ingeniería de atributos fue clave. Según el análisis de interpretabilidad con la librería SHAP, las variables creadas como los retornos recientes tienen un impacto directo y cuantificable en las decisiones del árbol de decisión.
4. **Impacto en el Negocio:** Un 71% de acierto permite complementar el análisis humano con una "segunda opinión" puramente estadística, ofreciendo una ventaja competitiva real en el mercado financiero.

---
**Tecnologías utilizadas:** `Python` `Pandas` `Scikit-Learn` `XGBoost` `SHAP` `Matplotlib` `Seaborn`
