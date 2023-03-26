# **Proyecciones de ventas alimenticias**

En este repositorio encontrarán información acerca de la proyección de ventas alimenticias realizada con árboles de regresión, en el transcurso de este proyecto limpié la data, realicé un análisis de las características, preparé la data para el aprendizaje automático y ejecuté los modelos de regresión lineal y árboles de regresión, siendo los segundos el modelo escogido para las predicciones de ventas.

Se encuentran subidos al repositorio los Notebooks de Google Colab, la presentación en PowePoint y una grabación de la explicación de dicha presentación.

## **Visualizaciones**
### Mapa de calor
![Mapa_calor](https://user-images.githubusercontent.com/87196602/227752782-d57c418a-1fd7-4890-b390-4ae81ebd1130.png)

Un mapa de calor nos ayuda a identificar la correlación entre características numéricas en nuestro conjunto de datos. En este caso pueden observar que la característica de “Precio máximo de venta al público” (Item_MRP) tiene una correlación moderada con las “Ventas totales del producto” (Item_Outlet_Sales), esto a primera vista nos indica que a mayor precio de venta tendremos mayores ventas.

El resto de características no tienen una correlación fuerte, sin embargo, no quiere decir que no sean importantes. 

### Cantidad y valor de productos vendidos
![Tipos_productos_vendidos](https://user-images.githubusercontent.com/87196602/227752880-927c4bf1-4763-42a9-8699-c37f9252dada.png)

![Valor_total_productos_vendidos](https://user-images.githubusercontent.com/87196602/227752885-62c62eec-d2f2-41ec-a49b-f2690b6f38b7.png)

Podemos observar que las “Frutas y vegetales” y los “Snacks” son los tipos de productos más vendidos en cuando a cantidad y a valor en ventas.

### Productos vendidos por cantidad de grasa
![Items_vendidos_contenido_grasa](https://user-images.githubusercontent.com/87196602/227752907-f08e594b-bb90-4751-817e-3d2a07270691.png)

En este gráfico pueden observar que los productos con menor cantidad de grasa (Low Fat) son más vendidos que los productos regulares, lo que podría significar un hábito saludable de las personas que visitan las tiendas.

### Valor de ventas por tiendas
![Valor_ventas_por_tienda](https://user-images.githubusercontent.com/87196602/227752932-b7000b5f-8e4b-4c95-8129-b770de75a36b.png)

En este gráfico podemos observar que existe una mayor cantidad de ventas en los Supermercados (tipo 1, 2, y 3), por tanto, la mayor cantidad de venta de productos es realizada en los supermercados, siendo los supermercados de tipo 1 la mayoría.

Las tiendas de abarrotes tienen una menor cantidad de ventas.

## **Modelos de aprendizaje automático**
### Modelo de regresión lineal
* R^2 en conjunto de entrenamiento:  0.5605554544355624
* R^2 en conjunto de prueba:  0.5658838444256
* RECM en conjunto de entrenamiento:  1140.4019761442698
* RECM en conjunto de prueba:  1094.4024001708467

### Modelo de árbol de regresión
* R^2 en conjunto de entrenamiento:  0.6039092654846363
* R^2 en conjunto de prueba:  0.5949542729674069
* RECM en conjunto de entrenamiento:  1082.6878514934986
* RECM en conjunto de prueba:  1057.1243831290897

**Modelo recomendado:** recomiendo utilizar el modelo de árboles de regresión, debido a que, luego de modificar un poco sus valores por defecto los valores de las métricas de predicción son mejores en los datos de prueba, además la diferencia del RECM entre los datos de entrenamiento y de prueba es menor.

## **Conclusiones**
* El precio de venta al público (MRP) está directamente relacionado con las ventas, se sugiere mantener precios competitivos para aumentar las ventas.
* Los productos bajos en grasa son los más vendidos, se recomienda de igual manera mantener precios competitivos y se podrían realizar promociones para los productos con contenido regular si se desea aumentar sus ventas.
* Las tiendas con mayor cantidad de ventas son los Supermercados, se debe dar prioridad a estas tiendas en campañas publicitarias. Las tiendas de abarrotes no representan muchas ventas, sin embargo, sería posible aumentar las ventas enfocándonos en los productos que más se venden.
