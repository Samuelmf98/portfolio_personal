#Red_Neuronal_Convolucional_Perro_Gato

# Finalidad
Este proyecto tiene como finalidad la construcción de una red neuronal convolucional para clasificar imágenes de perros y de gatos.
# Entrada
La entrada son dos carpeta, formadas por 4.000 imágenes de perros y 4.000 imágemnes de gatos.

# Parámetros
Los parámetros utilizados en la lectura de las imágenes, tanto para train/test como para predecir, se encuentran en el archivo "prm_Red_Neuronal_Convolucional_Perro_Gato".

# Red Neuronal
Para la construcción de la Red Neuronal Convolucional se utilizó Tensorflow. La capa de entrada fue configurada con 32 mapas de características de 3x3. Seguidamente se agrega un "Max_Pooling" para calcular el máximo de los subconjuntos de pixeles. Para aplanar las imágenes en un vector se utiliza la capa de "Flattening" y posteriormente se crea una red neuronal artificial para la capa de fully connected con una función de activación "relu" (rectificador lineal unitario). Para la capa de salida se usó la función de activación sigmoide para mostrar la probabilidad de que una imagen sea clasificada como perro o como gato.

La compilación se realizó con el optimizador "rmsprop", la función de pérdidas elegida es "binary_crossentropy" para minimizar el error y la métrica "accuracy" para medir el porcentaje de precisión. Durante el entrenamiento se utilizó un "batch_size" de 32 para actualizar los pesos después de cada iteración. Se llevaron a cabo 25 épocas.

# Resultados
Se obtuvo una precisión del 81% con los parámetros escogidos.

Se realiza una prueba con imágenes aleatorias extraídas de internet para comprobar la eficacia de nuestro modelo de clasificación de imágenes de perros y gatos. A los resultados obtenidos se le aplica una etiqueta, resultando en 1 para perros y 0 para gatos. De 10 imágenes mostradas predice correctmente 8 y falla en 2.

# Observaciones


# Responsable técnico
Samuel Marcos Fernández