[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mariantocostanzo/Challange_Telecom_X_parte2/blob/main/telecom_X_parte%202.ipynb)

# 📊 Proyecto Telecom X - Parte 2: Predicción de Cancelación de Clientes (Churn)

Este proyecto tiene como objetivo principal **predecir la cancelación de clientes (churn)** en una empresa de telecomunicaciones, utilizando modelos de machine learning basados en variables relevantes del comportamiento del cliente.

---

## 🗂️ Estructura del Proyecto

- `Telecom_X_Parte2.ipynb`: Cuaderno principal del análisis.
- `datos_tratados.csv`: Archivo con los datos preprocesados.
- `visualizaciones/`: Carpeta que contiene los gráficos generados (matrices de confusión, comparación de modelos, etc.).
- `README.md`: Este archivo de documentación.

---

## 🧹 Preparación de los Datos

### 🔠 Clasificación de Variables

- **Variables Categóricas**: `InternetService`, `Contract`, `PaymentMethod`, entre otras.
- **Variables Numéricas**: `tenure`, `MonthlyCharges`, `TotalCharges`, etc.

### ⚙️ Transformaciones Aplicadas

- **Codificación**: Se utilizaron técnicas como OneHotEncoding para variables categóricas.
- **Normalización**: Aplicada para modelos sensibles a la escala como la Regresión Logística.
- **Manejo de Nulos**: Se eliminaron o imputaron registros con valores nulos.

### 🧪 División de Datos

- **Conjunto de entrenamiento**: 80%
- **Conjunto de prueba**: 20%

---

## 🤖 Modelos Utilizados

### 1. Regresión Logística

- ✔️ Requiere normalización.
- ✔️ Útil para interpretación de coeficientes.
- ❌ Sensible a valores atípicos.

### 2. Random Forest

- ✔️ No requiere normalización.
- ✔️ Robusto ante datos ruidosos.
- ✔️ Permite calcular importancia de variables.

---

## 📊 Visualizaciones

### Matriz de Confusión - Regresión Logística

![Matriz de Confusión - Regresión Logística](visualizaciones/matriz-regresion.png)

### Matriz de Confusión - Random Forest

![Matriz de Confusión - Random Forest](visualizaciones/matriz-ramdom.png)

### Comparación de Modelos (Accuracy)

![Comparación de Modelos](visualizaciones/comparacion_de_modelos.png)

---

## 💡 Insights del Análisis Exploratorio (EDA)

- Los clientes con contratos mensuales tienden a cancelar más.
- La ausencia de servicio de Internet se asocia a menor churn.
- Altos cargos mensuales correlacionan con mayor probabilidad de cancelación.

---

📬 Consultas o sugerencias: ¡bienvenidas!
