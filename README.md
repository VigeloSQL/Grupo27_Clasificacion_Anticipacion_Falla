# Anticipación de Fallas en un Reactor Químico

Clasificación binaria para predecir si un reactor químico entrará en falla, usando DNN / LSTM / GRU sobre series de tiempo de proceso.

## Dataset

[Chemical Process Monitoring Time Series Dataset — Kaggle](https://www.kaggle.com/datasets/rohit8527kmr7518/chemical-process-monitoring-time-series-dataset/data?select=chemical_process_timeseries.csv)

6 reactores (`A_R1`…`B_R3`), 2 regímenes (base y estresado), muestreo de 1 min, ene–mar 2024 (~777 k filas).

## Estructura del experimento

- **Train**: `A_R1`, `A_R2`, `B_R1`, `B_R2`
- **Validación**: `A_R3`
- **Test**: `B_R3` (reactor no visto, mide generalización real)
