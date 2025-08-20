![Telecom X2](https://github.com/user-attachments/assets/f6f7bf69-69db-4251-8282-f7ec8998de79)
<hr>

<p align="center">
  <img src="https://img.shields.io/badge/Estado-Finalizado-blue">
  <img src="https://img.shields.io/badge/Licencia-MIT License-orange">
</p>

### Índice
- [Descripción del proyecto](#computer-descripción-del-proyecto)
- [Gráficos y métricas](#hammer-gráficos-y-métricas)
- [Acceso al proyecto](#unlock-acceso-al-proyecto)
- [Tecnologías usadas](#briefcase-tecnologías-usadas)
- [Desarrollador](#bowtie-desarrollador)

## :computer: Descripción del proyecto
<p align="justify">
Respositorio correspondiente al tercer challenge de la especialidad de Ciencia de Datos del programa One de Alura Latam y Oracle.
  
Tras realizar el anáisis de los factores que llevan a la pérdida de clientes en la empresa TelecomX, se solicitó la elaboración de un modelo de clasificación capaz de predecir si un cliente cancelará o no el servicio contratado. En este desafío se realiza el feature engineering, entrenamiento y selección de modelos, selección de características y optimización de hiperparámetros, utilizando Python y sus principales bibliotecas para producir un modelo que obtuvo un recall de 89.84%. A partir del trabajó realizado, se respondió a la preguntas ¿Que factores son importantes al predecir si un cliente dejará la empresa?,y generó un modelo predictivo que permita a la empresa desarrollar estrategias para reducir la pérdida de cientes

El análisis se realizó como reto de la formación "Estadística y Machine Learning" del Programa ONE edición 8 de Alura Latam y Oracle.
</p>

## :hammer: Pipeline del modelo ML
:heavy_check_mark: `Preparación de los datos:` Se realizó la eliminación de variables irrelevantes y transformación OneHot de las variables categóricas.

:heavy_check_mark: `Correlación y selección de variables:` Se realizó un análisis de correlación y del factor de inflación de la varianza que permitió la selección de variables más correlacionadas con la cancelación del servicio, y que no producen multicolinealidad.

:heavy_check_mark: `Comparación de modelos predictivos:` Se comparó tres modelos ML para la clasificación de clientes en quienes hacen y no hacen Churn. La métrica más importante fue recall, pues nos interesa predecir quiénes son los clientes que cancelarán el servicio (clase positiva). Se halló que el modelo de Regresión Logística produce los mejores resultados, y se probó que el método SMOTTENN permite al modelo ML indentificar mejor los patrones de los datos durante un entrenamiento con clases balanceadas. 

:heavy_check_mark: `Optimización del modelo escogido:` Se analizó la importancia total de la permutación de las variables predictoras y escogió las nueve que producían mejoras significativas en el recall.

:heavy_check_mark: `Optimización de hiperparámetros:` Tras la selección de caterísticas, se probó las combinaciones de 4 hiperparámetros del modelo de Regresión Logística teniendo cada uno 3 posibles valores. GridSearchCV encontró la mejor combinación de hiperparámetros y se evaluó el predictor con el conjunto de prueba obteniendo un recall de 89,84%.

:heavy_check_mark: `Esportación del modelo campeón:` Con la biblioteca pickle, se exportó el predictor campeón y el transformador OneHot para su uso posterior.

## :unlock: Acceso al proyecto
Puedes acceder al repositorio GitHub del proyecto haciendo [click aquí](https://github.com/JLuceroVasquez/challenge-telecom-x-latam-parte-2).

En el repositorio, se puede abrir el cuaderno de Jupyter en Google Colab haciendo click en el badge de color azul que está al principio.

## :briefcase: Tecnologías usadas
- Pyhton
- Pandas
- Numpy
- Maplotlib
- Seaborn
- Scikit-Learn
- Imbalanced-Learn
- Statsmodels
- Pickle

## :bowtie: Desarrollador
|[<img src="https://avatars.githubusercontent.com/u/176303607?v=4" width=115> <br> <sub>Jimmy Octavio Lucero Vasquez</sub>](https://github.com/JLuceroVasquez)|
|:---:|
