# Proyecto Telecom X - Análisis de Evasión de Clientes (Churn)

## Descripción del Proyecto
Telecom X enfrenta una alta tasa de cancelación de servicios por parte de sus clientes (evasión o churn). Este proyecto tiene como objetivo analizar los datos de clientes para identificar patrones y factores que influyen en la decisión de abandonar el servicio, ayudando a la empresa a diseñar estrategias para mejorar la retención.

## Objetivo
Realizar un análisis exploratorio de datos (EDA) para comprender las características de los clientes que se dan de baja y detectar variables relevantes que expliquen la evasión.

## Estructura del Proyecto
- **TelecomX_Data.json**: Archivo con los datos de clientes.
- **TelecomX_LATAM.ipynb**: Notebook con todo el análisis, desde la carga y limpieza de datos, hasta las visualizaciones y conclusiones.
- **TelecomX_diccionario.md**: Diccionario con la descripción de cada variable del dataset.

## Proceso Realizado

### 1. Extracción y Transformación de Datos
- Se cargaron los datos desde un archivo JSON.
- Se normalizó la estructura anidada y se exploraron columnas y tipos de datos.
- Se limpiaron valores nulos, especialmente en la variable objetivo `Evasion` y en `Cargo_Total`.
- Se reemplazaron valores como "No internet service" por "No" para evitar inconsistencias.
- Se creó la columna `Cuentas_Diarias` calculando el cargo mensual dividido en días.
- Se estandarizaron valores binarios ("Yes"/"No") a 1 y 0.
- Se tradujeron y renombraron las columnas para mayor claridad.

### 2. Análisis Exploratorio de Datos (EDA)
- Se calcularon estadísticas descriptivas para variables numéricas como gasto mensual, total y tiempo de contrato.
- Se visualizó la distribución de la evasión, encontrando que aproximadamente el 26.6% de los clientes se dieron de baja.
- Se analizó la evasión según variables categóricas como género, tipo de contrato y método de pago, identificando diferencias relevantes.
- Se estudiaron variables numéricas en función de la evasión mediante gráficos boxplot, encontrando que clientes con contratos más cortos y menor gasto tienden a evadir más.

### 3. Conclusiones e Insights
- La evasión afecta a más de una cuarta parte de los clientes.
- Clientes con contratos mensuales y ciertos métodos de pago presentan mayor riesgo de evasión.
- El gasto total y la duración del contrato están asociados a la retención.

### 4. Recomendaciones
- Incentivar contratos a largo plazo ofreciendo beneficios adicionales.
- Promover métodos de pago automáticos para facilitar la fidelización.
- Dirigir campañas especiales a clientes nuevos o con bajo gasto para mejorar su retención.

## Cómo ejecutar el notebook
1. Clonar o descargar el repositorio.
2. Abrir el archivo `TelecomX_LATAM.ipynb` en Google Colab o Jupyter Notebook.
3. Ejecutar las celdas paso a paso para reproducir el análisis.
4. Revisar las visualizaciones y conclusiones para comprensión completa.

