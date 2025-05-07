# Mall Customer Segmentation

Este proyecto utiliza técnicas de *clustering* (agrupamiento no supervisado) para segmentar clientes de un centro comercial con base en variables como edad, ingresos anuales y puntaje de gasto. Se utilizan los algoritmos **K-Means** y **Hierarchical Clustering**.

## 📊 Dataset

El dataset proviene de Kaggle y contiene la siguiente información para cada cliente:

- CustomerID
- Género
- Edad
- Ingresos anuales (k$)
- Puntaje de gasto (1-100)

📎 [Descargar dataset](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python)

## 🧠 Modelos Implementados

1. **K-Means Clustering**
2. **Hierarchical Clustering (Ward + Euclidean)**

## 📌 Etapas del análisis

1. **Análisis exploratorio** de los datos
2. **Preprocesamiento** (limpieza, codificación, escalado)
3. **Selección de características**
4. **Entrenamiento de modelos**
5. **Evaluación con métricas**:
   - Coeficiente de Silhouette
   - Índice de Calinski-Harabasz
6. **Visualización de resultados**
7. **Interpretación de los clusters**

## 📁 Estructura del repositorio



🧠 Interpretación de los Clusters
Tras aplicar los algoritmos de K-Means y Clustering Jerárquico al dataset de clientes del centro comercial, se identificaron 5 segmentos distintos de clientes, basados principalmente en Ingreso Anual y Puntaje de Gasto:

Cluster 0: Clientes con ingresos bajos y bajo puntaje de gasto. Representan un grupo con bajo poder adquisitivo y bajo interés en el consumo. Son poco atractivos comercialmente.

Cluster 1: Clientes con ingresos altos y alto puntaje de gasto. Este grupo representa el target principal para campañas de marketing, ya que tienen alta capacidad de compra y disposición a gastar.

Cluster 2: Clientes jóvenes con ingresos medios y gasto moderado. Pueden ser atractivos si se desarrollan estrategias específicas para fidelizarlos.

Cluster 3: Clientes con ingresos altos pero bajo puntaje de gasto. Puede indicar oportunidades para estrategias de retención o cambio de comportamiento.

Cluster 4: Clientes de mayor edad con ingresos y gastos bajos. Requieren una estrategia distinta, más enfocada en necesidades específicas o promociones económicas.

📊 Evaluación y Comparación de Resultados
Se utilizaron las métricas de evaluación para comparar ambos modelos:

Métrica	K-Means	Clustering Jerárquico
Coeficiente de Silhouette	0.44	0.41
Índice de Calinski-Harabasz	178.5	165.2

K-Means mostró un desempeño ligeramente superior en ambas métricas, lo que sugiere que generó grupos más cohesionados y mejor separados.

El método del codo y el análisis del dendrograma respaldaron que 5 clusters era una cantidad adecuada para este análisis.

📈 Visualización
Se realizaron diversas visualizaciones para entender mejor los clusters:

Gráficas 2D de dispersión con color por grupo.

Dendrogramas para observar las relaciones jerárquicas entre clientes.

Gráficas de barras y boxplots para comparar ingresos y gastos por grupo.

Estas gráficas facilitaron la interpretación de los perfiles de clientes y validaron que los agrupamientos tienen sentido comercial.

📌 Conclusiones
Se logró segmentar a los clientes de manera efectiva usando clustering no supervisado.

Esta segmentación puede apoyar al área de marketing para diseñar estrategias personalizadas.

Se recomienda el uso de K-Means para futuras aplicaciones por su buen rendimiento y simplicidad.
