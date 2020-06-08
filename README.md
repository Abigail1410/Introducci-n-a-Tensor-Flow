# Introducci-n-a-Tensor-Flow
Machine Learning con Tensor Flow
MACHINE LEARNING
En una máxima simplificación del proceso para aplicar ML podríamos decir que consiste en tomar un conjunto de datos
PREPARACIÓN DE LOS DATOS
Estas son algunas de las técnicas que se emplean para la limpieza y preparación del set de datos seleccionado:
•	Representación de las variables en distintas gráficas. 
•	Detección de valores nulos. 
•	Reducción del número de variables. 
•	Regularización.
•	Crear variables nuevas a partir de los datos. 
ELECCIÓN DEL MODELO
Principalmente existen tres tipos de algoritmos de Machine Learning:
•	Aprendizaje supervisado: 
•	Aprendizaje no supervisado: 
Aprendizaje por refuerzo: 
COMPROBACIÓN DEL RESULTADO
Análisis del resultado (análisis de errores) y estudiar cómo de buenas o malas han sido las predicciones o los resultados del modelo empleado.
#HERRAMIENTAS PARA COMENZAR
El lenguaje que se escoja sea Python, estas son algunas de las librerías más útiles que serán de gran ayuda: Numpy, Pandas, Matplotlib, Seaborn, TensorFlow, NLTK, Sklearn…
Introducción a TensorFlow
Un tensor es un conjunto de datos primitivos en un arreglo multidimensional, clasificado por número de dimensiones.(PHOTO)
 0: 5.0
[5.0, 10.0, 15.0, 20.0, 25.0]
[[5.0, 10.0], [15.0, 20.0], [25.0, 30.0]]
En los programas de TensorFlow, necesita de variables para almacenar las variables en memoria
1	import tensorflow as tf
 
firstnumber = tf.constant([10, 20, 30, 40, 50])
secondnumber = tf.Variable(firstnumber + 50)
 
with tf.Session() as session:
    session.run(tf.global_variables_initializer())
    print(session.run(secondnumber))
    
El API está bien documentado y bien diseñado
#TRES CAPAS DE LA ARQUITECTURA DE TENSORFLOW
1.	Librerías de alto nivel: Python, TensorBoard, Java y más1. Librerías de alto nivel: Python, TensorBoard, Java y más
2.	Núcleo de TensorFlow: Red neuronal de operaciones, motor de ejecución gráfica y más.
3.	Plataformas: CPUs, GPUs, TPUs, Android y iOS a través de los principales sistemas operativos.

16	import tensorflow as tf
 
five = tf.constant("00")
tf.Variable(0, name="variablename")
session = tf.Session()
 
file_writer = tf.summary.FileWriter('tflogs', session.graph)
 
run_options = tf.RunOptions(trace_level = tf.RunOptions.FULL_TRACE)
run_metadata = tf.RunMetadata()
 
summary, result = session.run(fetches=five, feed_dict=None, options=run_options, run_metadata=run_metadata)
print('Value %s' %result)
 
file_writer.add_run_metadata(run_metadata, 'result %s' %result)
session.close()
Pueden ejecutarse en un tiempo razonable gracias a las computadoras de más poder, GPUs y computación elástica en la nube
#CASOS DE USO
1.-Reconocimiento del lenguaje
2.-Reconocimiento de imagen
3.-Análisis sentimental
4.-Procesamiento de imágenes y vídeos móviles
5.-Traducción del lenguaje
6.-Chatbot
7.-Detección de cáncer







