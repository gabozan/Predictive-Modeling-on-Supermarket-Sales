# Predictive-Modeling-on-Supermarket-Sales

## 🧠 Objetivo: Predicción de Sucursal para la Optimización de Stock

## 📌 Descripción General
Este proyecto tiene como objetivo desarrollar y evaluar modelos de clasificación que permitan predecir la sucursal (`Branch`) en la que se realiza cada venta, utilizando técnicas de aprendizaje supervisado. El objetivo final es facilitar una mejor planificación del stock en función de la demanda localizada.

Dado que la empresa está en expansión y abrirá nuevas sucursales próximamente, el modelo debe ser escalable y tener buena capacidad de generalización.

## 📊 Dataset
El conjunto de datos contiene 1.000 transacciones registradas en 3 sucursales diferentes, con 17 atributos por registro. Algunas columnas del dataset:

- `Invoice ID`, `Branch`, `City`, `Customer type`, `Gender`
- `Product line`, `Unit price`, `Quantity`
- `Date`, `Time`, `Payment`
- `Gross income`, `Total`, `Rating`

## 🔍 Enfoque del Proyecto
1. Preprocesamiento
- Detección y visualización de valores nulos (`missingno`)
- Conversión de variables categóricas con `LabelEncoder` y `OneHotEncoder`
- Normalización de atributos numéricos con `StandardScaler`

2. Modelado
- Se entrenaron y evaluaron múltiples modelos de clasificación, incluyendo:
- `Logistic Regression`
- `Support Vector Machines (SVC)`
- `K-Nearest Neighbors (KNN)`
- `Decision Trees`
- `Random Forest`
- `AdaBoost`

3. Evaluación
- División de datos en train/test con `train_test_split`
- Validación cruzada con `StratifiedKFold` y `cross_val_score`
- Evaluación con métricas: `accuracy`, `ROC AUC`, `confusion matrix`
