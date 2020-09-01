# Results on Metr&PEMS Datasets

## Results on METR



| <font color='red'>**Fitness: 15 mins**</font> | val-rmse | test-rmse |     Converged Time      |
| :-------------------------------------------: | :------: | :-------: | :---------------------: |
|                   HM`2-0-4`                   | 7.20075  |  8.93415  |                         |
|                   ARIMA(C)                    | 6.67445  |  7.02787  |                         |
|                    XGBoost                    |          |           |                         |
|               GBRT`11-8-2-29-4`               | 6.22460  |  6.37050  |                         |
|                ST_MGCN (G/DCI)                | 6.37587  |  6.64489  | 9.66 hour / 424 epochs  |
|                 DCRNN(G/D C)                  |          |           |                         |
|                   LSTM (C)                    | 5.36337  |  6.38015  | 9.21 hour / 8296 epochs |
|                TMeta-LSTM-GAL                 | 5.35551  |  6.15585  | 0.96 hour / 1113 epochs |
|               AMulti-GCLSTM-V1                | 5.40675  |  5.64445  | 2.68 hour / 3100 epochs |
|               AMulti-GCLSTM-V2                | 5.34392  |  5.79998  | 3.10 hour / 4265 epochs |
|               AMulti-GCLSTM-V3                | 5.42232  |  5.78807  | 1.00 hour / 1202 epochs |

| <font color='red'>**Fitness: 30 mins**</font> | val-rmse | test-rmse |      Converged Time      |
| :-------------------------------------------: | :------: | :-------: | :----------------------: |
|                   HM`2-0-4`                   | 7.71999  |  9.55981  |                          |
|                   ARIMA(C)                    | 8.03009  |  9.22951  |                          |
|                    XGBoost                    |          |           |                          |
|               GBRT`10-0-0-27-3`               | 7.12267  |  8.26941  |                          |
|                ST_MGCN (G/DCI)                | 8.34595  |  8.07924  |  5.33 hour / 452 epochs  |
|                 DCRNN(G/D C)                  |          |           |                          |
|                   LSTM (C)                    | 6.26720  |  7.86569  | 5.06 hour / 10071 epochs |
|                TMeta-LSTM-GAL                 | 6.27180  |  7.43553  | 0.78 hour / 1744 epochs  |
|               AMulti-GCLSTM-V1                | 6.57803  |  7.15628  | 1.84 hour / 3465 epochs  |
|               AMulti-GCLSTM-V2                | 6.10779  |  6.88889  | 4.79 hour / 10860 epochs |
|               AMulti-GCLSTM-V3                | 6.38780  |  7.18431  | 1.40 hour / 2571 epochs  |

| <font color='red'>**Fitness: 60 mins**</font> | val-rmse | test-rmse |      Converged Time      |
| :-------------------------------------------: | :------: | :-------: | :----------------------: |
|                   HM`2-1-4`                   | 9.85644  | 10.72724  |                          |
|                   ARIMA(C)                    | 10.73827 | 11.73901  |                          |
|                    XGBoost                    |          |           |                          |
|               GBRT`4-5-1-19-4`                | 9.03259  | 10.01320  |                          |
|                ST_MGCN (G/DCI)                | 10.40405 | 10.79813  | 6.64 hour / 1240 epochs  |
|                 DCRNN(G/D C)                  |          |           |                          |
|                   LSTM (C)                    | 7.24440  | 10.08317  | 1.57 hour / 1868 epochs  |
|                TMeta-LSTM-GAL                 | 5.65159  |  8.66965  | 1.19 hour / 12000 epochs |
|               AMulti-GCLSTM-V1                | 5.89982  |  8.83393  | 2.99 hour / 1779 epochs  |
|               AMulti-GCLSTM-V2                | 5.89793  |  9.14697  | 0.55 hour / 1590 epochs  |
|               AMulti-GCLSTM-V3                | 6.33248  |  8.99345  | 0.80 hour / 2387 epochs  |





## Results on PEMS-BAY

| <font color='red'>**Fitness: 15 mins**</font> | val-rmse | test-rmse |      Converged Time       |
| :-------------------------------------------: | :------: | :-------: | :-----------------------: |
|                   HM`1-0-1`                   | 3.38002  |  3.68983  |                           |
|                   ARIMA(C)                    | 2.95765  |  2.86893  |                           |
|                    XGBoost                    |          |           |                           |
|               GBRT`10-6-1-65-6`               | 2.54514  |  2.64524  |                           |
|                ST_MGCN (G/DCI)                |          |           |                           |
|                 DCRNN(G/D C)                  |          |           |                           |
|                   LSTM (C)                    | 5.15498  |  2.68953  | 13.92 hour / 13000 epochs |
|                TMeta-LSTM-GAL                 | 5.61040  |  2.54368  |  3.68 hour / 2297 epochs  |
|               AMulti-GCLSTM-V1                | 5.52864  |  2.43292  | 24.00 hour / 8584 epochs  |
|               AMulti-GCLSTM-V2                | 5.56845  |  2.44947  | 19.26 hour / 8562 epochs  |
|               AMulti-GCLSTM-V3                | 5.54370  |  2.44571  | 19.71 hour / 6608 epochs  |

| <font color='red'>**Fitness: 30 mins**</font> | val-rmse | test-rmse |      Converged Time      |
| :-------------------------------------------: | :------: | :-------: | :----------------------: |
|                   HM`1-0-1`                   | 3.77182  |  3.96537  |                          |
|                   ARIMA(C)                    | 4.20225  |  3.93569  |                          |
|                    XGBoost                    |          |           |                          |
|               GBRT`12-6-2-90-7`               | 3.19538  |  3.37025  |                          |
|                ST_MGCN (G/DCI)                |          |           |                          |
|                 DCRNN(G/D C)                  |          |           |                          |
|                   LSTM (C)                    | 5.96921  |  3.68256  | 7.48 hour / 13000 epochs |
|                TMeta-LSTM-GAL                 | 6.51965  |  3.23098  | 7.99 hour / 11116 epochs |
|               AMulti-GCLSTM-V1                | 6.44145  |  3.11554  | 8.34 hour / 5467 epochs  |
|               AMulti-GCLSTM-V2                | 6.53199  |  3.20407  | 4.44 hour / 3492 epochs  |
|               AMulti-GCLSTM-V3                | 6.49245  |  3.18722  | 3.08 hour / 1663 epochs  |

| <font color='red'>**Fitness: 60 mins**</font> | val-rmse | test-rmse |      Converged Time       |
| :-------------------------------------------: | :------: | :-------: | :-----------------------: |
|                   HM`1-1-4`                   | 3.86753  |  4.01788  |                           |
|                   ARIMA(C)                    | 6.15591  |  5.67008  |                           |
|                    XGBoost                    |          |           |                           |
|               GBRT`12-7-2-59-5`               | 3.40530  |  3.70401  |                           |
|                ST_MGCN (G/DCI)                |          |           |                           |
|                 DCRNN(G/D C)                  |          |           |                           |
|                   LSTM (C)                    | 6.95412  |  4.77696  | 7.53 hour / 10002 epochs  |
|                TMeta-LSTM-GAL                 | 6.68086  |  3.61642  | 15.45 hour / 13000 epochs |
|               AMulti-GCLSTM-V1                | 6.62233  |  3.51389  |  5.81 hour / 2372 epochs  |
|               AMulti-GCLSTM-V2                | 7.11932  |  3.55159  |  6.45 hour / 9357 epochs  |
|               AMulti-GCLSTM-V3                | 7.05142  |  3.49954  |  6.88 hour / 7573 epochs  |