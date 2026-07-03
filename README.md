                    L I M A R E N T A
    Predictive Analytics para el Mercado de Alquileres en Lima
    ==========================================================
    
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


ESTRUCTURA DEL PROYECTO
-----------------------

lima-rent-predictive/
├── README.md                    # Este archivo
├── data/
│   └── dataset_clean.csv        # Dataset procesado y limpio
├── notebooks/
│   ├── 01_ETL_PySpark.ipynb     # ETL con PySpark
│   └── 02_Modelo_ML.ipynb       # Modelo Random Forest
├── models/
│   ├── modelo_random_forest.pkl # Modelo entrenado
│   └── features_used.txt        # Caracteristicas utilizadas
├── dashboards/
│   └── lima_rent_dashboard.pbix # Dashboard Power BI
├── screenshots/
│   ├── dashboard_final.png      # Captura del dashboard
│   ├── modelo_resultados.png    # Resultados del modelo
│   ├── feature_importance.png   # Importancia de variables
│   ├── neo4j_database_info.png  # Vista general de Neo4j
│   ├── neo4j_top_distritos.png  # Demanda por distrito
│   ├── neo4j_top_publicadores.png # Top publicadores
│   └── neo4j_precios_zona.png   # Precios por zona
└── docs/
    └── informe_ejecutivo.pdf    # Informe final (4 paginas)


ARQUITECTURA TECNICA
--------------------

  ┌─────────────────────────────────────────────────────────────┐
  │                    Google Colab (PySpark)                   │
  │  ┌─────────────┐   ┌──────────────┐   ┌──────────────┐      │
  │  │  ETL        │──▶│  ML Model    │──▶│   Neo4j Graf │      │
  │  │  Limpieza   │   │  RandomForest│   │   Centralidad│      │
  │  └─────────────┘   └──────────────┘   └──────────────┘      │
  └─────────────────────────────────────────────────────────────┘
                            │
                            ▼
  ┌─────────────────────────────────────────────────────────────┐
  │                    Power BI Desktop                         │
  │  ┌─────────────┐   ┌──────────────┐   ┌──────────────┐      │
  │  │  Mapa x     │   │  KPIs de     │   │  Tabla Top   │      │
  │  │  Distrito   │   │  Precios     │   │  10 Prop.    │      │
  │  └─────────────┘   └──────────────┘   └──────────────┘      │
  └─────────────────────────────────────────────────────────────┘


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
  Video Demo     : [Enlace a Loom]
  Informe        : docs/informe_ejecutivo.pdf


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
