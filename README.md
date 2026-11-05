# ⬡ NERV DATA ANALYSIS DIVISION
### CLASSIFIED RESEARCH FILE — DIMENSIONALITY REDUCTION

```text
███╗   ██╗███████╗██████╗ ██╗   ██╗
████╗  ██║██╔════╝██╔══██╗██║   ██║
██╔██╗ ██║█████╗  ██████╔╝██║   ██║
██║╚██╗██║██╔══╝  ██╔══██╗██║   ██║
██║ ╚████║███████╗██║  ██║╚██████╔╝
╚═╝  ╚═══╝╚══════╝╚═╝  ╚═╝ ╚═════╝
```

> **NERV CENTRAL DOGMA — DATA SCIENCE RESEARCH UNIT**

| SYSTEM INFORMATION | DESCRIPTION |
|:---|:---|
| **PROJECT** | Dimensionality Reduction & Classification |
| **PROGRAM** | Diplomado en Ciencia de Datos |
| **PRACTICE** | Práctica 2 |
| **RESEARCH AREA** | Unsupervised Learning / Supervised Learning |
| **OPERATOR** | JUAN |
| **STATUS** | `IN DEVELOPMENT` |

---

## 01. MISSION BRIEFING

**MISSION OBJECTIVE: DIMENSIONALITY REDUCTION**

El objetivo de esta práctica es explorar diferentes técnicas de reducción de dimensionalidad sobre un conjunto de datos compuesto por imágenes de dígitos escritos a mano.

Cada imagen se encuentra representada mediante un vector de 784 variables, correspondientes a la intensidad de los píxeles de una imagen de 28 × 28.

A través de técnicas de reducción de dimensionalidad, se busca representar la información original en espacios de menor dimensión, facilitando su visualización y análisis, así como su posterior utilización en modelos de aprendizaje supervisado.

## 02. DATASET INFORMATION

**TARGET:** Handwritten Digit Recognition

El conjunto de datos contiene imágenes de dígitos escritos a mano, representadas numéricamente mediante sus valores de intensidad por píxel.

| VARIABLE | DESCRIPTION |
|:---|:---|
| `pixel_1 ... pixel_784` | Intensidad de color de cada píxel |
| `label` | Dígito representado por la imagen |

**Dataset specifications:**

- Image resolution: `28 × 28 pixels`
- Input features: `784`
- Target variable: `label`
- Data type: Numerical pixel intensities
- Task: Digit classification (`0–9`)

## 03. RESEARCH OPERATIONS

### 03.1 — PCA (Principal Component Analysis)

Aplicar PCA para reducir la dimensionalidad del conjunto de datos y generar representaciones gráficas que permitan identificar la distribución de los diferentes dígitos.

**Required operations:**
- Generar una visualización en 2 dimensiones.
- Generar una visualización en 3 dimensiones.
- Destacar los diferentes dígitos mediante su representación gráfica.

### 03.2 — MDS (Multidimensional Scaling)

Aplicar MDS para representar los datos en espacios de menor dimensión, buscando conservar las relaciones de distancia entre las observaciones originales.

**Required operations:**
- Generar una visualización en 2 dimensiones.
- Generar una visualización en 3 dimensiones.
- Identificar agrupaciones y similitudes entre los dígitos.

### 03.3 — t-SNE (t-Distributed Stochastic Neighbor Embedding)

Implementar t-SNE para explorar la estructura local de los datos y obtener una representación gráfica que permita distinguir los diferentes dígitos.

**Required operations:**
- Seleccionar una dimensión para la representación gráfica.
- Experimentar con diferentes configuraciones de parámetros.
- Comparar las visualizaciones obtenidas.
- Seleccionar las tres mejores configuraciones y documentar sus parámetros.

### 03.4 — SUPERVISED MODELING

Construir modelos de aprendizaje supervisado utilizando las representaciones reducidas del conjunto de datos.

**MISSION CONSTRAINTS:**

No está permitido utilizar:
- Modelos neuronales.
- Modelos de ensamble.
- Modelos que utilicen el truco del kernel.

El objetivo es encontrar la arquitectura que permita estimar correctamente el dígito correspondiente a partir de sus píxeles, utilizando los datos después de aplicar reducción de dimensionalidad.

## 04. DELIVERABLES

| ID | REQUIRED OUTPUT | STATUS |
|:---|:---|:---|
| 01 | Visualización PCA 2D y 3D | `PENDING` |
| 02 | Visualización MDS 2D y 3D | `PENDING` |
| 03 | Tres visualizaciones t-SNE con configuraciones documentadas | `PENDING` |
| 04 | Resultados del modelado supervisado | `PENDING` |
| 05 | Mejor arquitectura y ajuste correspondiente | `PENDING` |

**EVALUATION DISTRIBUTION**

- PCA y MDS: 4 puntos.
- t-SNE: 4 puntos.
- Modelado: 2 puntos.

## 05. TECHNOLOGY STACK

| TECHNOLOGY | PURPOSE |
|:---|:---|
| Python | Programming language |
| NumPy | Numerical computation |
| Pandas | Data manipulation |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Dimensionality reduction and machine learning |
| Jupyter Notebook | Experimental environment |

## 06. PROJECT STRUCTURE

```text
PRACTICA_2/
│
├── P2_M3_Reduccion_dimensionalidad.ipynb
│
├── README.md
```

## 07. EXPECTED RESULTS

Al finalizar la práctica se espera obtener:

1. Representaciones bidimensionales y tridimensionales mediante PCA y MDS.
2. Visualizaciones t-SNE que permitan distinguir los diferentes dígitos.
3. Una comparación entre configuraciones de t-SNE.
4. Modelos supervisados entrenados sobre los datos transformados.
5. Identificación de la mejor arquitectura y sus correspondientes métricas de evaluación.

## 08. FINAL REPORT

**NERV SYSTEM — RESEARCH STATUS**

```text
[ PCA ]                 UNDER ANALYSIS
[ MDS ]                 UNDER ANALYSIS
[ t-SNE ]               UNDER ANALYSIS
[ SUPERVISED MODELING ] PENDING EXECUTION

-----------------------------------------
PROJECT STATUS: IN DEVELOPMENT
OPERATOR: JUAN
-----------------------------------------
```

> "The reduction of dimensions does not imply the loss of knowledge. It reveals the structure hidden within the data."

**NERV DATA ANALYSIS DIVISION — END OF FILE**