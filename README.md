# OpenCV: Colorización de imágenes en blanco y negro 

**Estudiantes:**
  - Tyron Fonseca B83007
  - Roberto Méndez B94788

Proyecto de tema de investigación para el curso de CI-0163 Análisis de Grandes Volúmenes de Datos, basado en el blog [Colorizing b/w photos with neural networks](https://blog.floydhub.com/colorizing-b-w-photos-with-neural-networks/) y el artículo [Colorful Image Colorization](https://arxiv.org/abs/1603.08511).

---
## Prerequisitos
Se recomienda utilizar [Anaconda](https://www.anaconda.com/) para crear un entorno virtual en el que se instalen los módulos necesarios para ejecutar los cuadernos.
Los módulos principales necesarios son:
- Tensorflow
- OpenCV
- Numpy

Puede crear un entorno en Anaconda y activarlo ejecutando:
```
conda env create -n open-cv --file environment.yml
conda activate
```

## Archivos

*Dataset para entrenamiento*: se utilizó un dataset de 10800 imágenes que se encuentra alojado en Kaggle en este [enlace](https://www.kaggle.com/datasets/mariomatos/image-colorization).

`alpha_version.ipynb`: notebook con la primer versión creada a modo de prueba y exploración con la colorización y guardado de modelos.

`beta_version.ipynb`: versión más organizada en funciones del alpha_version y usando solo una imagen para entrenar y probar.

`colorization-opencv-v2.ipynb`: versión final del proyecto, organizado con funciones de liberación de memoria y carga de imágenes desde un directorio. Modelo entrenado con 5 mil imágenes.

`/models`: contiene los modelos entrenados de la versión final.

`/input`: contiene algunas imágenes de prueba.

`/output`: contiene las imágenes predichas por el modelo de la versión final.

## Ejecución

Puede ejecutar y editar el notebook `colorization-opencv-v2` haciendo fork desde la página de Kaggle en este [enlace](https://www.kaggle.com/betocr/colorization-with-opencv).

> Puede activar el GPU accelator para obtener resultados en un menor tiempo.


## Referencias consultadas
- [Understanding convolutions for deep learning](https://towardsdatascience.com/intuitively-understanding-convolutions-for-deep-learning-1f6f42faee1)
- [Colorizing b/w photos with neural networks](https://blog.floydhub.com/colorizing-b-w-photos-with-neural-networks/)
- [Color conversions](https://docs.opencv.org/3.4/de/d25/imgproc_color_conversions.html)
- [Colorful Image Colorization](https://arxiv.org/abs/1603.08511) 
