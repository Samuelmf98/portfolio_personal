#Red_Neuronal_Artificial_Acciones_Google

# Finalidad
Este proyecto tiene como finalidad la construcción de una red neuronal artificial para predecir el precio de las acciones google para el primer mes de 2017.

# Entrada
La entrada es un dataset en formato .csv que contiene los datos del precio de apertura de las acciones desde 2012 hasta 2017.  
# Parámetros
Los parámetros utilizados en la lectura del fichero se encuentran en el archivo "prm_Red_Neuronal_Artificial_Acciones_Google".

# Red Neuronal
Para la construcción de la Red Neuronal Artificial se utilizó Tensorflow. La capa de entrada fue configurada con una distribución uniforme de pesos y la función de activación "relu" (rectificador lineal unitario). Los parámetros de la capa anterior se mantuvieron en la segunda capa oculta.  Seguido de cada capa se coloca un "dropout" del 10% para evitar el sobreajuste.

La compilación se realizó con el optimizador "adam", la función de pérdidas elegida es "mean_squared_error" para minimizar el error. Durante el entrenamiento se utilizó un "batch_size" de 32 para actualizar los pesos después de cada iteración. Se llevaron a cabo 100 épocas.

# Resultados
Se diseña una gráfica para comparar el resultado obtenido con el resultado real que hubo en 2017 y se
observa que la predicción se asemaja bastante al objetivo.
# Observaciones

# Responsable técnico
Samuel Marcos Fernández
