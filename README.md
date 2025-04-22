# ⭕️ Redes Neuronales: Teoría y Práctica en Detección de Fraude Financiero con Autoencoders

---

## 📘 Introducción

La detección de fraude en transacciones financieras es un problema crucial en la era digital. A medida que los sistemas de pago electrónicos se expanden, también lo hacen las técnicas fraudulentas, poniendo en riesgo los activos de millones de personas y empresas.  
Este proyecto se enfoca en la implementación de técnicas de aprendizaje automático, con énfasis en redes neuronales profundas tipo **autoencoder**, para identificar transacciones sospechosas dentro de un conjunto realista de datos financieros.

---

## 🎯 Objetivos

### Objetivo General:
Implementar un sistema de detección de anomalías basado en autoencoders utilizando Keras para identificar patrones de fraude financiero en un dataset simulado de transacciones bancarias.

### Objetivos Específicos:
- 🔍 Analizar, explorar y preprocesar un conjunto de datos transaccionales con características numéricas y categóricas.  
- 🧠 Desarrollar un modelo autoencoder para identificar transacciones anómalas sin supervisión directa.  
- 📊 Evaluar el modelo utilizando métricas como precisión, recall y matriz de confusión.  
- 🎚️ Establecer umbrales óptimos de error de reconstrucción para maximizar la detección de fraudes reales.

---

## ⚠️ Núcleo Problemático

Las instituciones financieras enfrentan un constante desafío: detectar de manera precisa y en tiempo real transacciones fraudulentas entre millones de operaciones legítimas.  
La alta desproporción de datos (desequilibrio de clases) y la naturaleza cambiante de los patrones de fraude dificultan el uso de enfoques tradicionales.  
Se requieren técnicas capaces de aprender las características normales del sistema y detectar desviaciones sutiles que puedan representar riesgos.

---

## ❓ Pregunta Problemática

> ¿Es posible detectar transacciones financieras fraudulentas utilizando un autoencoder entrenado únicamente con datos normales, y cómo se puede ajustar su arquitectura y umbral de detección para maximizar el rendimiento del modelo?

---

## 🧪 Metodología

1. **Exploración del Dataset**  
   Comprensión del conjunto de datos, estructura, tipos de variables y distribución de clases.

2. **Preprocesamiento**  
   - Limpieza de datos: manejo de valores nulos, duplicados y outliers.  
   - Codificación de variables categóricas y normalización de datos numéricos.

3. **Construcción del Autoencoder**  
   - Arquitectura basada en capas simétricas de codificación y decodificación.  
   - Entrenamiento exclusivamente con transacciones normales.

4. **Evaluación del Modelo**  
   - Cálculo del error de reconstrucción sobre todo el dataset.  
   - Determinación de umbral de anomalía.  
   - Evaluación con métricas de clasificación.

5. **Visualización y análisis de resultados**  
   Análisis gráfico del error de reconstrucción y comparación con etiquetas reales de fraude.

6. **Conclusión y reflexión**  
   Interpretación de resultados, ventajas y limitaciones del uso de autoencoders para la detección de fraude financiero.

---

## 🧩 Dependencias

Este proyecto utiliza las siguientes librerías:

```toml
[tool.poetry.dependencies]
python = "3.10.15"
kagglehub = "^0.3.11"
pandas = "^2.2.3"
seaborn = "^0.13.2"
scipy = "^1.15.2"
imblearn = "^0.0"
numpy = "^2.2.5"
matplotlib = "^3.10.1"
scikit-learn = "^1.6.1"
imbalanced-learn = "^0.13.0"