# Proyecto-Final-Sprint-7-TripleTen

# 📊 Análisis de Comportamiento de usuario: compañía ConnectaTel

## 🎯 Objetivo del Proyecto
El propósito de este análisis es transformar los datos de consumo de **ConnectaTel** en insights accionables para optimizar la oferta comercial. El enfoque principal radica en identificar patrones de uso, segmentar a los usuarios y detectar comportamientos atípicos que puedan sesgar la estrategia de negocio.

## 🛠️ Tecnologías Utilizadas
* **Python**
* **Pandas:** Limpieza y manipulación de datos.
* **Seaborn & Matplotlib:** Visualización estadística.
* **NumPy:** Operaciones matemáticas y manejo de datos nulos.

## 📁 Estructura del Dataset
El proyecto integra datos de tres fuentes principales:
1. **plans.csv →** información de los planes actuales (precio, minutos incluidos, GB incluidos, costo por extra)
2. **users.csv →** información de los clientes (edad, ciudad, fecha de registro, plan, churn)
3. **usage.csv →** detalle del uso real de los servicios (llamadas y mensajes)

## 🧹 Proceso de Limpieza y Preprocesamiento
Para garantizar la integridad del análisis, se realizaron las siguientes acciones:
* **Tratamiento de Nulos:** Se identificó un 11.72% de datos ausentes en la columna `city`, los cuales fueron categorizados como "Unknown".
* **Corrección de Tipos:** Conversión de fechas y limpieza de caracteres especiales.
* **Manejo de Outliers:** Se aplicó la técnica de **IQR (Rango Intercuartílico)** para identificar consumos extremos. En el caso de los minutos de llamada, se realizó una winsorización en 61.85 minutos para evitar sesgos en la media.

## 📈 Hallazgos Principales
### 1. Segmentación por Edad
Los usuarios de entre **30 y 60 años** representan el segmento más valioso para la empresa, con una alta lealtad al plan básico pero con necesidades de consumo creciente.

### 2. Comportamientos Atípicos
Se detectaron usuarios "Heavy Users" cuyo consumo de minutos duplica el límite superior normal, sugiriendo un uso comercial o profesional del servicio.

### 3. Potencial crecimiento
Se recomiendan planes de fidelización para los clientes jóvenes, y evitar la deserción de estos, pues a largo plazo serán clientes que aportarán gran valor a la compañía. 

> 

## 💡 Recomendaciones Estratégicas
* **Mejorar:** Migrar a los usuarios adultos con "Consumo Medio" hacia un plan intermedio.
* **Plan Business:** Crear una oferta específica para los outliers detectados para proteger la rentabilidad de los planes básicos.
* **Optimización Digital:** Reforzar paquetes de datos para el segmento que prefiere mensajería sobre llamadas de voz.
* **fidelización:** Campañas de fidelización de clientes jóvenes. 

---
## 🚀 Cómo ejecutar el proyecto
1. Clona el repositorio: `git clone https://github.com/JhonYara/Proyecto-Final-Sprint-7-TripleTen`
3. Abre el notebook: `jupyter notebook notebook:ConnectaTel.ipynb`
