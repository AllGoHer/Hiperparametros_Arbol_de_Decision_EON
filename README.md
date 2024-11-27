# Optimización de Conversión de Leads
En este proceso lo que se busca es obtener el mejor parametro y mejor precisión de modelo para la conversión de Leads de la Escuela Online de Negocio

## Procesos

### Árbol de Decisión

1. División entre características (independientes) y variable objetivo (dependiente)
   
2. Aplicamos SMOTE para equilibrar las clases
3. Dividir los datos en conjuntos de entrenamiento y prueba
4. Hacer el escalado de datos con MinMaxScaler
5. Ajustar el escalador a los datos de entrenamiento y transformarlos
6. Transformar los datos de evaluación

### Creación y Visualización del Árbol de Clasificación

1. Crear el objeto del modelo de árbol de decisión con un estado aleatorio fijo para reproducibilidad.
2. Entrenar el modelo con los conjuntos de entrenamiento.
3. Generar la visualización del árbol.
4. Simplificar el árbol estableciendo un 'max_depth' razonable.
5. Visualizar el árbol simplificado.
6. Primeros resultados

### Poda de Árbol

1. Creamos varios árboles, generemos una función que tome como parámetro el nombre del árbol y lo grafique

### Poda con min_samples_leaf

1. Creamos la instancia DecisionTreeClassifier.
2. Hacemos el fit del modelo con los datos de entrenamiento.
3. Graficamos.
4. podaremos más restringiendo el número de hojas.

### Poda con ccp_alpha

1. Poda con ccp_alpha de 0.005 para mayor crecimiento antes de la poda.
2. Poda con ccp_alpha de 0.010 para equilibro de manera optima del modelo.

### Calculo del Área Bajo la Curva para el modelo (AUC)

1. Estimamos los AUC para los diferentes modelos de árboles de clasificación.

### Hiperparámetros y Cuadrícula de Búsqueda

1. Definir el modelo base de árbol de decisión.
2. Establecer los parámetros para la búsqueda en cuadrícula
3. Crear el objeto GridSearchCV.
4. Ejecutar la búsqueda en cuadrícula con los datos de entrenamiento.
5. Busqueda de los mejores parámetros encontrados.
6. Busqueda del Mejor modelo encontrado.
7. Asignamos los mejores parámetros al modelo.
8. Entrenamos el modelo con los datos de entrenamiento.
9. Realizamos predicciones sobre el conjunto de evaluación.
10. Calculamos el AUC utilizando los datos de evaluación.
11. Optimización del Modelo con Búsqueda en Cuadrícula con Hiperparámetros

### Random Forest

1. Crear el modelo de Random Forest.
2. Entrenar el modelo con los datos de entrenamiento.
3. Hacer predicciones en el conjunto de evaluación.
4. Calcular la Precisión (Accuracy).
5. Calcular AUC.

### Gradient Boosting

1. creamos el modelo de Gradient Boosting.
2. Entrenamos el modelo con los datos de entrenamiento.
3. hacemos predicciones sobre el conjunto de evaluación.
4. Calculamos la Precisión (Accuracy), que nos indica qué porcentaje de nuestras predicciones son correctas.
5. calculamos el AUC, que nos da una idea de la capacidad del modelo para distinguir entre clases.

### Optimización de Hiperparámetros con GridSearchCV y ChatGPT

1. Definimos el modelo base de Gradient Boosting.
2. Establecemos un rango más amplio y detallado de hiperparámetros para la búsqueda en cuadrícula.
3. Crear el objeto GridSearchCV para realizar la búsqueda en cuadrícula.
4. Ejecutar la búsqueda en cuadrícula con los datos de entrenamiento.
5. Obtener los mejores parámetros y el mejor modelo.
6. Entrenar y evaluar el modelo optimizado.
7. Resultados Finales.


   


   

   
   
