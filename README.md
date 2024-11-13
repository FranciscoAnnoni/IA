# Reconocimiento de Caracteres Coreanos

Este proyecto utiliza aprendizaje automático para reconocer caracteres del alfabeto coreano (Hangul) a partir de imágenes. El modelo está basado en una red neuronal convolucional (CNN) entrenada con un conjunto de datos de imágenes de caracteres coreanos.

## Descripción

La aplicación fue desarrollada en Google Colab y tiene como objetivo entrenar un modelo de clasificación para reconocer caracteres coreanos. Utilizando la biblioteca TensorFlow y un enfoque de red neuronal convolucional, el modelo procesa imágenes de 250x250 píxeles, las cuales son previamente convertidas a escala de grises para mejorar la precisión del modelo.

## Tecnologías utilizadas

- **TensorFlow**: Para construir y entrenar el modelo de clasificación basado en CNN.
- **OpenCV**: Para la manipulación de imágenes (carga, cambio de tamaño y preprocesamiento).
- **Matplotlib**: Para visualizar algunas de las imágenes durante el entrenamiento.
- **NumPy**: Para el manejo eficiente de datos numéricos en el preprocesamiento.

## Datos

El modelo fue entrenado utilizando un conjunto de datos que contiene imágenes de caracteres coreanos. Las imágenes fueron divididas en conjuntos de entrenamiento y validación, con 8938 imágenes para el entrenamiento y 2234 imágenes para la validación.

## Flujo del proyecto

1. **Carga de datos**: Se cargan las imágenes y se etiquetan para el entrenamiento del modelo.
2. **Preprocesamiento de imágenes**: Las imágenes se convierten a escala de grises y se redimensionan a 250x250 píxeles para ser procesadas por el modelo.
3. **Entrenamiento del modelo**: Se construye y entrena una red neuronal convolucional (CNN) con varias capas convolucionales, capas de max pooling, y una capa de dropout para evitar el sobreajuste.
4. **Evaluación**: Después del entrenamiento, el modelo alcanza una precisión cercana al 100% en el conjunto de validación.
5. **Predicción**: El modelo entrenado es utilizado para predecir la clase de nuevos caracteres coreanos proporcionados en imágenes.
