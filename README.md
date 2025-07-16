# Titanic Machine Learning Challenge - Core Project

Este repositorio contiene la implementación completa del **Challenge Técnico Core** de Machine Learning para el dataset de Titanic de Kaggle.

## 🎯 Objetivo del Proyecto

Desarrollar un pipeline completo de machine learning para predecir la supervivencia de los pasajeros del Titanic, implementando y comparando múltiples modelos de clasificación.

## 📊 Dataset

- **Fuente**: [Titanic - Machine Learning from Disaster (Kaggle)](https://www.kaggle.com/c/titanic)
- **Datos de entrenamiento**: 891 muestras con 11 características
- **Datos de prueba**: 418 muestras para predicción
- **Variable objetivo**: Survived (0 = No sobrevivió, 1 = Sobrevivió)

## 🔧 Características del Proyecto

### 1. Análisis Exploratorio de Datos (EDA)
- Estadísticas descriptivas completas
- Análisis de valores faltantes y outliers
- Visualizaciones interactivas
- Identificación de patrones de supervivencia

### 2. Preprocesamiento de Datos
- **Feature Engineering**:
  - Extracción de títulos del nombre
  - Creación de variables de tamaño familiar
  - Grupos de edad y tarifa
  - Indicadores binarios (cabina, viaja solo)
- **Imputación inteligente** de valores faltantes
- **Codificación** de variables categóricas
- **Escalado** de características numéricas

### 3. Modelos Implementados

| Modelo | Tipo | Características |
|--------|------|----------------|
| 🔵 Regresión Logística | Lineal | Baseline, interpretable |
| 🟢 K-Nearest Neighbors | Instance-based | No paramétrico |
| 🟡 Árbol de Decisión | Tree-based | Interpretable, propenso a overfitting |
| 🟠 Random Forest | Ensemble | Robusto, maneja overfitting |
| 🔴 XGBoost | Gradient Boosting | Alto rendimiento, optimizado |
| 🟣 LightGBM | Gradient Boosting | Rápido, eficiente en memoria |

### 4. Evaluación y Benchmark
- **Validación cruzada** estratificada (5-fold)
- **Métricas múltiples**: Accuracy, precisión, recall
- **Análisis de overfitting**
- **Optimización de hiperparámetros** con GridSearchCV

## 🚀 Instalación y Uso

### Prerrequisitos
```bash
Python 3.8+
pip install -r requirements.txt
```

### Ejecutar el Notebook
```bash
jupyter notebook titanic_ml_challenge.ipynb
```

### Estructura de Archivos
```
SVM_CT_ML_Core/
├── titanic_ml_challenge.ipynb    # Notebook principal
├── train.csv                     # Datos de entrenamiento
├── test.csv                      # Datos de prueba
├── gender_submission.csv         # Ejemplo de submission
├── requirements.txt              # Dependencias
├── README.md                     # Este archivo
└── titanic_submission.csv        # Predicciones generadas
```

## 📈 Resultados Esperados

- **Accuracy objetivo**: > 80%
- **Mejor modelo**: Generalmente Random Forest o XGBoost optimizado
- **Características más importantes**:
  1. Género (Sex)
  2. Clase (Pclass)
  3. Tarifa (Fare)
  4. Edad (Age)
  5. Título extraído del nombre

## 🔬 Metodología

1. **Carga y exploración inicial** de datos
2. **Análisis exploratorio** con visualizaciones
3. **Preprocesamiento** y feature engineering
4. **Entrenamiento** de 6 modelos diferentes
5. **Evaluación** con validación cruzada
6. **Optimización** de hiperparámetros
7. **Generación** de predicciones finales

## 📊 Benchmark de Modelos

El notebook incluye una comparación comprehensiva de todos los modelos:
- Accuracy de entrenamiento vs validación
- Scores de validación cruzada con desviación estándar
- Análisis de overfitting
- Tiempo de entrenamiento
- Importancia de características

## 🎯 Submisión a Kaggle

El archivo `titanic_submission.csv` está listo para ser subido a Kaggle con el formato requerido:
```csv
PassengerId,Survived
892,0
893,1
...
```

## 🛠️ Tecnologías Utilizadas

- **Python 3.8+**
- **Pandas** - Manipulación de datos
- **NumPy** - Computación numérica
- **Matplotlib/Seaborn** - Visualización
- **Scikit-learn** - Machine Learning
- **XGBoost** - Gradient Boosting
- **LightGBM** - Gradient Boosting
- **Jupyter** - Notebook interactivo

## 📝 Versiones

- **v1.0.0** - Implementación inicial completa del challenge

## 🤝 Contribuciones

Este proyecto forma parte del Challenge Técnico Core de Machine Learning. 

## 📧 Contacto

Para preguntas o comentarios sobre este proyecto, por favor contacta al autor del challenge.

---

**¡Proyecto completado exitosamente! 🎉**

*Desarrollado como parte del Challenge Técnico de Machine Learning* 