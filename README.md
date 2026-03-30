# 🌍 Análisis de Salud Mundial con Python y Pandas

**Autor:** Andres Felipe Mojarrango Silgado
**Curso:** Introducción a Data Science  
**Fecha:** Marzo 2026

\---

## 📋 Descripción del dataset

El dataset `salud\\\_mundial.csv` contiene indicadores de salud de **159 países** alrededor del mundo.

|Característica|Detalle|
|-|-|
|Filas|159 países|
|Columnas|13 variables|
|Fuente|Datos simulados con base en indicadores OMS / Banco Mundial|

### Variables incluidas

|Variable|Descripción|
|-|-|
|`pais`|Nombre del país|
|`region`|Continente o región geográfica|
|`nivel\\\_ingresos`|Low / Medium / High / Very High|
|`esperanza\\\_vida`|Años promedio de vida|
|`gasto\\\_salud\\\_usd`|Gasto per cápita en salud (USD)|
|`mortalidad\\\_infantil`|Muertes por cada 1,000 nacidos vivos|
|`medicos\\\_por\\\_1000`|Médicos por cada 1,000 habitantes|
|`poblacion\\\_urbana\\\_pct`|% de población en zonas urbanas|
|`obesidad\\\_pct`|% de población con obesidad|
|`diabetes\\\_pct`|% de población con diabetes|
|`tabaquismo\\\_pct`|% de población fumadora|
|`camas\\\_hospital\\\_por\\\_1000`|Camas hospitalarias por 1,000 hab.|
|`vacunacion\\\_pct`|% de cobertura de vacunación|

\---

## ▶️ Cómo ejecutar el notebook

### Requisitos previos

* Python 3.11.15
* pip instalado

### Pasos

```bash
# 1. Clona el repositorio
git clone https://github.com/tu-usuario/taller-datos.git
cd taller-datos

# 2. Crea y activa un entorno virtual
python -m venv venv
source venv/bin/activate        # Mac/Linux
venv\\\\Scripts\\\\activate           # Windows

# 3. Instala las dependencias
pip install -r requirements.txt

# 4. Abre Jupyter
jupyter notebook

# 5. Abre el archivo
# taller\\\_salud\\\_mundial.ipynb
```

### Dependencias (`requirements.txt`)

```
pandas>=2.0.0
jupyter>=1.0.0
```

\---

## 🔍 Hallazgos principales

### 1\. 💰 El gasto en salud predice la esperanza de vida

Se encontró una correlación de **r = 0.67** entre el gasto per cápita en salud y la esperanza de vida.
Slovakia gasta $10,311 USD por persona, mientras que Afghanistan gasta solo $18.4 USD — una diferencia de 560 veces.

### 2\. 👨‍⚕️ Más médicos = menos muertes infantiles

La correlación entre médicos por 1,000 habitantes y mortalidad infantil fue de **r = −0.71** (la más fuerte del análisis).
Los países con menos médicos (Q1) tienen una mortalidad infantil de 60.12, mientras que los de más médicos (Q4) registran solo 6.60.

### 3\. 🏙️ Mayor urbanización está asociada a mayor obesidad

Con una correlación de **r = 0.69**, los países más urbanizados presentan casi el doble de obesidad (25.91%) que los menos urbanizados (12.98%).

### 4\. 🌍 Europa lidera en esperanza de vida, África en el extremo opuesto

Esperanza de vida promedio por región: Europa 77.65 años vs. África 63.51 años — una brecha de 14 años.

### 5\. 🔴 Los países de ingresos bajos tienen mortalidad infantil crítica

Los 46 países clasificados como `Low` income tienen un promedio de **63.03 muertes** por cada 1,000 nacidos vivos, más del doble que la mediana global (23.70).

\---

## 🛠️ Tecnologías usadas

|Tecnología|Uso|
|-|-|
|**Python**|Lenguaje principal del análisis|
|**Pandas**|Manipulación y análisis de datos|
|**Jupyter Notebook**|Entorno interactivo de desarrollo|
|**Git**|Control de versiones local|
|**GitHub**|Alojamiento del repositorio remoto|

\---

## 

