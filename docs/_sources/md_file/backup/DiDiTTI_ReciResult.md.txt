# Results on DiDiTTI Datasets

## Search Space

|      Model       |                         Search Space                         |
| :--------------: | :----------------------------------------------------------: |
|        HM        |               `CT: 0~6`, `PT: 0~7`, `TT: 0~4`                |
|      ARIMA       |                                                              |
|    ST_ResNet     |                           `待补充`                           |
|     XGBoost      | `CT: 0~12`, `PT: 0~14`, `TT: 0~4`, `estimater: 10~200`, `depth: 2~10` |
|       GBRT       | `CT: 0~12`, `PT: 0~14`, `TT: 0~4`, `estimater: 10~200`, `depth: 2~10` |
|       LSTM       | `lstm_layers: 1~3`, `lstm_hidden_units: 32~128 `, `dense_units: 32~128`, `temp_merge_heads: 2~4`, `temp_merge_units: 32~128` |
| STMeta-GCLSTM-V1 | `gcn_k: 1~3`, `gcn_l: 1~3` `gclstm_layers: 1~3`, `lstm_hidden_units: 64~256 `, `dense_units: 32~128`, `temp_merge_heads: 2~4`, `temp_merge_units: 32~128` |

原始数据为六个城市一年的数据，仅使用半年的数据进行实验，data_range参数为[59,273]

Note that C represent Correlation graph and R represent Road-distance graph(in previous experiment, we call it distant graph).

#### Results on Chengdu Dataset

|  **City: Chengdu**  |       Params       | val-rmse | test-rmse | # Params |       Converged Time       |
| :-----------------: | :----------------: | :------: | :-------: | :------: | :------------------------: |
|      ARIMA(TC)      |        ---         | 0.07955  |  0.08409  |   ---    |                            |
|     SARIMA(TC)      |   3-1-1-0-0-0-24   | 0.07860  |  0.08309  |          |                            |
|      LSTM(TC)       |                    | 0.20943  |  0.21869  |   ---    |            ---             |
|       HM(TM)        |       1-3-2✅       | 0.05889  |  0.06369  |          |                            |
|     XGBoost(TM)     |   14-5-2-161-2✅    | 0.05721  |  0.06155  |          |                            |
|      GBRT(TM)       |    13-4-1-52-4✅    | 0.05590  |  0.06008  |   ---    |            ---             |
| TMeta-LSTM-GAL (TM) |      `待补充`      | 0.05738  |  0.06041  |          |  31.28 hour / 4146 epochs  |
|    DCRNN (TC+SP)    |                    | 0.05965  |  0.06520  |          | 164.13 hour / 9717 epochs  |
|   ST-MGCN (TM+SM)   |   `1-64-32-2-64`   | 0.056217 |  0.05928  |          |                            |
|     STMeta-V1-C     | `1-1-1-64-32-2-64` | 0.05720  |  0.06048  |          |  64.47 hour / 4685 epochs  |
|     STMeta-V1-R     |                    | 0.05416  |  0.05738  |          | 372.21 hour / 45398 epochs |
|    STMeta-V1-CR     |                    | 0.05391  |  0.05694  |          | 378.97 hour / 15068 epochs |
|    STMeta-V2-CR     |                    |          |           |          |                            |
|    STMeta-V3-CR     |                    | 0.05465  |  0.05770  |          | 246.00 hour / 10000 epochs |

#### Results on Haikou Dataset

