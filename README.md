# 🩺 Análisis de Casos de Anemia en la Región San Martín

Este repositorio documenta un proyecto en la creación de un dashboard interactivo en **Power BI** para el análisis y visualización de datos relacionados con los **casos de anemia en la región San Martín (Perú)**.  Los datos fueron previamente procesados en **SQL Server**, donde se implementó un modelo estrella como parte del proceso ETL.

---

## 🧪 Dataset

El conjunto de datos utilizado proviene de **archivos planos en formato CSV**, los cuales fueron descargados desde el portal oficial de **Datos Abiertos del Gobierno del Perú**. 

La fuente específica corresponde al siguiente recurso:

🔗 [Reporte de detección de casos de anemia en niños menores de 5 años en la región San Martín](https://datosabiertos.gob.pe/dataset/reporte-de-detecci%C3%B3n-de-casos-de-anemia-en-ni%C3%B1os-menores-de-05-cinco-a%C3%B1os-en-la-regi%C3%B3n-san)


---

## ⚙️ Proceso ETL

Antes del análisis visual en Power BI, se realizó un proceso completo de ETL en **SQL Server**, compuesto por las siguientes etapas:

1. **Extracción** de los archivos planos (CSV).
2. **Transformación** de los datos para limpiar inconsistencias, estandarizar formatos y normalizar estructuras.
3. **Carga** en un modelo de datos en estrella, conformado por:

   - 🟦 Tabla de hechos: `THRegistroAtencion`
   - 🟩 Tablas de dimensiones: `Paciente`, `Establecimiento`, `Diagnostico`, `Geografica`, entre otras.

Este modelo permitió optimizar las relaciones y consultas, facilitando la explotación eficiente de los datos en Power BI.

---

## 🎯 Objetivo del análisis

El objetivo del proyecto fue construir un dashboard en Power BI que permitiera:

- Identificar zonas geográficas con mayor incidencia
- Analizar la distribución por grupos etarios y sexo
- Observar tendencias a lo largo del tiempo
- Facilitar decisiones informadas en salud pública

---

## 📎 Tecnologías utilizadas

- 🛢️ **SQL Server** – Para procesos de ETL y modelado en estrella  
- 📊 **Power BI** – Para visualización de datos y creación de dashboards  
- 🧮 **DAX** – Para el cálculo de medidas, KPIs y fórmulas  
- 📁 **Archivos CSV** – Fuente de datos original
