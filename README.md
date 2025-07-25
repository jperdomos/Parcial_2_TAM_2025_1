# 📘 Parcial 2 - Teoría de Aprendizaje de Máquina (TAM) 2025-1

**Universidad Nacional de Colombia - sede Manizales**  
**Departamento de Ingeniería Eléctrica, Electrónica y Computación**  
**Profesor:** Andrés Marino Álvarez Meza, Ph.D.  
**Estudiantes:**  
- Juan Camilo Perdomo  
- Jholman Dasney Meza
- Campos Herney Campos Tulcan

---

## 📄 Descripción General

Este repositorio contiene la solución completa al **Parcial 2 de la asignatura Teoría de Aprendizaje de Máquina (2025-1)**. Se resuelven los cinco puntos solicitados, integrando teoría, simulación, visualización interactiva y un video explicativo.

---

## 📁 Estructura del Proyecto

```
Parcial_2_TAM_2025_1-main/
│
├── 📘 Parcial TAM.pdf                 # Punto (a): teoría y formulaciones
├── 📓 Parcial2_TAM_2025_1.ipynb       # Punto (b) y (c): proyección y clasificación
├── 📓 DashboardParcial2TAM.ipynb      # Punto (d): dashboard interactivo
├── 📄 README.md                       # Este archivo explicativo
```

---

## ✅ Punto (a) – Modelos y Problemas de Optimización

En el archivo **Parcial TAM.pdf** se presentan los modelos teóricos de:

- **Reducción de dimensión:** PCA, UMAP  
- **Clasificadores clásicos:** GaussianNB, SGDClassifier, LogisticRegression, LDA, KNN, SVC, RandomForest, GaussianProcessClassifier  
- **Clasificadores profundos (deep learning)**

Cada modelo incluye:  
🔹 Formulación matemática  
🔹 Problema de optimización asociado  
🔹 Método de entrenamiento o solución

---

## 📉 Punto (b) – Proyección del dataset USPS

- Se usó el dataset de dígitos escritos a mano **USPS**
- Se aplicaron los métodos:
  - **PCA** (`sklearn.decomposition.PCA`)
  - **UMAP** (`umap-learn`)
- Se graficó la proyección 2D con colores por clase (dígitos 0–9)
- Se superpusieron imágenes reales con `OffsetImage`
- Se analizó el efecto del parámetro `n_neighbors` en UMAP sobre la estructura latente

---

## 🧠 Punto (c) – Clasificadores y Evaluación

Modelos utilizados:
- **Regresión Logística**
- **Random Forest**
- **Red Neuronal Convolucional (CNN)** en PyTorch

Evaluación con:
- Matriz de confusión
- Curvas ROC multiclase (`OneVsRestClassifier`)
- Accuracy, F1-score, Precision y Recall
- Optimización de hiperparámetros con `Optuna`
- Validación cruzada con `StratifiedKFold`

---

## 📊 Punto (d) – Dashboard Interactivo

El notebook `DashboardParcial2TAM.ipynb` contiene:
- Visualización de proyecciones (PCA/UMAP)
- Comparación de clasificadores
- Métricas interactivas
- Predicción de nuevas muestras

> Puede adaptarse fácilmente a una app `Streamlit` con `app.py`.

---

## 🎥 Punto (e) – Video Explicativo

🔗 **Enlace al video de YouTube:**  
[https://youtu.be/cnuHIShaGeI](https://youtu.be/cnuHIShaGeI) 

Contenido del video (duración: 3–5 minutos):
1. Recorrido por el dashboard
2. Explicación de los puntos (a)-(c)
3. Introducción a Transformers:
   - Capas de atención
   - Arquitectura general
   - Aplicación en clasificación multiclase (como USPS)

---

## 🧪 Requisitos

Instala los paquetes con:

```bash
pip install -r requirements.txt
```

Librerías principales:
- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`, `seaborn`
- `umap-learn`
- `torch`, `torchvision`
- `optuna`
- `ipywidgets` o `streamlit` (opcional para dashboard)

---

