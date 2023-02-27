#Red_Neuronal_Artificial_Banca

# Finalidad
Este proyecto tiene como finalidad la construcción de una red neuronal artificial para predecir la probabilidad de que un cliente abandone al banco.

# Entrada
La entrada es un dataset en formato .csv que contiene los datos de 10.000 clientes cuya columna target llamada exited nos devuelve 1 si el cliente abandona el banco y 0 si se queda.

# Parámetros
Los parámetros utilizados en la lectura del fichero se encuentran en el archivo "prm_Red_Neuronal_Artificial_Banca".

# Red Neuronal
Para la construcción de la Red Neuronal Artificial se utilizó Tensorflow. La capa de entrada fue configurada con una distribución uniforme de pesos y la función de activación "relu" (rectificador lineal unitario). Los parámetros de la capa anterior se mantuvieron en la segunda capa oculta. Para la capa de salida se usó la función de activación sigmoide para mostrar la probabilidad de que un cliente abandone el banco. Seguido de cada capa se coloca un "dropout" del 10% para evitar el sobreajuste.

La compilación se realizó con el optimizador "rmsprop", la función de pérdidas elegida es "binary_crossentropy" para minimizar el error y la métrica "accuracy" para medir el porcentaje de precisión. Durante el entrenamiento se utilizó un "batch_size" de 32 para actualizar los pesos después de cada iteración. Se llevaron a cabo 150 épocas.

# Resultados
Se obtuvo una precisión del 83,1% con los parámetros escogidos.
Se obtuvo una precisión del 83,4% con la validación cruzada.

A los resultados obtenidos se le aplica un umbral, resultando así en únicamente dos resultados, "True" para los que tiene más de un 50% de probabilidades de abandonar el banco y "False" para los que tienen menos del 50%.

Se realiza una prueba con los datos de un cliente que no figura en el dataset de entrada para comprobar la eficacia de la RNA y proporciona una probabilidad del 9% de abandonar el banco.

# Observaciones
Se proporciona el código necesario para elaborar un "GridSearchCV" con la finalidad de encontrar los parámetros que maximicen la precisión. Debido a los altos costes de tiempo y de consumo computacional este paso no se ha realizado.

# Responsable técnico
Samuel Marcos Fernández
