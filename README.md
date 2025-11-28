# Fundamentos de Ciencia de Datos: Análisis de la Demanda Energética en Tetuán: Influencia de Variables Climáticas y Patrones Cíclicos Horarios.
##  Descripción general del proyecto
El objetivo de este proyecto es analizar la relación entre el consumo eléctrico y las variables climáticas (temperatura, humedad y velocidad del viento), así como los factores temporales (hora y día), con el fin de identificar patrones de comportamiento energético y posibles factores que influyen significativamente en la demanda eléctrica de la ciudad de Tetuán, Marruecos. El fin último es establecer una base sólida para el desarrollo de modelos de predicción de la demanda a corto plazo.

## Estructura del repositorio
 Estructura del repositorio:
 
📁 Fundamentos_cc_datos/ │

├── 📁 datos/
|├── Tetuan City power consumption.csv
|└── Tetuan_City_power_consumption_clean (2).csv
|

├── 📁 informe/
│ ├── articulo_academico_karen_cardona_gutierrez.pdf
│

├── 📁 proyecto_aula/
│ ├── py_karen_cardona_gutierrez_01_analisis_inicial.ipynb
│ ├── py_karen_cardona_gutierrez_02_analisis_y_atipicos.ipynb
│ ├── py_karen_cardona_gutierrez_03_Imputacion_escalamiento_transformacion.ipynb
| └── py_karen_cardona_gutierrez_avances.ipynb
│

|├── 📁 recursos/
│ └── referencias
|

├── 📁 sesiones_practicas/
│ ├── FCD_U2_a_ciclo_de_vida.ipynb
│ ├── sc_1_karen_cardona.ipynb
| ├── sp_2_karen_cardona_gutierrez.ipynb
| ├── sp_3_karen_cardona_gutierrez (1).ipynb
│ └── sp_4_karen_cardona_gutierrez.ipynb
│
│

└── README.md

## Principales hallazgos
El análisis exploratorio y de preprocesamiento ha revelado varios patrones cruciales en la demanda energética de Tetuán:

Factor Climático Dominante: La Temperatura es la variable con mayor correlación lineal positiva con el consumo en las tres zonas (coeficientes de 0.38 a 0.49). Este es un factor crítico para el modelado de la demanda.

Patrón Temporal Estructural: Se identificó un Pico de Demanda Vespertino altamente consistente que ocurre entre las 19:00 y 21:00 h en todas las zonas, reflejando hábitos de uso agregados.

Comportamiento por Zonas:

Zona 1: Presenta el mayor consumo promedio y la mayor variabilidad.

Zona 3: Es la zona más anómala, con el menor promedio pero la mayor asimetría (1.02) y curtosis (1.08), lo que indica la presencia de picos de consumo extremos poco frecuentes pero intensos.

Reducción de Dimensionalidad (PCA): El sistema es altamente predecible, ya que solo los dos primeros componentes principales (PC1: Demanda Térmica Agregada y PC2: Variabilidad Atmosférica) explican el 70.52% de la varianza total.

Preprocesamiento: Se confirmó la integridad del dataset (0% nulos) y se aplicó la estandarización (StandardScaler) a las variables numéricas, preservando los valores atípicos (considerados eventos genuinos del sistema).


## Autor
Karen Cardona Gutierrez.

Estudiante de Ingeniería de Sistemas.

karen.cardonag@udea.edu.co

## Librerias utilizadas

* Python 3.x

* Pandas – Manejo y limpieza de datos

* Matplotlib / Seaborn – Visualización

* Scikit-learn – Algoritmos de Machine Learning, PCA y preprocesamiento (StandardScaler, OneHotEncoder)

* NumPy – Operaciones numéricas

* Statsmodels – Modelado estadístico y regresión múltiple
  
* Jupyter Notebook – Desarrollo y documentación del análisis



