# Reconocimiento-Facial
## Reconocimiento Facial con el uso de Python TensorFlow, Keras, OpenCV y una base de datos propia.

# Contenido
1. Data_Collection
2. Modelo2
3. Prueba_de_Modelo
4. Notas


## [Data_Collection](https://github.com/X4ndre/Reconocimiento-Facial/blob/main/Data_Collection.ipynb)
Para realizar el proyecto primero se necesita crear una base de datos con imagenes de rostros. El cuaderno usa OpenCv para hacer uso de la camara y con esta tomar y guardar las fotos de forma consecutiva. Para que este funcione primero hay que asegurarse que la ruta donde se guardan las fotos existan, ejemplo: file_name_path = './Data/Train/sebastian/sebastian' + str(count) + '.jpg', significa que debe de existir en la ruta actual una carpeta llamada Data, dentro de Data Train, y dentro de Train una carpeta llamada sebastian, lo mismo en caso de test. El cuaderno usa OpenCv para tomar las fotos desde la camara en la que se esta ejecutando el codigo por lo que se recomienda usar un entorno local para que se pueda activar la camara, ya que software como Collaboratory no permiten el acceso a la camara.

## [Modelo2](https://github.com/X4ndre/Reconocimiento-Facial/blob/main/Modelo2.ipynb)
Para entrenar el modelo se usa el cuaderno llamado "Modelo2.ipynb" en este mientras se tenga una base de datos propia que contenga datos en train y test con el mismo nuemro de clases y datos en ambas se puede ejecutar, aunque tambien se tendra que cambiar las rutas de acceso a la base de datos donde se requiera ("train_datagen.flow_from_directory('Data/Train',", "test_data = test_datagen.flow_from_directory('Data/Test',", y "folders = glob('Data/Test/*')")

## [Prueba_de_Modelo](https://github.com/X4ndre/Reconocimiento-Facial/blob/main/Prueba_de_Modelo.ipynb)<a name="prueba_de_modelo"></a>
Para probar de forma local se usa el cuaderno "Prueba_de_Modelo.ipynb" de igual forma que el primer cuaderno las recomendaciones son ejecutarlo en un entorno local, y cambiar las rutas de acceso en la base de datos.

## Notas
Para que los cuadernos "Data_Collection" y Prueba_de_Modelo puedan funcionar se necesita de un procesro harcascade el cual fue obtenido en del siguiente link (https://github.com/anaustinbeing/haar-cascade-files)

