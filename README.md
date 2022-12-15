![Ironhack logo](https://i.imgur.com/1QgrNNw.png) 

## Final Project: PREDICCION DEL VALOR FINAL DE LAS SUBASTAS

<p align="center"> <img src="https://github.com/Artturoo/Final_Project/blob/main/img/primera.png" width="700" height="350">  </p>

## INDICE


 1. Objetivo.
 2. Procedimientos.
 3. Machine Learning.

---

## 1. 📈 OBJETIVO


- Predecir la puja final de cada subasta en España.

El tipo de bien subastado que se ha elegido para el proyecto: Inmuebles; Vivienda.

Variables a tener en cuenta para la predicción:

    - Cantidad Reclamada (deuda del propietario de la vivienda).
    - Valor Subasta (valor que le da el Juez a esa vivienda).
    - Provincia, Localidad, Código Postal y el precio por metro cuadrado.

---

## 2. 🗂 PROCEDIMIENTO


Se realziará una ETL: extracción, transformación y carga de los datos.

Para la extracción, se utilizará las subastas ya finalizadas para poder predecir en las futuras subastas la mejor puja final.

Primero, se escrapeará la página oficial del <b>BOE</b> donde se extraerán datos específicos que se encuentran en cada subasta . Posteriormente, con el código postal, se escrapeará la página oficial de <b>RealAdvisor</b> para extraer el precio por metro cuadrado de cada una de las subastas.

Para la extracción de datos, se utilizará la herramienta selenium y Joblib (librería de Python) que permitirá paralelizar un programa.

Datos totales extraidos para el proyecto: 9.500 datos.

Años que se analizará las subastas: 2016 - 2022

Una vez obtenidos los datos, se transformarán y se generará las relaciones entre las tablas. En este caso, se unirán las tablas obtenidas en un único DataFrame, para luego analizar y lograr la mejor predicción final de cada subasta.

---

## 3. 📊 Machine Learning:


PASOS:

    - Preparar los datos para los diversos modelos (proceso empírico).
    - Entrenar y testear los modelos de Machine Learning.

El mejor modelo entrenado extraído (según las variables mencionadas anteriormente) para la predicción del valor final en una subasta es, el modelo Lgbmr, donde se observa un <b>r2 0.873.</b>

---

## 🛠 HERRAMIENTAS


- <b>Python:</b> Selenium, Joblib, Multiprocessing Pandas, Numpy, Regex, Pylab, Seaborn.
- <b>Tableau.</b>


---

## FUENTES


- <b>BOE:</b>  https://subastas.boe.es/
- <b>RealAdvisor:</b>  https://realadvisor.es/es/precios-viviendas











