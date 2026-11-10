# Lab 9.3 – RNN y LSTM para caudales del río Mala (CAMELS-PE)

**Autora:** Betzy Camila Lopez Cerna – UTEC

Réplica de la **Práctica A** del Lab 9.3 (*Deep Learning II: RNN/LSTM*) con una cuenca nueva.
En clase se usó el río Majes (estación Huatiapa, `PE_204617`); aquí se usa el
**río Mala, estación La Capilla (`PE_212900`)**, con datos de **CAMELS-PE (SENAMHI)**.

## Contenido

| Archivo | Descripción |
|---|---|
| `Lab9_3_PracticaA_RioMala_LSTM.ipynb` | Notebook de Google Colab con A1 y A2 |
| `PE_212900_mala.csv` | Serie diaria de la cuenca (se genera al ejecutar el notebook) |

## Tareas

- **A1 · Simulación lluvia–escorrentía:** RNN simple vs. LSTM vs. modelo hidrológico del SENAMHI,
  usando solo 180 días de meteorología (prec, tmean, tmax, tmin, srad, vprp).
- **A2 · Pronóstico:** LSTM con asimilación del caudal observado a 1, 3 y 7 días, comparada con la persistencia.

Periodos: entrenamiento 1998–2010, validación 2011–2015, prueba 2016–2020. Métricas: NSE y KGE.

## Cómo ejecutar

1. Abrir el notebook en Google Colab.
2. `Entorno de ejecución → Ejecutar todo`. La primera celda de datos descarga CAMELS-PE v2.0 desde Zenodo
   y extrae solo el archivo de la cuenca `PE_212900`.

## Datos

Llauca, H., Montesinos-Caceres, C., Gutierrez-Reynaga, M., & Lavado-Casimiro, W. (2026).
*CAMELS-PE: Catchment Attributes and Meteorology for Large-sample Studies in Peru* [Data set]. Zenodo.
https://doi.org/10.5281/zenodo.20058778
