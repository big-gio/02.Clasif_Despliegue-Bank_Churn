# 02.Clasif_Despliegue-Bank_Churn

## Descripción

Se analizó un conjunto de datos sobre los clientes de un banco. Datos como: sexo, salario estimado, balance, etc. Se aplicaron y se compararon diferentes algoritmos de clasificación (regresión logística, árbol de decisión, random forest y support vector machine), modificando algunos de sus hiperparámetros para encontrar el modelo más eficiente, y así determinar si el cliente fugará o no. Esto último se representa mediante la variable "Exited", que contiene valores binarios: 0 ("no fuga") y 1 ("fuga").

El proyecto está dividido en tres cuadernos de Google Colab:

* [Churn 1_Clasificaciones.] En este cuaderno se tratan los datos y se entrenan diferentes algoritmos de aprendizaje supervisado, modificando sus hiperparámetros para encontrar el modelo más eficiente para cada algoritmo.
* [Churn 2_Evaluación_Entrenamiento.] En el segundo cuaderno se prueban los diferentes modelos, se calculan sus métricas y se comparan entre sí para seleccionar el modelo óptimo que se utilizará en los nuevos datos que lleguen después. El modelo seleccionado se exporta en un archivo de extensión .pkl.
* [Churn 3_Despliegue.] Se utiliza el modelo seleccionado para predecir la fuga de nuevos clientes.

## Obtención de los datos

El archivo "Churn_Modelling.csv" se descargó de la plataforma Kaggle.

## Resultados

Al analizar el reporte final de métricas, se encontró que el mejor modelo para clasificar a los cientes, sería el de "arbol de decisión". Hubo problemas con el modelo de SVM, que provocó errores, por lo que tuvo que dejarse fuera, antes de un análisis más exhaustivo:

![Portada_Churn_Clasif](https://raw.githubusercontent.com/Giovanni-Chipuli/Churn_Clasif_Despliegue/main/Archivos/Portada_Churn_Clasif.JPG)

Con dicho modelo se procede a predecir la fuga de los cleintes, según nueva data:

![Portada_Churn_Clasif2](https://raw.githubusercontent.com/Giovanni-Chipuli/Churn_Clasif_Despliegue/main/Archivos/Portada_Churn_Clasif2.JPG)