|  **City: Haikou**   |       Params       | val-rmse | test-rmse | # Params |      Converged Time      |
| :-----------------: | :----------------: | :------: | :-------: | :------: | :----------------------: |
|      ARIMA(TC)      |        ---         | 0.07348  |  0.07942  |   ---    |                          |
|     SARIMA(TC)      |       sp=24        | 0.06424  |  0.07058  |          |                          |
|      LSTM(TC)       |                    | 0.11948  |  0.12639  |   ---    |                          |
|       HM(TM)        |       1-2-2✅       | 0.05619  |  0.06277  |          |                          |
|     XGBoost(TM)     |   `16-8-0-128-2✅   | 0.05470  |  0.06092  |   ---    |           ---            |
|      GBRT(TM)       |   `13-6-1-69-4`✅   | 0.05355  |  0.05958  |    --    |           ---            |
| TMeta-LSTM-GAL (TM) |      `待补充`      | 0.05481  |  0.06087  |          |                          |
|    DCRNN (TC+SP)    |                    | 0.06884  |  0.07410  |          |                          |
|   ST-MGCN (TM+SM)   |                    | 0.05410  |  0.05983  |          |  3.74 hour / 386 epochs  |
|     STMeta-V1-C     | `1-1-1-64-32-2-64` | 0.05317  |  0.05798  |          | 3.30 hour / 1940 epochs  |
|     STMeta-V1-R     |                    | 0.05385  |  0.05908  |          |                          |
|    STMeta-V1-CR     |                    | 0.05449  |  0.06011  |          |                          |
|     STMeta-V2-C     |                    | 0.05436  |  0.06009  |          | 12.04 hour / 7020 epochs |
|     STMeta-V2-R     |                    | 0.05420  |  0.05955  |          |                          |
|    STMeta-V2-CR     |                    | 0.05390  |  0.05939  |          |                          |
|      STMeta-V3      |                    |          |           |          |                          |



#### Results on Jinan Dataset

|   **City: Jinan**   |       Params       | val-rmse | test-rmse | # Params | Converged Time |
| :-----------------: | :----------------: | :------: | :-------: | :------: | :------------: |
|      ARIMA(TC)      |        ---         | 0.07471  |  0.08329  |   ---    |      ---       |
|     SARIMA(TC)      |                    |          |           |          |                |
|      LSTM(TC)       |                    | 0.12365  |  0.13262  |   ---    |      ---       |
|       HM(TM)        |       1-2-2✅       | 0.05546  |  0.06323  |          |                |
|     XGBoost(TM)     |   `9-7-1-39-3`✅    | 0.05277  |  0.06171  |   ---    |      ---       |
|      GBRT(TM)       |    13-7-1-59-4✅    | 0.05164  |  0.06046  |   ---    |      ---       |
| TMeta-LSTM-GAL (TM) |      `待补充`      |          |           |          |                |
|    DCRNN (TC+SP)    |                    | 0.07140  |  0.06583  |          |                |
|   ST-MGCN (TM+SM)   |   `1-64-32-2-64`   |          |           |          |                |
|      STMeta-V1      | `1-1-1-64-32-2-64` |          |           |          |                |
|      STMeta-V2      |                    |          |           |          |                |
|      STMeta-V3      |                    |          |           |          |                |

#### Results on Shenzhen Dataset

| **City: Shenzhen**  |       Params       | val-rmse | test-rmse | # Params | Converged Time |
| :-----------------: | :----------------: | :------: | :-------: | :------: | :------------: |
|      ARIMA(TC)      |       3-1-1        | 0.08054  |  0.09018  |   ---    |      ---       |
|     SARIMA(TC)      |                    |          |           |          |                |
|      LSTM(TC)       |                    |          |           |   ---    |      ---       |
|       HM(TM)        |       1-2-3✅       | 0.065712 |  0.08016  |          |                |
|     XGBoost(TM)     |                    |          |           |   ---    |      ---       |
|      GBRT(TM)       |  `13-2-3-121-3`✅   | 0.06230  |  0.07569  |   ---    |      ---       |
| TMeta-LSTM-GAL (TM) |      `待补充`      |          |           |          |                |
|    DCRNN (TC+SP)    |                    |          |           |          |                |
|  ST-ResNet (TM+SP)  |                    |          |           |          |                |
|   ST-MGCN (TM+SM)   |   `1-64-32-2-64`   |          |           |          |                |
|      STMeta-V1      | `1-1-1-64-32-2-64` |          |           |          |                |
|      STMeta-V2      |                    |          |           |          |                |
|      STMeta-V3      |                    |          |           |          |                |

#### Results on Suzhou Dataset

|  **City: Suzhou**   |       Params       | val-rmse | test-rmse | # Params |      Converged Time       |
| :-----------------: | :----------------: | :------: | :-------: | :------: | :-----------------------: |
|      ARIMA(TC)      |        ---         | 0.06605  |  0.07136  |   ---    |            ---            |
|     SARIMA(TC)      |                    |          |           |          |                           |
|      LSTM(TC)       |                    | 0.10589  |  0.11267  |   ---    |   2.87 hour / 43 epochs   |
|       HM(TM)        |       1-2-3✅       | 0.05105  |  0.05481  |          |                           |
|     XGBoost(TM)     |    12-9-0-78-2✅    | 0.05008  |  0.05408  |          |                           |
|      GBRT(TM)       |  `12-11-1-43-4`✅   | 0.04928  |  0.05336  |   ---    |            ---            |
| TMeta-LSTM-GAL (TM) |      `待补充`      | 0.05010  |  0.05322  |          | 60.64 hour / 10000 epochs |
|    DCRNN (TC+SP)    |                    |          |           |          |                           |
|   ST-MGCN (TM+SM)   |   `1-64-32-2-64`   |          |           |          |                           |
|      STMeta-V1      | `1-1-1-64-32-2-64` |          |           |          |                           |
|      STMeta-V2      |                    |          |           |          |                           |
|      STMeta-V3      |                    |          |           |          |                           |

#### Results on Xi'an Dataset

|   **City: Xi'an**   |    Params    | val-rmse | test-rmse | # Params |       Converged Time       |
| :-----------------: | :----------: | :------: | :-------: | :------: | :------------------------: |
|      ARIMA(TC)      |     ---      | 0.07680  |  0.08594  |   ---    |            ---             |
|     SARIMA(TC)      |              |          |           |          |                            |
|      LSTM(TC)       |              | 0.07173  |  0.08033  |   ---    | 16.24 hour / 10000 epochs  |
|       HM(TM)        |    1-2-2✅    | 0.05381  |  0.06193  |          |                            |
|     XGBoost(TM)     | 9-12-0-41-3✅ | 0.05234  |  0.06031  |   ---    |            ---             |
|      GBRT(TM)       | 13-4-2-64-4✅ | 0.05080  |  0.05867  |   ---    |            ---             |
| TMeta-LSTM-GAL (TM) |              | 0.05227  |  0.05940  |          | 38.09 hour / 10000 epochs  |
|    DCRNN (TC+SP)    |              |          |           |          |                            |
|   ST-MGCN (TM+SM)   |              |          |           |          |                            |
|      STMeta-V1      |              | 0.05014  |  0.05616  |          | 102.62 hour / 10000 epochs |
|      STMeta-V2      |              | 0.05091  |  0.05715  |          | 83.07 hour / 10000 epochs  |
|      STMeta-V3      |              | 0.04974  |  0.05558  |          | 118.74 hour / 10000 epochs |







































































