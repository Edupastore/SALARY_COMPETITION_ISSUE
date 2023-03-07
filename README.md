# SALARY_COMPETITION_Proyect

![elsdiners](https://github.com/Edupastore/SALARY_COMPETITION_ISSUE/blob/main/img/dineritus.jfif)


## ⛓️ Índice de contenidos

1.[✍️ Descripción del proyecto](#descripción)\
2.[👀 Exploración y preparación de los datos (análisis y limpieza)](#limpieza)\
3.[📈 Entrenamiento y testeo de modelos de Machine Learning](#traintest)\
4.[⏫ Resultados: mejor modelo](#resultados)\

## ✍️ Descripción

Este proyecto trata sobre una competición en la plataforma Kaggle, cuya meta es predecir el salario de los trabajos de científicos de datos en USD. Para ello, exploraremos y limpiaremos unos datos contenidos en un fichero csv llamado "salaries_data", para después entrenar un modelo de Machine Learning y posteriormente testear y subir la muestra a Kaggle con el objetivo de reducir el RMSE (evaluamos el error) en el salario que tratamos de predecir.

## 👀 Exploración y preparación de los datos (análisis y limpieza)

Para limpiar los datos, hemos seguido los siguientes pasos:

- Hemos explorado nuestro dataset para ver a qué nos enfrentábamos; hemos observado que no hay nulos.
- Hemos prescindido de varias columnas al pensar que no tenían peso a la hora de poder predecir nuestra variable objetivo.
- Hemos hecho una serie de transformaciones en varias columnas para homogeneizar los datos.
- Las columnas categóricas las hemos transformado a númericas mediante get_dummies.
- Hemos chequeado las correlaciones entre las distintas variables y nuestra variable objetivo.
- Hemos comprobado que no había registros duplicados.

## 📈 Entrenamiento y testeo de modelos de Machine Learning

A continuación, hemos hecho un split para separar los datos en datos de entrenamiento y de testeo (tanto para nuestras X, que son las variables, como para la Y, que es nuestra variable objetivo, o sea, los salarios en USD).

Al entrenar los datos pasándole "lazy", hemos visto que el modelo que mejor se ajusta es el GammaRegressor; esto quiere decir que es el que nos devuelve menor error (RMSE) al hacer la predicción.

Para finalizar, hemos hecho el mismo proceso para la fase de testeo y hemos exportado los datos a un csv llamado salary_predict_usd que hemos subido a Kaggle.

## ⏫ Resultados: mejor modelo

Como hemos comentado en el epígrafe anterior, el modelo que mejor se ajusta a los datos con los que hemos trabajado es el GammaRegressor.

Al subir el fichero a Kaggle, hemos visto que la puntuación que hemos obtenido es de 43118.12176 y el ranking público nos eleva a la décima posición:

![posizione](https://github.com/Edupastore/SALARY_COMPETITION_ISSUE/blob/main/img/ranking.jpg)
