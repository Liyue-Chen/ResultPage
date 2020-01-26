# Results on Different Datasets(KDD)

## Results on Bike

| <font color='red'>**Fitness: 15 mins**</font> | NYC  | Chicago |  DC  |
| :-------------------------------------------: | :--: | :-----: | :--: |
|                      HM                       |      |         |      |
|                   ARIMA(C)                    |      |         |      |
|                    XGBoost                    |      |         |      |
|                     GBRT                      |      |         |      |
|                ST_MGCN (G/DCI)                |      |         |      |
|                 DCRNN(G/D C)                  |      |         |      |
|                   LSTM (C)                    |      |         |      |
|                TMeta-LSTM-GAL                 |      |         |      |
|               AMulti-GCLSTM-V1                |      |         |      |
|               AMulti-GCLSTM-V2                |      |         |      |
|               AMulti-GCLSTM-V3                |      |         |      |



| <font color='red'>**Fitness: 30 mins**</font> | NYC  | Chicago |  DC  |
| :-------------------------------------------: | :--: | :-----: | :--: |
|                      HM                       |      |         |      |
|                   ARIMA(C)                    |      |         |      |
|                    XGBoost                    |      |         |      |
|                     GBRT                      |      |         |      |
|                ST_MGCN (G/DCI)                |      |         |      |
|                 DCRNN(G/D C)                  |      |         |      |
|                   LSTM (C)                    |      |         |      |
|                TMeta-LSTM-GAL                 |      |         |      |
|               AMulti-GCLSTM-V1                |      |         |      |
|               AMulti-GCLSTM-V2                |      |         |      |
|               AMulti-GCLSTM-V3                |      |         |      |



| <font color='red'>**Fitness: 60 mins**</font> |          NYC           |         Chicago         |           DC            |
| :-------------------------------------------: | :--------------------: | :---------------------: | :---------------------: |
|                      HM                       |    3.99224 `1-1-3`     |     2.97693 `1-1-2`     |     2.63165 `2-1-3`     |
|                   ARIMA(C)                    |        5.60928         |         3.83584         |         3.60450         |
|                    XGBoost                    | 4.12407 `12-10-0-20-5` |  2.92569 `9-7-0-20-5`   | 2.65671 `12-14-2-20-5`  |
|                     GBRT                      | 3.99907 `12-7-4-100-5` | 2.84257 `12-14-2-100-5` | 2.61768 `12-14-2-100-5` |
|                ST_MGCN (G/DCI)                |        3.72380         |         2.88300         |         2.48560         |
|                 DCRNN(G/D C)                  |        4.18666         |         3.27759         |         3.08616         |
|                   LSTM (C)                    |                        |                         |                         |
|                TMeta-LSTM-GAL                 |                        |                         |                         |
|               AMulti-GCLSTM-V1                |                        |                         |                         |
|               AMulti-GCLSTM-V2                |                        |                         |                         |
|               AMulti-GCLSTM-V3                |                        |                         |                         |



## Results on DiDi

