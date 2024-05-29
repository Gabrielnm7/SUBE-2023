
# Análisis del Uso de la Tarjeta SUBE en Argentina: Tendencias y Comportamientos en 2023

<img src="./_src/sube.webp">

## Descripción del Proyecto

Este proyecto analiza los datos de uso de la tarjeta SUBE en Argentina durante el año 2023. La tarjeta SUBE es un sistema de pago utilizado en el transporte público en varias regiones del país. El análisis incluye la visualización de datos, un análisis exploratorio para identificar patrones en el uso del transporte público y la creación de modelos de regresión.

## Estructura del Proyecto

El proyecto está dividido en las siguientes secciones, todas en el archivo [sube](./sube.ipynb):

1. **Procesamiento de Datos**
2. **Análisis Exploratorio**
3. **Modelado**

## Instalación

Este proyecto se puede ver sin instalar nada, pero en caso de querer ejecutar el jupyter notebook por tu cuenta, necesitas tener instalado Python y las bibliotecas presentes en el archivo [requirements.txt](./requirements.txt)

Puedes instalar todas las dependencias en tu entorno virtual de esta manera:
```bash
pip install -r requirements.txt
```
En caso de no saber como instalar un entorno virtual, podes hacer [click aca](https://github.com/Gabrielnm7/How-to-create-a-virtual-enviroment/tree/main/ES%20-%20version) y te muestro paso a paso como. 

## Procesamiento de Datos

En esta sección se carga y limpia el dataset. Se transforman columnas a formatos adecuados y se agregan nuevas columnas para facilitar el análisis. Los datos son extraidos de la [secretaria de transporte](https://datos.transporte.gob.ar/dataset/sube-cantidad-de-transacciones-usos-por-fecha).

## Análisis Exploratorio

En esta sección se visualizan y analizan los datos utilizando herramientas de visualización como `seaborn` y `matplotlib`. El objetivo es identificar patrones en el uso del transporte público.

Por ejemplo, se analiza el uso de la tarjeta SUBE a lo largo del año para determinar los periodos de mayor y menor utilización y las razones detrás de estas variaciones. También se investiga cuáles son las empresas de transporte más utilizadas por los argentinos y se examinan las diferencias en el uso del transporte público entre distintas provincias, explorando las causas de una mayor utilización en ciertas regiones. Todo el análisis detallado se encuentra en el Jupyter Notebook


## Modelado

En esta sección se crean y validan modelos de regresión para predecir la cantidad de pasajeros utilizando la información de hasta otras 5 líneas de colectivos, con el objetivo de predecir específicamente la línea `BSAS_LINEA_009`. Los modelos desarrollados fueron los siguientes:

- Regresión Lineal con las 5 líneas aleatorias
- Ridge Regression con las 5 líneas más correlacionadas
- Regresión Lineal con la mejor combinación de 5 líneas en el top 35

Todo el analisis y testeo de estos modelos se pueden ver a detalle en el notebook


## Contribución

Las contribuciones son bienvenidas. Si deseas contribuir, por favor, abre un issue o envía un pull request. 

## Disclaimer
Este proyecto fue realizado para la materia Laboratorio de Datos de la carrera de Ciencia de Datos en la Universidad de Buenos Aires. 