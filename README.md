# Challenge TelecomX LATAM

## Descripción

Este proyecto aborda el análisis de evasión de clientes (Churn) para una empresa de telecomunicaciones ficticia llamada TelecomX. El objetivo es identificar los factores que influyen en la cancelación de servicios por parte de los clientes y proponer estrategias para reducir la evasión.

## Proceso realizado

### 1. Extracción de Datos
- Se importaron los datos desde un archivo JSON.
- Se normalizaron las estructuras anidadas para obtener un DataFrame plano y fácil de analizar.

### 2. Limpieza y Transformación
- Se seleccionaron y unieron tablas relevantes: información general, datos de cliente, teléfono, internet y cuenta.
- Se transformaron variables categóricas ("Yes"/"No") a valores numéricos (1/0).
- Se reemplazaron valores como "No phone service" y "No internet service" por 0 para facilitar el análisis.
- Se eliminaron filas con valores nulos en variables clave como "Charges.Total".
- Se eliminaron columnas irrelevantes para el análisis.
- Se creó la variable `Cuentas_Diarias` para analizar el gasto diario promedio de los clientes.

### 3. Análisis Exploratorio de Datos
- Se calcularon estadísticas descriptivas (media, mediana, desviación estándar, etc.) para comprender la distribución de las variables.
- Se generó una matriz de correlación para identificar relaciones entre variables.
- Se analizaron las distribuciones de variables clave como "Charges.Total" y "Contract.Months" según la evasión de clientes, utilizando histogramas y boxplots.

### 4. Visualización
- Se utilizaron gráficos de distribución y boxplots para comparar el comportamiento de clientes que cancelaron y los que no.
- Se incluyó un heatmap para visualizar la correlación entre variables.

### 5. Conclusiones y Recomendaciones
- Se identificaron patrones y variables asociadas a la evasión.
- Se propusieron recomendaciones estratégicas para reducir la evasión, como segmentación de clientes, mejora de servicios clave y uso de modelos predictivos.

## Cómo reproducir el análisis

1. Clona este repositorio.
2. Asegúrate de tener Python 3 y las siguientes librerías instaladas: `pandas`, `numpy`, `matplotlib`, `seaborn`, `json`.
3. Ejecuta el notebook `TelecomX_LATAM.ipynb` en Jupyter Notebook o Visual Studio Code.
4. Sigue el flujo del notebook para ver cada paso del análisis y las visualizaciones generadas.

## Estructura del repositorio

- `TelecomX_Data.json`: Archivo de datos de entrada.
- `TelecomX_LATAM.ipynb`: Notebook principal con todo el análisis.
- `README.md`: Este archivo.