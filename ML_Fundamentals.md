 # Fundamentos de Machine Learning
Despues de los primeros pasos, podemos empezar a entender el problema del machine learning. Ahora daremos unas descripciones de los problemas que podemos resolver con machine learning.
## Cuatro ramas del machine learning
Tareas como la clasificación binaria, la clasificación multiclase, la regresión y la análisis de sentimiento, son instancias del _aprendizaje supervisado_, en el cuál la meta es predecir un valor para una variable dependiente de una variable independiente. Los algoritmos de Machine learing caen dentro de cuatro categorías, descritas a continuación: 
### **Aprendizaje supervisado**
Consiste en una tarea de aprendizaje que se realiza sobre un conjunto de datos de entrenamiento, y que se evalúa con un conjunto de datos de prueba. En este se mapean unos datos de entrada, contra unos de salida llamados _Labels_ o _Target_. La mayor parte de los algoritmos de Machine Learning son de este tipo, tales como el reconocimiento de caracteres, reconocimiento de voz, clasificación de imágenes y regresión.
<center>
<img src="figs/SupervisedLearning.png" alt="alt text" title="image Title" width="600"/>

<p> Aprendizaje supervisado. Imagen: braintobytes.com </p>
</center>

### **Aprendizaje no supervisado**
Esta rama del machine learning consiste en encontrar transformaciones interesantes en los datos sin la ayuda de _targets_, principalemnte para propósitos de visualización, compresión de datos, o limpieza de datos. El aprendizaje no supervisado es una de los pilares el análisis de datos. La reducción de dimensionalidad y el _clustering_ son dos categorías del aprendizaje no supervisado. 
<center>
<img src="figs/clustering.png" alt="alt text" title="image Title" width="600"/>

<p> Ejemplo de clustering basado en similaridades. Imagen: blogs.sas.com</p>
</center>

### **Aprendizaje autosupervisado**
Esta es una instancia específica del aprendizaje supervisado, pero es tan diferente qeu merece su propia categoría. EL aprendizaje autosupervisado crea sus propios targets en el proceso sin la ayuda de etiquetas creadas a mano, algo así como aprendizaje sin humanos envueltos en el proceso. Las etiquetas son creadas desde los datos de entrada, tipicamente utilizando un algoritmo heurístico. Un ejemplo de esto son los sistemas para predicción de el siguiente texto en una oración dados los pasos anteriores, o la predicción del siguiente cuadro de un vídeo dados los cuadros anteriores.
<center>
<img src="figs/kt-step-3.png" alt="alt text" title="image Title" width="600"/>

<p> Ejemplo de autoetiquetado basado en clusters. Imagen: amitness.com </p>
</center>

### **Aprendizaje reforzado**
En el aprendizaje reforzado un _agente_ recibe información de su entorno y aprende a tomar decisiones que meximicen alguna recompensa. Por ejemplo, una red neuronal que con base en la información obtenida de la pantalla de un video juego, pueda producir acciones para el jugador que permita maximizar el puntaje del juego. Uno de los ejemplos más relevantes en este campo fue el modelo AlphaGo de Deepmind, el cuál derrotó al campeón mundial de Go en un juego.
<center>
<img src="figs/AlphaGo.jpeg" alt="alt text" title="image Title" width="500"/>

<p> Encuentro entre Lee Sedol y AlphaGo. Imagen: pureactu.com </p>
</center>


## Glosario de términos en Machine Learning
La clasificación y regresión involucran muchos términos especializados. Estos términos tienen definiciones relevantes para el aprendizaje de machine learning.

- **_Sample_(muestra) o _input_**  : Una dato que entra al modelo.
- **_Predicción_ o _salida_**: La salida del modelo.
- **_Target_ (objetivo)** - La verdad: Lo que el modelo debe predecir de manera ideal de acuerdo con los datos externos.
- **_loss value_ (_Error de predicción_)** : Una medida de la distancia entre la predicción hecha por el modelo y el target (objetivo).
- **Clases:** Un conjunto posible de etiquetas para escoger en un problema de clasificación. Por ejemplo si clasificamos gatos y perros, "gato" y "perro" serían las dos clases.
-  **Label (etiqueta)**: Es una instancia de la clase. Por ejemplo, si una imagen image.jpg pertenece a la clase "perro", el Label o etiqueta de esta imagen es "perro". 
-  **_Ground truth_ o _Annotations_**: Es el conjunto de todas las etiquetas en un conjunto de datos, normalmente creada por humanos.
-  **_Clasificación binaria_**: Es una tarea de clasificación donde cada muestra de entrada se clasifica en dos categorías. 
- **_Clasificación multiclase_**: Una tarea de clasificación en donde una muestra esta categorizada en mas de dos clases. Un ejemplo de esto es un programa que clasifique los numeros del 0 al 9, para este caso cada numero pertenece a una de las 10 clases (0 al 9).
- **_Regresión escalar_**: Una tarea de clasificación donde el target es un valor escalar continuo. Por ejemplo una regresión lineal en el cuál se busca encontrar los parámetros _m_ y _b_ de una recta a partir de los puntos _x_ y _y_, con el fin de predecir el valor que se obtendría para un nuevo _y_
   $$y=mx+b$$
- **_Mini-batch o batch_**: Es un pequeño conjunto de muestras o samples que son procesados de manera simultamena por el modelo. Este número es tipicamente entre 8 y 128. El número de samples es a menudo una potencia de 2, para facilitar la localización en la GPU. En la fase de entrenamiento, el minibatch es usado para calcular una actualicación simple del gradiente descendiente aplicacdo a los pesos del modelo.




