# **Análisis de la eficiencia de los operadores de telecomunicaciones**
## Descripción general del proyecto

Este proyecto analiza el rendimiento de los operadores de telecomunicaciones con el fin de identificar a aquellos que presentan ineficiencias y detectar los cuellos de botella operativos que puedan afectar a la calidad del servicio al cliente.

Mediante el uso de Python, análisis estadístico y Tableau, el proyecto evalúa el rendimiento de los operadores a través de métricas clave, como las llamadas perdidas, los tiempos de espera y la actividad de llamadas salientes. El objetivo es facilitar la toma de decisiones operativas y mejorar la eficiencia del servicio.

## Problema empresarial

Una empresa de telecomunicaciones virtual quería identificar a los operadores cuyo rendimiento pudiera afectar negativamente a la experiencia del cliente.

Se debío determinar qué operadores podían clasificarse como ineficientes basándose en indicadores de rendimiento objetivos, en lugar de en una evaluación subjetiva.

## Dataset

El proyecto utiliza datos operativos del centro de atención telefónica que contienen información sobre llamadas entrantes y salientes, tiempos de espera, duración de las llamadas, actividad de los operadores e interacciones con los clientes.

## Variables principales

- Operator ID
- Client ID
- Call Direction (Incoming/Outgoing)
- Call Duration
- Waiting Time
- Missed Calls
- Internal Calls
- Call Date and Time

## Herramientas y tecnologías
- Python
- Pandas
- NumPy
- SciPy
- Tableau
- Análisis estadístico
- Análisis exploratorio de datos (EDA)

## Flujo de trabajo del proyecto
### 1. Carga de datos

Los conjuntos de datos se importaron a Python para su limpieza y análisis.

### 2. Limpieza de datos

Entre los pasos que se llevaron a cabo, se realizó lo siguiente:
- Tratamiento de valores perdidos.
- Eliminación de registros duplicados.
- Estandarización de los formatos de datos.
- Validación de la dirección de las llamadas y la información de los operadores.
- Preparación de los conjuntos de datos para el cálculo de métricas de rendimiento.

### 3. Análisis exploratorio de datos (EDA)

El análisis se centró en comprender:

- La distribución de las llamadas entrantes y salientes.
- Los patrones de duración de las llamadas.
- El comportamiento de las llamadas perdidas.
- Las distribuciones del tiempo de espera.
- La variabilidad de la carga de trabajo de los operadores.

###  4. Desarrollo de indicadores clave de rendimiento (KPI)

Se crearon indicadores de rendimiento personalizados para cada operador, entre los que se incluyen:

- Llamadas entrantes
- Llamadas entrantes perdidas
- Tasa de llamadas perdidas
- Tiempo medio de espera
- Llamadas salientes
- Duración media de las llamadas

### 5. Clasificación de los operadores

Los operadores se clasificaron como ineficientes basándose en un sistema de puntuación que tenía en cuenta:

- Altas tasas de llamadas perdidas.
- Tiempos de espera prolongados.
- Baja actividad en llamadas salientes.

Se asignó una puntuación de ineficiencia a cada operador para identificar a aquellos que requerían una mayor atención.

### 6. Validación estadística

Se realizaron pruebas de hipótesis U de Mann-Whitney para validar si los operadores ineficientes diferían significativamente de los eficientes en:

- Tasa de llamadas perdidas
- Tiempo medio de espera
- Volumen de llamadas salientes

## Dashboard
- Indicadores clave de rendimiento (KPI)
- Total de operadores
- Total de llamadas
- Tiempo medio de espera
- Índice de llamadas perdidas
- Operadores ineficientes identificados

## Visualizaciones
- Distribución de llamadas entrantes frente a salientes
- Clasificación del rendimiento de los operadores
- Análisis de llamadas perdidas
- Distribución del tiempo de espera
- Dashboard de operadores ineficientes

## Conclusiones principales
### Rendimiento operativo
- Los operadores ineficientes presentaban sistemáticamente tasas de llamadas perdidas más elevadas.
- Los tiempos de espera prolongados estaban estrechamente relacionados con un bajo rendimiento de los operadores.

### Análisis estadístico
- Los operadores clasificados como ineficientes presentaban tasas de llamadas perdidas significativamente más elevadas.
- Los operadores ineficientes registraban tiempos de espera significativamente más largos.
- La actividad de llamadas salientes era significativamente menor entre los operadores ineficientes.

### Repercusión en el negocio
- Se ha identificado un subconjunto de operadores cuyo rendimiento es sistemáticamente inferior al esperado.
- El dashboard permite identificar rápidamente los cuellos de botella operativos y las oportunidades de mejora de los procesos.

## Cómo ejecutar este proyecto
### 1. Clona el repositorio
git clone <repository-url>
cd telecom-operator-analysis
### 2. Instala las dependencias
pip install pandas numpy scipy matplotlib tableau-api-lib
### 3. Abre el cuaderno

Ejecuta:

notebooks/telecom_operator_analysis.ipynb
### 4. Ejecuta el análisis

Ejecuta el notebook de forma secuencial para:

- Limpiar los datos.
- Calcular las métricas de rendimiento de los operadores.
- Clasificar a los operadores ineficientes.
- Realizar pruebas estadísticas.
- Generar visualizaciones y conclusiones.
### 5. Revisa el dashboard

Abre el dashboard de Tableau para explorar el rendimiento de los operadores de forma interactiva.

