# Implementación y comparación de algoritmos de clasificación

**Estudiante:** Jheyson Jair Morales Serrato
**Materia:** Introducción a Machine Learning (604027), Universidad de Cundinamarca
**Actividad:** Semana 8, algoritmos de clasificación

## Objetivo
Aplicar cinco algoritmos de clasificación (Decision Tree, Random Forest, SVM, K-NN y Naive Bayes) sobre un mismo caso, comparar sus resultados y seleccionar el más adecuado.

## Datos
Breast Cancer Wisconsin (Diagnostic), incluido en scikit-learn (`load_breast_cancer`). 569 muestras, 30 variables numéricas. Variable objetivo: 1 = maligno, 0 = benigno. Uso exclusivamente académico; no es una herramienta clínica.

## Método
- División 80/20 con `random_state=42` y `stratify=y`, la misma para los cinco modelos.
- Escalamiento (`StandardScaler`) solo en SVM y K-NN.
- Métricas: Accuracy, Precision, Recall, F1 y matriz de confusión.

## Resultado
Random Forest y SVM obtuvieron el mejor desempeño (recall 0,929; precision 1,000). Se seleccionó Random Forest porque no requiere escalamiento y permite identificar qué variables pesan más en la decisión.

## Cómo ejecutar
1. Abrir `ML_S8_Clasificacion_MoralesJheyson.ipynb` en Google Colab (botón "Open in Colab").
2. Entorno de ejecución > Ejecutar todo. No se requiere subir archivos: la base se carga desde scikit-learn.

## Librerías
pandas, scikit-learn
