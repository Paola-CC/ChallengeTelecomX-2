# 📡 Telecom X: Predicción de Churn (Fase 2)

Este proyecto desarrolla un pipeline de Machine Learning para predecir la cancelación de servicios (churn) en una empresa de telecomunicaciones. El objetivo es identificar clientes en riesgo y proporcionar insights estratégicos para mejorar la retención.

## 🚀 Descripción del Proyecto

En esta segunda fase del desafío, nos enfocamos en la preparación avanzada de datos, el balanceo de clases y la implementación de modelos predictivos de clasificación. Se comparó el rendimiento de modelos basados en distancia y modelos basados en árboles para determinar la mejor solución.

## 🧠 Objetivos

* **Preprocesamiento:** Limpieza, codificación (One-Hot Encoding) y normalización de datos.
* **Balanceo de Datos:** Aplicación de técnica SMOTE para corregir el desequilibrio de clases.
* **Modelado:** Entrenamiento de modelos de **Regresión Logística**, **KNN** y **Random Forest**.
* **Evaluación:** Análisis mediante matrices de confusión, Accuracy, Precision, Recall y F1-Score.
* **Interpretación:** Identificación de las variables con mayor impacto en la evasión de clientes.

## 🛠️ Herramientas Utilizadas

* **Google Colab:** Entorno de desarrollo.
* **Pandas & NumPy:** Manipulación de datos.
* **Scikit-Learn:** Algoritmos de Machine Learning y métricas.
* **Imbalanced-learn (SMOTE):** Balanceo de clases.
* **Seaborn & Matplotlib:** Visualización de datos y matrices de correlación.

## 📊 Hallazgos y Resultados

### 1. ¿Quiénes son los clientes con mayor riesgo de evasión?
* **Contratos cortos:** Personas con planes de pago mes a mes.
* **Nuevos usuarios:** Clientes con menos de 6 a 12 meses de antigüedad.
* **Usuarios de Fibra con facturas altas:** Clientes con cargos mensuales elevados que no cuentan con servicios adicionales de apoyo.

### 2. Variables de Mayor Influecia
1.  **Tipo de Contrato:** El factor más determinante.
2.  **Cargos Mensuales:** El impacto del precio en la decisión de salida.
3.  **Falta de Soporte Técnico:** Correlación directa entre la ausencia de soporte y la fuga.
4.  **Método de Pago:** Los pagos manuales presentan mayor inestabilidad.

## 📈 Perfil de Fidelización Estratégica

| Característica | Detalle Estratégico |
| :--- | :--- |
| **Vinculación Contractual** | Clientes con contratos de **uno o dos años**. |
| **Automatización** | Usuarios con **pagos automáticos** (tarjeta o transferencia). |
| **Ecosistema de Servicios** | Clientes con **múltiples servicios** (Internet + Seguridad + Soporte). |
| **Perfil Digital Acompañado** | Usuarios con **factura electrónica** que usan canales digitales de soporte. |

## 📁 Estructura del Repositorio

* `Desafio_Telecom_X_Parte_2.ipynb`: Notebook principal con todo el análisis y código.
* `datos_tratados.csv`: Dataset procesado utilizado para el entrenamiento.
* `README.md`: Documentación del proyecto.
