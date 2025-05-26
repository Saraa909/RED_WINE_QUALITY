# Cualidades del Vino Tinto 
## Análisis de Agrupamiento No Supervisado – PCA, Selección de Características y K-Means

**Autora:** Sara González Rodríguez

## Descripción

Este proyecto aplica técnicas de aprendizaje no supervisado para analizar patrones ocultos en un conjunto de datos con variables numéricas. El objetivo es comparar el desempeño del algoritmo **K-Means** bajo tres enfoques distintos: con las **variables originales**, tras una **reducción de dimensionalidad mediante PCA** (componentes principales) y usando una **selección de características relevantes**. Se evalúa la calidad de los agrupamientos a través del *Silhouette Score*, buscando identificar la cantidad óptima de clusters y la mejor transformación de los datos para mejorar la cohesión interna y separación entre grupos.

## Dataset

Se utilizó un conjunto de datos con 10 variables numéricas representando características diversas de observaciones anónimas.

Las variables incluyen medidas como:

- Métricas financieras y demográficas simuladas
- Variables continuas de comportamiento o consumo
- Ninguna variable categórica

## Análisis Exploratorio de Datos (EDA)

- Se verificó que los datos estaban escalados para una correcta implementación de K-Means.
- No se encontraron valores nulos ni outliers significativos.
- Se realizó un análisis de correlación, que permitió identificar redundancia entre algunas variables.
- Se prepararon los datos para PCA y selección de características usando criterios de varianza explicada y relevancia estadística.

## Modelado y Resultados

Se aplicó el algoritmo K-Means bajo tres enfoques:

- **Datos Originales:** Sin transformación previa.
- **PCA (2 Componentes):** Reducción de dimensionalidad para mejorar visualización y separación.
- **Selección de Características:** Eliminación de variables irrelevantes con base en su contribución a la varianza.

### Métrica de Evaluación:
Se utilizó el **Silhouette Score** para medir la calidad del agrupamiento, evaluando valores de K entre 2 y 6.

| Método                 | Mejor K | Silhouette Score |
|------------------------|---------|------------------|
| Original               | 2       | 0.214            |
| PCA (2 Componentes)    | 2       | 0.399            |
| Selección de Variables | 4       | 0.258            |


## Conclusiones

Los resultados muestran que la reducción de dimensionalidad mediante **PCA** no solo mejora la visualización del agrupamiento, sino que también incrementa significativamente la calidad del clustering, alcanzando un *Silhouette Score* de 0.399 con **K=2**. En contraste, los datos originales mostraron menor capacidad de formar grupos definidos. La **selección de características** ofreció un desempeño intermedio, con su mejor resultado en **K=4**. Estos hallazgos destacan la importancia de transformar adecuadamente los datos antes de aplicar algoritmos no supervisados como K-Means.

## Contenido del Repositorio

- Notebook con EDA, PCA, selección de características y clustering, gráficos.
- Dataset utilizado
- Archivo README
# RED_WINE
# RED_WINE
# RED_WINE_QUALITY