| <font color='red'>**City: Xi'an <br />Fitness: 15 mins**</font> |       Params       |      val-rmse      |     test-rmse      | # Params |      Converged Time      |
| :----------------------------------------------------------: | :----------------: | :----------------: | :----------------: | :------: | :----------------------: |
|                              HM                              |      `1-1-2`       |                    |                    |   ---    |           ---            |
|                           ARIMA(C)                           |         --         |                    |                    |    --    |            --            |
|                           XGBoost                            |   `12-0-2-10-5`    |                    |                    |   ---    |           ---            |
|                             GBRT                             |    `9-0-2-50-2`    |                    |                    |   ---    |           ---            |
|                          ST-ResNet                           |      `待补充`      |                    |                    | `待补充` |                          |
|                       ST_MGCN (G/DCI)                        |      `待补充`      |                    |                    |  248985  |                          |
|                        DCRNN (G/D C)                         |                    |                    |                    |  50368   |                          |
|                           LSTM(C)                            |   `1-64-32-2-64`   | 2.5833148788660765 | 3.051378064846481  |          | 6.01 hour / 8600 epochs  |
|                          TMeta(TM)                           |                    |     2.39822754     |  2.9171236653898   |          |   0.86 hour / 7 epochs   |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` |    2.4511483684    | 2.6531950443195034 |          | 24.12 hour / 7082 epochs |
|                   AMulti-GCLSTM-V2(G/DCI)                    | `1-1-1-64-32-2-64` | 2.359822215512395  | 2.636734795190405  |          | 8.34 hour / 2778 epochs  |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    | 2.4035983718931675 |  2.64848648673072  |          |  6.50 hour / 941 epochs  |



| <font color='#ff0000'>**City: Xi'an <br />Fitness: 30 mins**</font> |       Params       |      val-rmse      | test-rmse | # Params |      Converged Time       |
| :----------------------------------------------------------: | :----------------: | :----------------: | :-------: | :------: | :-----------------------: |
|                              HM                              |      `1-1-2`       |                    |           |   ---    |            ---            |
|                           ARIMA(C)                           |         --         |                    |           |    --    |            --             |
|                           XGBoost                            |   `12-0-2-10-5`    |                    |           |   ---    |            ---            |
|                             GBRT                             |    `9-0-2-50-2`    |                    |           |   ---    |            ---            |
|                          ST-ResNet                           |      `待补充`      |                    |           | `待补充` |                           |
|                       ST_MGCN (G/DCI)                        |      `待补充`      |                    |           |  248985  |                           |
|                        DCRNN (G/D C)                         |                    |                    |           |  50368   |                           |
|                           LSTM(C)                            |   `1-64-32-2-64`   |  4.4937057606875   | 4.9503675 |          | 10.37 hour / 39614 epochs |
|                            TMeta                             |                    | 4.101934153586626  | 3.8468966 |          | 5.25 hour / 10612 epochs  |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` | 4.000900061801076  | 3.808124  |          | 16.23 hour / 9331 epochs  |
|                   AMulti-GCLSTM-V2(G/DCI)                    | `1-1-1-64-32-2-64` | 4.113256735727191  | 3.7719011 |          |  9.07 hour / 6312 epochs  |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    | 4.0017965622246265 | 3.8327777 |          |  7.96 hour / 3184 epochs  |



| <font color='red'>**City: Xi'an <br />Fitness: 60mins**</font> |       Params       |     val-rmse      | test-rmse | # Params |      Converged Time      |
| :----------------------------------------------------------: | :----------------: | :---------------: | :-------: | :------: | :----------------------: |
|                              HM                              |     `1-1-2` ✅      |      6.82453      |  6.18623  |   ---    |           ---            |
|                           ARIMA(C)                           |         --         |      8.87565      |  9.47478  |    --    |            --            |
|                           XGBoost                            |   `12-0-2-10-5`✅   |      6.90805      |  6.73346  |   ---    |           ---            |
|                             GBRT                             |   `9-0-2-50-2`✅    |      6.95321      |  6.44639  |   ---    |           ---            |
|                          ST-ResNet                           |     ✅ `待补充`     |    **6.41107**    |  6.08476  | `待补充` |        0.55 hour         |
|                       ST_MGCN (G/DCI)                        |      `待补充`      |      7.51881      |  5.87456  |  248985  |   1.31 hour 300 epochs   |
|                        DCRNN (G/D C)                         |                    |      7.29442      |  8.20254  |  50368   | 2.10 hour / 10000 epochs |
|                           LSTM(C)                            |   `1-64-32-2-64`   |  9.8606210052967  | 9.829621  |          | 2.37 hour / 11776 epochs |
|                            TMeta                             |                    | 7.489513948559761 | 5.8426275 |          | 1.25 hour / 4265 epochs  |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` | 7.295302748680115 | 5.871044  |          | 6.64 hour / 6911 epochs  |
|                   AMulti-GCLSTM-V2(G/DCI)                    | `1-1-1-64-32-2-64` | 7.35794323682785  | 5.8289084 |          | 2.52 hour / 2956 epochs  |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    | 7.144264250993729 | 5.9081187 |          | 3.37 hour / 2393 epochs  |



## Results on Metro

| **<font color='#ff0000'>City: Chongqing <br />Fitness: 15mins</font>** |       Params       | val-rmse | test-rmse | # Params | Converged Time |
| :----------------------------------------------------------: | :----------------: | :------: | :-------: | :------: | :------------: |
|                              HM                              |      `0-1-4`       |          |           |   ---    |      ---       |
|                           ARIMA(C)                           |        ---         |          |           |   ---    |      ---       |
|                           XGBoost                            |   `9-14-2-200-5`   |          |           |   ---    |      ---       |
|                             GBRT                             |  `12-10-4-200-5`   |          |           |   ---    |      ---       |
|                       ST_MGCN (G/DCI)                        |      `待补充`      |          |           |  248985  |                |
|                         DCRNN(G/D C)                         |        ---         |          |           |          |                |
|                           LSTM(C)                            |   `1-64-32-2-64`   |          |           |          |                |
|                            TMeta                             | `1-1-1-64-32-2-64` |          |           |  62789   |                |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` |          |           |  189521  |                |
|                   AMulti-GCLSTM-V2 (G/DCI)                   |                    |          |           |  180561  |                |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    |          |           |  488447  |                |



