# PracticoN3-RedesNeuronales-AutoencoderFeedForward
## Objetivo del trabajo 
Predecir y replicar números del dataset MNIST

## ¿Qué es un auto-encoder?
El auto-encoder es un algoritmo de aprendizaje que permite el preprocesamiento de los datos con el objetivo que la red aprenda la función identidad, es decir que la entrada sea igual a la salida, tal que al realizar este preprocesamiento de los acoplamientos, y partiendo de una red que ha sido autoaprendida, el método del back propagation es más eficiente, eliminando el problema de la aleatoriedad de los pesos sinápticos iniciales y hace que la red sea mucho más lenta e ineficiente.


## Resumen del trabajo realizado
En nuestro caso, implementamos una red feed-forward auto-encoder con una capa oculta, pero puramente con la finalidad que aprenda la identidad, utilizando la base de datos MNIST de dígitos de número escritos a mano. En la primera instancia, nuestra red tiene 784 unidades de entrada, una capa oculta de 64 neuronas y obviamente una capa de salida de 784 neuronas. Utilizando como algoritmo de optimización al descenso por gradiente estocástico (SGD), trabajando con un valor del learning rate de 10 (se decide trabajar con este valor del parámetro de aprendizaje porque cuando se usa uno de los valores dado por el estado del arte de entre 10^(-1) y 10^(-4), la red es muy lenta para aprender), dándole un valor de 0,1 al parámetro de dropout, minitbatch de tamaño 1000.

## Conclusión
Se concluye que la red logra replicar de forma casi perfecta la imagen de entrada y predecir con un 95% de efectividad el número que se muestra en la imagen, es decir, se logran los objetivos buscados.
