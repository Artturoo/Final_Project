![Ironhack logo](https://i.imgur.com/1QgrNNw.png) 

# Final Project: PREDICCION VALOR FINAL SUBASTAS

<p align="center"> <img src="https://github.com/Artturoo/Final_Project/blob/main/img/primera.png" width="700" height="350">  </p>

# INDICE


 1. Objetivo.
 2. Procedimiento.
 3. Machine Learning.

---

## 1. 📈 OBJETIVO


- Predecir la puja final de cada subasta en España.

El tipo de bien subastado que hemos elegido para el proyecto: Inmuebles; Vivienda.

Variables a tener en cuenta para la predicción:

    - Cantidad Reclamada (deuda del propietario de la vivienda).
    - Valor Subasta (valor que le da el Juez a esa vivienda).
    - Provincia, Localidad, Código Postal y el precio por metro cuadrado.

---

## 2. 🗂 PROCEDIMIENTO


Se realziará una ETL: extracción, transformación y carga de los datos.

Para la extracción, se utilizará las subastas ya finalizadas para posteriormente poder predecir en las futuras subastas la mejor puja final.

Primero, se escrapeará la página oficial del <b>BOE</b> y se extraerán datos específicos de algunas de las pestañas que se encuentran en cada subasta . Posteriormente, con el código postal, se escrapeará la página oficial de <b>RealAdvisor</b> para extraer el precio por metro cuadrado de cada una de las subastas.

Para la extracciónde de datos, se utilizará la herramienta selenium y Joblib (librería de Python) que nos permitirá paralelizar un programa.

Datos totales extraidos para el proyecto: alrededor de 10.000 mil datos.

Años que se analizará las subastas: 2016 - 2022

Una vez obtenidos los datos, se procederá a transformarlos y se gerará las relaciones entre las tablas, en este caso se unirán las tablas que tenemos en un único DataFrame, para luego analizar y obtener la mejor predicción final de cada subasta.

---

## 3. 📊 Machine Learning:


PASOS:

    - Se prepararán los datos para los diversos modelos (proceso empírico).
    - Se entrenará y testeará los modelos de Machine Learning.

El mejor modelo entrenado que obtenemos (según las variables mencionadas anteriormente) para la predicción del valor final en una subasta es, el modelo Lgbmr, donde se observará un <b>r2 0.873.</b>

---

## 🛠 HERRAMIENTAS


- <b>Python:</b> Selenium, Joblib, Multiprocessing Pandas, Numpy, Regex, Pylab, Seaborn.
- <b>Tableau.</b>


---

FUENTES


- <b>BOE:</b>  https://subastas.boe.es/
- <b>RealAdvisor:</b>  https://realadvisor.es/es/precios-viviendas