| <font color='#ff0000'>**City: Chongqing Fitness:30mins**</font> |       Params       | val-rmse | test-rmse | # Params | Converged Time |
| :----------------------------------------------------------: | :----------------: | :------: | :-------: | :------: | :------------: |
|                              HM                              |      `0-1-4`       |          |           |   ---    |      ---       |
|                           ARIMA(C)                           |        ---         |          |           |   ---    |      ---       |
|                           XGBoost                            |   `9-14-2-200-5`   |          |           |   ---    |      ---       |
|                             GBRT                             |  `12-10-4-200-5`   |          |           |   ---    |      ---       |
|                       ST_MGCN (G/DCI)                        |      `待补充`      |          |           |  248985  |                |
|                         DCRNN(G/D C)                         |        ---         |          |           |          |                |
|                           LSTM(C)                            |   `1-64-32-2-64`   |          |           |          |                |
|                            TMeta                             |                    |          |           |          |                |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` |          |           |  189521  |                |
|                   AMulti-GCLSTM-V2 (G/DCI)                   |                    |          |           |  180561  |                |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    |          |           |  488447  |                |



| <font color='#ff0000'>**City: Chongqing <br />Fitness: 60mins**</font> |       Params       | val-rmse  | test-rmse | \# Params |     Converged Time     |
| :----------------------------------------------------------: | :----------------: | :-------: | :-------: | :-------: | :--------------------: |
|                              HM                              |     `0-1-4` ✅      | 208.73630 | 120.30723 |    ---    |          ---           |
|                           ARIMA(C)                           |        ---         | 547.82632 | 578.18563 |    ---    |          ---           |
|                           XGBoost                            |  `9-14-2-200-5` ✅  | 115.05053 | 117.05069 |    ---    |          ---           |
|                             GBRT                             | `12-10-4-200-5 `✅  | 118.89574 | 113.92276 |    ---    |          ---           |
|                       ST_MGCN (G/DCI)                        |      `待补充`      | 105.19451 | 118.86668 |  248985   | 40.38 hour 2189 epochs |
|                         DCRNN(G/D C)                         |        ---         | 93.04695  | 122.31121 |           |                        |
|                           LSTM(C)                            |   `1-64-32-2-64`   |           |           |           |                        |
|                            TMeta                             |                    |           |           |   62789   |                        |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` |           |           |  189521   |                        |
|                   AMulti-GCLSTM-V2 (G/DCI)                   |                    |           |           |  180561   |                        |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    |           |           |  488447   |                        |





## Results on Charge-Station

