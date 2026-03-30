# Taller Módulo 1 — Salud Mundial

**Autor:** Tu Nombre  
**Máster:** IA & Data Science — DevSeniorCode

---

## Descripción

Este proyecto realiza un análisis exploratorio de datos de salud a nivel mundial usando Python y Pandas. Se aplican técnicas de limpieza de datos, filtrado, agrupación y clasificación para extraer conclusiones sobre la relación entre indicadores de salud, nivel de ingresos y región geográfica.

---

## Dataset

El archivo `salud_mundial.csv` contiene información de **159 países** con **13 columnas**:

- **Identificación:** `pais`, `region`, `nivel_ingresos`
- **Salud:** `esperanza_vida`, `mortalidad_infantil`, `vacunacion_pct`
- **Recursos médicos:** `medicos_por_1000`, `camas_hospital_por_1000`
- **Economía:** `gasto_salud_usd`
- **Estilo de vida:** `obesidad_pct`, `diabetes_pct`, `tabaquismo_pct`, `poblacion_urbana_pct`

El dataset contenía 53 valores nulos distribuidos en 9 columnas, los cuales fueron imputados con la media de cada columna.

---

## Cómo ejecutar

1. Clona el repositorio: `git clone [url]`
2. Instala dependencias: `pip install pandas jupyter`
3. Ejecuta: `jupyter notebook taller_modulo1.ipynb`

---

## Hallazgos principales

- **Hallazgo 1:** Existe una correlación fuerte (r = 0.67) entre el gasto en salud y la esperanza de vida — los países que más invierten en salud viven más años. Slovakia gasta 560 veces más que Afghanistan por persona.
- **Hallazgo 2:** Los países con más médicos por habitante tienen dramáticamente menor mortalidad infantil (r = −0.71). El cuartil con menos médicos registra 60 muertes por cada 1,000 nacidos vivos, frente a solo 6.6 en el cuartil con más médicos.
- **Hallazgo 3:** Los países de ingresos bajos (46 países) tienen un promedio de mortalidad infantil de 63 muertes por cada 1,000 nacidos vivos — más del doble que la mediana global de 23.7, evidenciando una brecha crítica de desigualdad en salud.

---

## Tecnologías

Python · Pandas · Jupyter Notebook · Git · GitHub
