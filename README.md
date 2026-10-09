# Análisis estadístico de calidad del café arábica (CQI)
## Descripción general

Análisis estadístico de datos relacionado con la calidad del café del país de cada continente de acuerdo con la **Coffee Quality Institute** o (CQI), que es una organización sin ánimos de lucro que se dedica a mejorar el valor y calidad del café en el mundo, con el propósito de promover café de calidad a través de la investigación, entrenamiento y programas de certificación.

Tras eso, se ha realizado una base de datos con el propósito de saber más al respecto con la calidad del café, así como saber qué país produce el café mejor calificado?, ¿Qué atributo del café tiene más relación con la calificación total? y si Hay diferencia estadística en la calidad del café entre continentes

## Datos

El dataset obtenido a través de la base de datos de la red de CQI a través de Kaggle, contiene una lista con los países productores, los propios productores, así como su certificación, tipos de suelo y otros factores que suelen afectar la calidad del café. En el dataset se encuentran las calificaciones de calidad del café por evaluaciones de atributo que son las siguientes

- `Aroma`: Escencia o fragancia del café.

- `Flavor`: Sabor del café evaluado por la dulcedad, amargez y acidez u otros sabores.

- `Aftertaste`: Referente al sabor que queda después de consumirlo.

- `Acidity`: Referente a la claridad del sabor

- `Body`: Referente a la viscosidad o espesor del café al consumirlo

- `Balance`: Referente a que tan bien trabajan juntos los diferentes componentes del sabor

- `Uniformity`: Referente a la consistencia del café de taza a taza

- `Sweetness`: Referente al sabor dulce, si es deseable en la calidad del café


## Metodologías

Para la realización del proyecto, se realizaron las siguientes acciones:

- Análisis estadísitico: Graficación de barras, boxplot y scatterplot para la identificacíón u estudio de la calidad del café por país, y cómo contribuye los atributos del café y las muestras en el estudio

- Análisis de correlación: Correlación con los atributos del café por las puntuaciones.

- Pruebas de estadística: Uso de las pruebas de estadistica *ANOVA* con eta², para comparar las medias de los tres grupos, e identificar las diferencias de cada una. Prueba de estadística *Kruskal-Wallis* con epsilon² para comprobar diferencias significativas entre las tres muestras, y un post-hoc (Tukey y Mann-Whitney con Bonferroni) para obtener un resultado global significativo.

## Hallazgos principales y observaciones

Tras la realización de las metologías usadas, se encontraron algunos datos interesantes:

- Etiopía obtiene el **mayor promedio** entre los países con muestra suficiente con *84.96 puntos*. Le siguen Tanzania *84.74 puntos* con 6 muestras, Taiwán *84.35 puntos* con 61 muestras y Guatemala *84.30 puntos* con 21 muestras. 

- Mientras que el **más bajo** fué El Salvador con *81.53 puntos*, Brasil *81.88* y Nicaragua *81.89*, así que entre el primero y el último hay unos 3.4 puntos de diferencia.

- El Atributo **"Flavor"** es el que más se relaciona con la calificación total.
Con un R² de 0.88: explica cerca del 88 % de la variación del puntaje total.

- `Americas` posee 100 *números de muestra*, no obstante `Africa` es el que posee el promedio más alto con un promedio de *84.63 puntos* a pesar de que este último tiene 23 *números de muestra*, que es una cifra baja.

América obtiene puntajes menores que África y Asia, pero la diferencia es modesta. Hay que tomarla con cautela: África tiene pocos registros (23), Taiwán aporta 61 de los 84 de Asia, y hay varios lotes por país, así que las observaciones no son totalmente independientes.

Se recomienda terminar la estadística en las dos pruebas, ya que hay diferencias significativas entre continentes, pero el tamaño del efecto es de pequeño a moderado: el continente explica solo alrededor del 8 % de la variación en la calidad.


