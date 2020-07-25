# External Feature Ablation Results

Default granularity is 60 mins.

## Results on Bike Dataset

| **City: NYC** | external feature  | val-rmse | test-rmse |      Converged Time       |
| :-----------: | :---------------: | :------: | :-------: | :-----------------------: |
|    STMeta     |      not use      |    -     |  3.51827  |        5930 epochs        |
| STMeta-Gating |      weather      |          |           |                           |
| STMeta-Gating |      holiday      |          |           |                           |
| STMeta-Gating | temporal position |          |           |                           |
| STMeta-Gating |  weather-holiday  |          |           |                           |
| STMeta-Gating |    weather-tp     |          |           |                           |
| STMeta-Gating |    holiday-tp     |          |           |                           |
| STMeta-Gating |        all        |    -     |  3.37795  | 120.89 hour / 4043 epochs |

| **City: Chicago** | external feature  | val-rmse | test-rmse |      Converged Time      |
| :---------------: | :---------------: | :------: | :-------: | :----------------------: |
|      STMeta       |      not use      |    -     |  2.73998  | 22.00 hour / 1430 epochs |
|   STMeta-Gating   |      weather      | 2.18217  |  2.66780  |  9.18 hour / 420 epochs  |
|   STMeta-Gating   |      holiday      | 2.11500  |  2.65086  | 13.59 hour / 720 epochs  |
|   STMeta-Gating   | temporal position | 2.04238  |  2.58757  | 14.68 hour / 781 epochs  |
|   STMeta-Gating   |  weather-holiday  | 2.12527  |  2.65247  | 10.54 hour / 459 epochs  |
|   STMeta-Gating   |    weather-tp     | 2.03994  |  2.55323  |  7.43 hour / 335 epochs  |
|   STMeta-Gating   |    holiday-tp     | 2.04882  |  2.55389  |  6.93 hour / 315 epochs  |
|   STMeta-Gating   |        all        |    -     |  2.59783  | 67.95 hour / 3888 epochs |

| **City: DC**  | external feature  | val-rmse | test-rmse |      Converged Time      |
| :-----------: | :---------------: | :------: | :-------: | :----------------------: |
|    STMeta     |      not use      |          |           |                          |
| STMeta-Gating |      weather      | 2.64569  |  2.44860  | 20.68 hour / 1267 epochs |
| STMeta-Gating |      holiday      |          |           |                          |
| STMeta-Gating | temporal position |          |           |                          |
| STMeta-Gating |  weather-holiday  |          |           |                          |
| STMeta-Gating |    weather-tp     |          |           |                          |
| STMeta-Gating |    holiday-tp     |          |           |                          |
| STMeta-Gating |        all        | 2.54658  |  2.43501  | 54.22 hour / 3563 epochs |

## Results on DiDi Dataset

| **City: Xian** | external feature  | val-rmse |  test-rmse  |      Converged Time      |
| :------------: | :---------------: | :------: | :---------: | :----------------------: |
|     STMeta     |      not use      | 7.62051  |   5.82054   | 3.68 hour / 4367 epochs  |
| STMeta-Gating  |      weather      | 6.56913  |   6.14120   | 13.27 hour / 7498 epochs |
| STMeta-Gating  |      holiday      | 7.54557  |   5.78980   | 3.27 hour / 1608 epochs  |
| STMeta-Gating  | temporal position | 6.53068  | **5.68496** | 8.61 hour / 4878 epochs  |
| STMeta-Gating  |  weather-holiday  | 7.42879  |   6.06445   | 2.53 hour / 1208 epochs  |
| STMeta-Gating  |    weather-tp     | 6.41114  |   5.94091   | 6.36 hour / 3164 epochs  |
| STMeta-Gating  |    holiday-tp     | 6.75393  | **5.69865** | 11.33 hour / 6350 epochs |
| STMeta-Gating  |        all        | 6.62653  |   5.80114   |  1.57 hour / 410 epochs  |

