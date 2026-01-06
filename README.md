# 📊 Análisis de Evasión de Clientes (Churn) - Telecom X

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Library-Pandas-150458)
![Seaborn](https://img.shields.io/badge/Library-Seaborn-green)
![Status](https://img.shields.io/badge/Status-Finalizado-success)

## 📖 Descripción del Proyecto

Este proyecto consiste en un análisis de datos exhaustivo para la empresa ficticia **Telecom X**, con el objetivo de identificar las causas raíz de la fuga de clientes (*Churn*) y proponer estrategias de retención basadas en datos.

El análisis abarca desde la limpieza de datos complejos (JSON anidados) hasta la modelación estadística mediante matrices de correlación y visualización avanzada, permitiendo detectar patrones de comportamiento en más de 7,000 usuarios.

## 🎯 Objetivos Principales

1.  **Diagnóstico:** Determinar el porcentaje actual de evasión y los segmentos más afectados.
2.  **Identificación de Patrones:** Analizar cómo variables demográficas, financieras y de servicios influyen en la decisión del cliente.
3.  **Validación Estadística:** Utilizar mapas de calor de correlación para confirmar hipótesis visuales.
4.  **Estrategia:** Proponer acciones comerciales concretas para reducir la tasa de bajas.

## 🛠️ Tecnologías y Herramientas

* **Python:** Lenguaje principal.
* **Pandas:** Manipulación de datos, normalización de JSON y limpieza.
* **Matplotlib & Seaborn:** Visualización de datos (Countplots, Histplots, Heatmaps).
* **Jupyter Notebook:** Entorno de desarrollo interactivo.

## ⚙️ Procesamiento y Limpieza de Datos

El dataset original presentaba desafíos técnicos que fueron resueltos mediante Ingeniería de Datos:

* **Manejo de JSON Anidado:** Se utilizó `json_normalize` para desagregar estructuras complejas y se unificaron mediante `pd.concat`.
* **Transformación de Variables:**
    * Conversión de variables binarias ("Yes"/"No") a numéricas (`1`/`0`) con mapeo lógico manual.
    * *Corrección Clave:* Se invirtió la lógica de variables como "Soporte Técnico" para que el valor `1` representara la posesión del servicio, permitiendo una lectura correcta de correlaciones positivas.
* **Ingeniería de Características:** Creación de la variable `Cargos Diarios` para granularizar el análisis financiero.

## 📊 Análisis Exploratorio (EDA) y Hallazgos

A través del análisis visual y estadístico, se detectaron los siguientes "Insights" de negocio:

### 1. El Factor Contractual (El hallazgo más crítico)
El tipo de contrato es el predictor número uno de la retención.
* **Riesgo:** Los usuarios con contratos "Mes a Mes" (*Month-to-month*) presentan la tasa más alta de abandono.
* **Seguridad:** Los contratos a "1 Año" o "2 Años" blindan al cliente contra la competencia.

### 2. Servicios "Ancla"
Contrario a la intuición de que "vender más molesta al cliente", los datos demostraron que ciertos servicios actúan como barreras de salida:
* Clientes con **Soporte Técnico** y **Seguridad Online** tienen una tasa de retención significativamente mayor.
* La falta de estos servicios aumenta la probabilidad de fuga.

### 3. Matriz de Correlación
El análisis matemático confirmó que:
* Existe una **Correlación Positiva (Rojo)** entre la retención y variables como: Antigüedad (*Tenure*), Contratos largos y Entorno familiar (Pareja/Dependientes).
* Existe una **Correlación Negativa (Azul)** con los Costos (*Monthly Charges*). A mayor precio, mayor sensibilidad al abandono.

## 🚀 Recomendaciones Estratégicas

Basado en los datos, se proponen las siguientes acciones para Telecom X:

1.  **Migración de Contratos:** Implementar campañas agresivas de descuentos (ej. 15% los primeros 3 meses) para migrar usuarios de esquemas mensuales a anuales.
2.  **Paquetización (Bundling):** Incluir *Soporte Técnico* y *Seguridad Online* en los planes base para aumentar el costo de cambio del cliente (Barrera de salida).
3.  **Fidelización Familiar:** Crear promociones "Plan Familiar" para usuarios solteros, aprovechando que los clientes con dependientes son más estables.
4.  **Incentivos por Antigüedad:** Programas de recompensas en los meses críticos (3, 6 y 9) para superar la curva de aprendizaje y riesgo inicial.

## 📂 Estructura del Repositorio
¡Claro que sí! Aquí tienes un README.md profesional, estructurado y redactado específicamente para tu proyecto de Telecom X.

He resaltado los puntos técnicos fuertes que implementaste (como el manejo de JSON anidado y la corrección de la matriz de correlación) para que quien vea tu repositorio note tu nivel técnico.

Solo copia el siguiente bloque de código y pégalo en un archivo llamado README.md en la raíz de tu repositorio.

Markdown

# 📊 Análisis de Evasión de Clientes (Churn) - Telecom X

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Library-Pandas-150458)
![Seaborn](https://img.shields.io/badge/Library-Seaborn-green)
![Status](https://img.shields.io/badge/Status-Finalizado-success)

## 📖 Descripción del Proyecto

Este proyecto consiste en un análisis de datos exhaustivo para la empresa ficticia **Telecom X**, con el objetivo de identificar las causas raíz de la fuga de clientes (*Churn*) y proponer estrategias de retención basadas en datos.

El análisis abarca desde la limpieza de datos complejos (JSON anidados) hasta la modelación estadística mediante matrices de correlación y visualización avanzada, permitiendo detectar patrones de comportamiento en más de 7,000 usuarios.

## 🎯 Objetivos Principales

1.  **Diagnóstico:** Determinar el porcentaje actual de evasión y los segmentos más afectados.
2.  **Identificación de Patrones:** Analizar cómo variables demográficas, financieras y de servicios influyen en la decisión del cliente.
3.  **Validación Estadística:** Utilizar mapas de calor de correlación para confirmar hipótesis visuales.
4.  **Estrategia:** Proponer acciones comerciales concretas para reducir la tasa de bajas.

## 🛠️ Tecnologías y Herramientas

* **Python:** Lenguaje principal.
* **Pandas:** Manipulación de datos, normalización de JSON y limpieza.
* **Matplotlib & Seaborn:** Visualización de datos (Countplots, Histplots, Heatmaps).
* **Jupyter Notebook:** Entorno de desarrollo interactivo.

## ⚙️ Procesamiento y Limpieza de Datos

El dataset original presentaba desafíos técnicos que fueron resueltos mediante Ingeniería de Datos:

* **Manejo de JSON Anidado:** Se utilizó `json_normalize` para desagregar estructuras complejas y se unificaron mediante `pd.concat`.
* **Transformación de Variables:**
    * Conversión de variables binarias ("Yes"/"No") a numéricas (`1`/`0`) con mapeo lógico manual.
    * *Corrección Clave:* Se invirtió la lógica de variables como "Soporte Técnico" para que el valor `1` representara la posesión del servicio, permitiendo una lectura correcta de correlaciones positivas.
* **Ingeniería de Características:** Creación de la variable `Cargos Diarios` para granularizar el análisis financiero.

## 📊 Análisis Exploratorio (EDA) y Hallazgos

A través del análisis visual y estadístico, se detectaron los siguientes "Insights" de negocio:

### 1. El Factor Contractual (El hallazgo más crítico)
El tipo de contrato es el predictor número uno de la retención.
* **Riesgo:** Los usuarios con contratos "Mes a Mes" (*Month-to-month*) presentan la tasa más alta de abandono.
* **Seguridad:** Los contratos a "1 Año" o "2 Años" blindan al cliente contra la competencia.

### 2. Servicios "Ancla"
Contrario a la intuición de que "vender más molesta al cliente", los datos demostraron que ciertos servicios actúan como barreras de salida:
* Clientes con **Soporte Técnico** y **Seguridad Online** tienen una tasa de retención significativamente mayor.
* La falta de estos servicios aumenta la probabilidad de fuga.

### 3. Matriz de Correlación
El análisis matemático confirmó que:
* Existe una **Correlación Positiva (Rojo)** entre la retención y variables como: Antigüedad (*Tenure*), Contratos largos y Entorno familiar (Pareja/Dependientes).
* Existe una **Correlación Negativa (Azul)** con los Costos (*Monthly Charges*). A mayor precio, mayor sensibilidad al abandono.

## 🚀 Recomendaciones Estratégicas

Basado en los datos, se proponen las siguientes acciones para Telecom X:

1.  **Migración de Contratos:** Implementar campañas agresivas de descuentos (ej. 15% los primeros 3 meses) para migrar usuarios de esquemas mensuales a anuales.
2.  **Paquetización (Bundling):** Incluir *Soporte Técnico* y *Seguridad Online* en los planes base para aumentar el costo de cambio del cliente (Barrera de salida).
3.  **Fidelización Familiar:** Crear promociones "Plan Familiar" para usuarios solteros, aprovechando que los clientes con dependientes son más estables.
4.  **Incentivos por Antigüedad:** Programas de recompensas en los meses críticos (3, 6 y 9) para superar la curva de aprendizaje y riesgo inicial.

## ✒️ Autor

**Jesus Antonio Torres Contreras**
* https://www.linkedin.com/in/jesús-antonio-torres-contreras-718069168/
* https://github.com/MrX7Torres

---
*Este proyecto fue realizado como parte de un desafío de análisis de datos enfocado en Business Intelligence y Data Science.*
