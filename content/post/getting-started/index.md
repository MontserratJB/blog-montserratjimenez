---
authors:
- admin
categories:
- SIG
date: "2021-09-07T00:00:00Z"
draft: false
featured: false
image:
  caption: 'Image credit: [**Basesdedatos**](https://www.google.com/url?sa=i&url=https%3A%2F%2Fblog.krowdy.com%2Ftodo-para-tener-base-de-candidatos-perfecta&psig=AOvVaw279cjVDPVQGIcQo_bOkPdM&ust=1631142109011000&source=images&cd=vfe&ved=0CAsQjRxqFwoTCMDN3v_77fICFQAAAAAdAAAAABAD)'
  focal_point: ""
  placement: 2
  preview_only: false
lastmod: "2021-09-07T00:00:00Z"
projects: []
subtitle: "Comparación de extensión PostGIS y Software ArcSDE."
summary: "Comparación de extensión PostGIS y Software ArcSDE."
tags:
- Academic
title: Comparación de extensión PostGIS y Software ArcSDE
---

## Introducción

El almacenamiento, procesamiento y visualización de datos geoespaciales ha generado la necesidad de estructuras de bases de datos que permitan el manejo de esta información en un mismo repositorio, los modelos de bases de datos heterogéneos pueden presentar dificultades en el modelaje, uso e integración de los datos. Víquez, A. & Hernández, I. (2020). 
Algunas de las soluciones que se usan con más frecuencia en la actualidad para trabajar con datos geoespaciales son la extensión Postgis y el software producido por ESRI ArcSDE. 



## Conceptos Básicos

- 👉 **PostGis:**
 	“PostGIS es una extensión del sistema de base de datos PostgreSQL, que permite el almacenamiento y la manipulación de objetos geométricos vectoriales en bases de datos; incluyendo, además, el Sistema de Referencia Espacial; lo que la convierte en una base de datos espacial para su utilización en Sistema de Información Geográfica”. Duke-Williams, (2006).
- 👉 **PostgreSQL:**
 “PostgreSQL es un potente sistema de base de datos relacional de objetos de código abierto con más de 30 años de desarrollo activo que le ha ganado una sólida reputación por su fiabilidad, solidez de funciones y rendimiento.”  PostgreSQL (Accesado en: 2021).
- 👉 **ArcSDE:**
“Permite administrar datos geoespaciales dentro de la base de datos relacional, la tecnología admite la lectura y la escritura de varios estándares, entre ellos los estándares de OGC para entidades simples y estándares ISO para tipo espaciales” Ochoa (2015).
- 👉 **Datos espaciales:**
“Los datos espaciales representan digitalmente, elementos o fenómenos que suceden en la faz de la tierra o cerca de la misma. Dichos elementos se pueden modelizar mediante modelos de datos Vectoriales y modelos de datos Ráster; los datos vectoriales representan formas geométricas como puntos, líneas o polígonos (por ejemplo, una casa, una carretera, un bosque, respectivamente); y los datos Ráster se caracterizan por la presencia de celdas o cuadrículas, más conocidas como píxeles, en donde cada píxel muestra una cualidad espacial (color, altitud, etc.)”. Botella, Camps, & Muñoz (1989).
- 👉 **Base de datos espacial:**
“Una Base de Datos Espacial permite describir los objetos espaciales que la forman a través de tres características básicas: atributos, localización y topología. Los atributos representan características de los objetos que nos permiten saber qué es lo que son. La localización, representada por la geometría del objeto y su ubicación espacial de acuerdo a un sistema de referencia, permite saber dónde está el objeto y qué espacio ocupa”. Gutiérrez (2006).


## Comparación

Dentro del trabajo que se realiza para la creación de una base de datos espacial se considera el modelamiento de la base de datos de acuerdo a los requerimientos del sistema.
Al trabajar con el modelo físico se debe integrar a la base de datos nueva todas las condiciones definidas previamente como tipos de datos y restricciones en columnas, tablas y relaciones entre tablas.
Esta integración del modelo físico a la base de datos puede variar al trabajar con una extensión PostGIS y con el Software ArcSDE.
Según Víquez, A. & Hernández, I. (2020), al trabajar con ArcSDE, se presentan deficiencias al transformar el modelo físico porque asignan automáticamente la llave primaria y las restricciones a valores codificados no son considerados por el motor de base de datos.
Al trabajar con la extensión PostGIS e incorporar un modelo físico generado desde PgModeler se mantienen llaves primarias establecidas en el modelo físico.



