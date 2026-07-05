**LIMA RENTA**
Predictive Analytics para el Mercado de Alquileres en Lima
===========================================================

Proyecto Integrador - Big Data
Universidad Católica Sede Sapientiae
Facultad de Ingeniería - Ingeniería de Sistemas


DESCRIPCION DEL PROYECTO
------------------------

El mercado de alquiler de viviendas en Lima Metropolitana presenta
una alta variabilidad de precios sin informacion clara sobre los
factores determinantes. Este proyecto utiliza tecnicas de Big Data
para:

  1. Predecir el precio justo de alquiler de una propiedad
     basado en sus caracteristicas (Random Forest Regressor)

  2. Identificar distritos con mayor demanda y mejor relacion
     precio/area mediante analisis de grafos (Neo4j)

  3. Visualizar el mercado de alquiler a traves de un dashboard
     interactivo (Power BI)


HERRAMIENTAS UTILIZADAS
----------------------- 

  - Google Colab      : Entorno de desarrollo Python
  - PySpark           : Procesamiento distribuido y ETL
  - Pandas            : Manipulacion de datos
  - Scikit-learn      : Modelo Random Forest Regressor
  - Neo4j Aura        : Base de datos de grafos
  - Power BI Desktop  : Visualizacion interactiva
  - GitHub            : Control de versiones
  - Loom              : Video demo (3 min)


RESULTADOS CLAVE
----------------

  Modelo de Machine Learning (Random Forest)
  -----------------------------------------
   - R² Score              : 0.8234
   - MAE (Error Medio)     : S/. 245.67
   - RMSE                  : S/. 450.23
   - MAPE (Error %)        : 18.45%
   - Feature mas importante: Area (62.14%)

  Analisis de Grafos (Neo4j)
  --------------------------
   - Nodos totales         : 597
   - Distritos unicos       : 50
   - Publicadores unicos   : 200
   - Relaciones creadas    : 3 (UBICADA_EN, PERTENECE_A, PUBLICADA_POR)

  Dashboard Power BI
  ------------------
   - 3 KPIs (Total, Precio Promedio, Precio m2)
   - Top 10 Distritos por Precio Promedio
   - Propiedades por Zona
   - Mapa de Distribucion por Distrito
   - 4 Segmentaciones interactivas


STAKEHOLDERS
------------

  1. Inmobiliarias      : Para fijar precios competitivos
  2. Arrendadores       : Para conocer el valor real de su propiedad
  3. Arrendatarios      : Para encontrar mejores ofertas
  4. Equipo de TI       : Para implementacion y mantenimiento


PREGUNTA DE NEGOCIO
-------------------

   ¿Como reducir el porcentaje de propiedades con precios
   sobrevalorados en un 15% durante el proximo trimestre?


OBJETIVOS SMART
---------------

  1. Desarrollar un modelo predictivo con R² > 0.80
  2. Identificar distritos con mayor demanda
  3. Crear un dashboard ejecutivo interactivo
  4. Reducir el error de prediccion (MAE < S/. 300)


ENTREGABLES
-----------

  1. Enlace al repositorio GitHub (publico)
  2. Notebooks ejecutados en Google Colab
  3. Archivo .pbix del dashboard de Power BI
  4. Enlace al video demo (Loom)
  5. Informe ejecutivo en PDF (maximo 4 paginas)


ENLACES RAPIDOS
 ---------------

   Repositorio    : https://github.com/Soviet117/lima-rent-predictive
   Dashboard      : dashboards/lima_rent_dashboard.pbix
   Informe        : docs/informe_ejecutivo.pdf

 VIDEOS EXPLICATIVOS
 -------------------

   1. Planteamiento del Problema
      video1_problema.mp4
      https://drive.google.com/file/d/1e92oOH9uBJo0ROSF09dgAz-XDm6I4U7I/view?usp=sharing

   2. Arquitectura de la Solución
      video2_arquitectura.mp4
      https://drive.google.com/file/d/1KP4m0zHZS8FhqzUtIk9AkTE8wDQjTIAi/view?usp=sharing

   3. Demo del Dashboard y Modelo
      video3_demo.mp4
      https://drive.google.com/file/d/1c7j-STLmNf6aFk9XMl6EmF7O6iNKwmCy/view?usp=sharing

   4. Impacto y Conclusiones
      video4_impacto.mp4
      https://drive.google.com/file/d/1ZXtL1k2EULW5EFOlVXgZWtMedIReqkAt/view?usp=sharing


EQUIPO
------

  Product Owner  : Torres Quispe Adixon Jhair (Soviet)
  Data Engineer  : Torres Quispe Adixon Jhair (Soviet)
  Data Scientist : Torres Quispe Adixon Jhair (Soviet)
  BI Storyteller : Torres Quispe Adixon Jhair (Soviet)


DOCENTE
-------

  Ing. Jhon Alexander Zagaceta Daza


FECHA
-----

  2026-07-03


LICENCIA
--------

  Este proyecto es de uso academico.
