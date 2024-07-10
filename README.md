#Detección de defectos en papas tipo hojuelas (chips) por visión artificial

##Descripción

Este repositorio contiene los scrips que se desarrollaron para abordar el problema:“Detección de defectos en papas tipo hojuelas (chips) por visión artificial”. El proyecto se encuentra estructurado en 6 secciones:
- Adquisición de dataset
- Procesamiento y segmentación de la ROI
- Modelo U-Net 2 – segmentación total de chips
- Clasificador CNN
- Modelo U-Net 2 – segmentación del área defectuosa
- Proceso General

Los modelos U-Net y CNN se han entrenado en Colab; sin embargo, las pruebas de validación han sido compiladas y ejecutadas en un entorno local.

**Tabla de contenidos**

[TOCM]

[TOC]
#Preparación del entorno virtual
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

#Adquisición de dataset
- El dataset que ha servido para el proceso de entrenamiento se encuentra en un repositorio denominado Kaggle: [Link](https://www.kaggle.com/datasets/concaption/pepsico-lab-potato-quality-control)



#Procesamiento y segmentación de la ROI

##Modelo U-Net 1 – segmentación total de chips

# Clasificador CNN
# Método por conteo de píxeles
## Modelo U-Net 2 – segmentación del área defectuosa

# Proceso general