| <font color='#ff0000'>**City: Beijing <br />TimeFitness: 15mins**</font> |       Params       | val-rmse | test-rmse | # Params | Converged Time |
| :----------------------------------------------------------: | :----------------: | :------: | :-------: | :------: | :------------: |
|                              HM                              |      `2-0-2`       |          |           |   ---    |      ---       |
|                           ARIMA(C)                           |                    |          |           |   ---    |      ---       |
|                           XGBoost                            |   `12-7-0-20-2`    |          |           |   ---    |      ---       |
|                             GBRT                             |  `12-10-0-100-2`   |          |           |   ---    |      ---       |
|                        ST_MGCN (G/DC)                        |      `待补充`      |          |           |  166025  |                |
|                         DCRNN(G/D C)                         |                    |          |           |  50368   |                |
|                           LSTM(C)                            |   `1-64-32-2-64`   |          |           |  28992   |                |
|                            TMeta                             |                    |          |           |  62789   |                |
|                   AMulti-GCLSTM-V1 (G/DC)                    | `1-1-1-64-32-2-64` |          |           |  130379  |                |
|                   AMulti-GCLSTM-V2 (G/DC)                    |                    |          |           |  129867  |                |
|                   AMulti-GCLSTM-V3 (G/DC)                    |                    |          |           |  488447  |                |



| <font color='#ff0000'>**City: Beijing <br />TimeFitness: 30mins**</font> |       Params       | val-rmse | test-rmse | # Params | Converged Time |
| :----------------------------------------------------------: | :----------------: | :------: | :-------: | :------: | :------------: |
|                              HM                              |      `2-0-2`       |          |           |   ---    |      ---       |
|                           ARIMA(C)                           |                    |          |           |   ---    |      ---       |
|                           XGBoost                            |   `12-7-0-20-2`    |          |           |   ---    |      ---       |
|                             GBRT                             |  `12-10-0-100-2`   |          |           |   ---    |      ---       |
|                        ST_MGCN (G/DC)                        |      `待补充`      |          |           |  166025  |                |
|                         DCRNN(G/D C)                         |                    |          |           |  50368   |                |
|                           LSTM(C)                            |   `1-64-32-2-64`   |          |           |  28992   |                |
|                            TMeta                             |                    |          |           |  62789   |                |
|                   AMulti-GCLSTM-V1 (G/DC)                    | `1-1-1-64-32-2-64` |          |           |  130379  |                |
|                   AMulti-GCLSTM-V2 (G/DC)                    |                    |          |           |  129867  |                |
|                   AMulti-GCLSTM-V3 (G/DC)                    |                    |          |           |  488447  |                |





| <font color='#ff0000'>**City: Beijing <br />TimeFitness: 60mins**</font> |       Params       | val-rmse | test-rmse | \# Params |      Converged Time      |
| :----------------------------------------------------------: | :----------------: | :------: | :-------: | :-------: | :----------------------: |
|                              HM                              |     `2-0-2` ✅      | 0.99617  |  1.01610  |    ---    |           ---            |
|                           ARIMA(C)                           |                    | 0.96335  |  0.98236  |    ---    |           ---            |
|                           XGBoost                            |  `12-7-0-20-2` ✅   | 0.79800  |  0.83381  |    ---    |           ---            |
|                             GBRT                             | `12-10-0-100-2 `✅  | 0.79771  |  0.82814  |    ---    |           ---            |
|                        ST_MGCN (G/DC)                        |      `待补充`      | 0.59853  |  0.82714  |  166025   |  1.57 hour  253 epochs   |
|                         DCRNN(G/D C)                         |                    | 0.70646  |  0.98871  |   50368   | 7.20 hour / 10000 epochs |
|                           LSTM(C)                            |   `1-64-32-2-64`   |          |           |   28992   |                          |
|                            TMeta                             |                    |          |           |   62789   |                          |
|                   AMulti-GCLSTM-V1 (G/DC)                    | `1-1-1-64-32-2-64` |          |           |  130379   |                          |
|                   AMulti-GCLSTM-V2 (G/DC)                    |                    |          |           |  129867   |                          |
|                   AMulti-GCLSTM-V3 (G/DC)                    |                    |          |           |  488447   |                          |
