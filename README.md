# Detección de defectos en papas tipo hojuelas (chips) por visión artificial
![](https://github.com/Sniper202/Detecccion-de-defectos-en-chips-de-papa/blob/main/img/img_originales.png)
## Descripción

Este repositorio contiene los scrips que se desarrollaron para abordar el problema:“Detección de defectos en papas tipo hojuelas (chips) por visión artificial”. El proyecto se encuentra estructurado en 6 secciones:
- Adquisición de dataset
- Procesamiento y segmentación de la ROI
- Modelo U-Net 2 – segmentación total de chips
- Clasificador CNN
- Modelo U-Net 2 – segmentación del área defectuosa
- Proceso General

Los modelos U-Net y CNN se han entrenado en Colab; sin embargo, las pruebas de validación han sido compiladas y ejecutadas en un entorno local.

# Preparación del entorno virtual
Se ha preparado un entorno virtual utilizando una interfaz gráfica de usuario, denominada como Anaconda Navigator, python 3.9.16  y jupyter notebook. Las librerías necesarias son:
- matplotlib
- keras 2.15.0
- opencv-python
- torch 1.12.1 +cud113
- torchvision 0.13.1 + cud113
- Pillow
- pandas
- scikit-learn 1.2.2
- tensorflow 2.15.0

# Adquisición de dataset
- El dataset utilizado para el proceso de entrenamiento se encuentra en un repositorio denominado Kaggle: [Link](https://www.kaggle.com/datasets/concaption/pepsico-lab-potato-quality-control) 

# Procesamiento y segmentación de la ROI
- Tener en cuenta que para replicar cualquiera de los modelos, se sugiere leer el siguiente documento:
## Modelo U-Net 1 – segmentación total de chips
- Es necesario poseer un conjunto de imágenes con sus respectivas máscaras binarias
- Para el desarrollo del modelo U-Net, se toma como referencia el repositorio de [Link](https://github.com/JACantoral/DL_fundamentals/blob/main/Fundamentals_DL_UNET_4_video_FP16_v2.ipynb)
- Los directorios: Generador de máscaras binarias y Modelo U-Net 1 contiene los archivos con los códigos para la creación del conjunto de entrenamiento y desarrollo del modelo. 
# Clasificador CNN
- Para empezar con el entrenamiento, es necesario cargar el modelo entrenado: MODELO3_29_01_24.pt
- El directorio CNN contiene el archivo con el código necesario para desarrollar el modelo CNN
# Método por conteo de píxeles
## Modelo U-Net 2 – segmentación del área defectuosa
- Para replicar este modelo,es necesario poseer un conjunto de imágenes con sus respectivas máscaras binarias.
- Los archivos necesarios se encuentran disponibles en el directorio: Modelo U-Net 2.
# Proceso general
- Para compilar y ejecutar el archivo, es necesario cargar los siguientes modelos: MODELO3_29_01_24.pt, UNETDEFECTV_2_new.pt, modeloCNNUNET.h5
- nota: el archivo del modelo CNN entrenado se encuentra disponible en: 