| **City: Chengdu** | external feature  | val-rmse |  test-rmse  |     Converged Time      |
| :---------------: | :---------------: | :------: | :---------: | :---------------------: |
|      STMeta       |      not use      | 6.81043  |   6.90155   | 1.58 hour / 1218 epochs |
|   STMeta-Gating   |      weather      | 7.06867  |   6.98848   | 1.19 hour / 184 epochs  |
|   STMeta-Gating   |      holiday      | 6.78676  | **6.84083** | 3.87 hour / 2778 epochs |
|   STMeta-Gating   | temporal position | 6.77283  |   6.96706   | 9.08 hour / 6428 epochs |
|   STMeta-Gating   |  weather-holiday  | 6.90914  | **6.89400** | 1.30 hour / 477 epochs  |
|   STMeta-Gating   |    weather-tp     | 6.88513  |   6.96674   | 1.63 hour / 816 epochs  |
|   STMeta-Gating   |    holiday-tp     | 6.67799  |   6.92909   | 3.57 hour / 2278 epochs |
|   STMeta-Gating   |        all        | 6.84756  |   6.95486   | 1.49 hour / 1300 epochs |

## Results on Metro Dataset

| **City: Shanghai** | external feature  | val-rmse  |   test-rmse   |      Converged Time       |
| :----------------: | :---------------: | :-------: | :-----------: | :-----------------------: |
|       STMeta       |      not use      | 108.01402 |   154.47606   |  5.01 hour / 4661 epochs  |
|   STMeta-Gating    |      weather      | 111.37406 |   170.38507   |  2.43 hour / 1057 epochs  |
|   STMeta-Gating    |      holiday      | 102.33872 |   155.98723   | 15.34 hour / 7944 epochs  |
|   STMeta-Gating    | temporal position | 97.73984  |    131.662    | 36.09 hour / 19476 epochs |
|   STMeta-Gating    |  weather-holiday  | 114.22076 |   164.31705   | 10.04 hour / 4660 epochs  |
|   STMeta-Gating    |    weather-tp     | 114.11836 |   143.5678    | 16.89 hour / 7919 epochs  |
|   STMeta-Gating    |    holiday-tp     | 96.05388  | **124.23711** | 41.68 hour / 20000 epochs |
|   STMeta-Gating    |        all        | 106.15893 |   145.45236   |  6.00 hour / 2563 epochs  |

| **City: Chongqing** | external feature  | val-rmse | test-rmse | Converged Time |
| :-----------------: | :---------------: | :------: | :-------: | :------------: |
|       STMeta        |      not use      |          |           |                |
|    STMeta-Gating    |      weather      |          |           |                |
|    STMeta-Gating    |      holiday      |          |           |                |
|    STMeta-Gating    | temporal position |          |           |                |
|    STMeta-Gating    |  weather-holiday  |          |           |                |
|    STMeta-Gating    |    weather-tp     |          |           |                |
|    STMeta-Gating    |    holiday-tp     |          |           |                |
|    STMeta-Gating    |        all        |          |           |                |

## Results on EV Dataset

| **City: Beijing** | external feature  | val-rmse | test-rmse |      Converged Time       |
| :---------------: | :---------------: | :------: | :-------: | :-----------------------: |
|      STMeta       |      not use      | 0.79145  |  0.81805  | 10.58 hour / 6205 epochs  |
|   STMeta-Gating   |      weather      | 0.76781  |  0.81634  | 25.75 hour / 13129 epochs |
|   STMeta-Gating   |      holiday      | 0.75004  |  0.78205  | 18.80 hour / 9315 epochs  |
|   STMeta-Gating   | temporal position | 0.74307  |  0.80274  | 32.46 hour / 18586 epochs |
|    STMeta-Gating    |  weather-holiday  | 0.75671 | 0.79993 | 16.83 hour / 10000 epochs |
|    STMeta-Gating    |    weather-tp     | 0.74291 | 0.78019 | 13.59 hour / 7866 epochs |
|    STMeta-Gating    |    holiday-tp     | 0.73362 | **0.77900** | 6.93 hour / 10000 epochs |
|    STMeta-Gating    |        all        | 0.74789 | 0.78317 | 9.68 hour / 4563 epochs |