# ML Classification Baseline: Titanic Dataset

Primer proyecto de clasificación binaria implementando un *pipeline* de preprocesado estructurado y evaluación de un modelo base.

## Flujo de Procesamiento de Datos
- **Depuración y Reducción:** Eliminación de ruido y variables de alta cardinalidad sin valor predictivo directo (`PassengerId`, `Name`, `Ticket`).
- **Normalización Diferencial:** Aplicación aislada de `MinMaxScaler` para variables con límites definidos (edad) y `StandardScaler` para asentar el descenso de gradiente.
- **Validación Arquitectónica:** Separación estricta de conjuntos de datos (Train/Validation/Test) para prevenir la filtración de datos (*data leakage*) durante el entrenamiento.

## Rendimiento del Modelo Base
- **Algoritmo:** Regresión Logística.
- **Precisión (Validation Set):** 76.22%
