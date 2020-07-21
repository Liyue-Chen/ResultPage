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

| **City: Chicago** | external feature  | val-rmse | test-rmse | Converged Time |
| :---------------: | :---------------: | :------: | :-------: | :------------: |
|      STMeta       |      not use      |          |           |                |
|   STMeta-Gating   |      weather      |          |           |                |
|   STMeta-Gating   |      holiday      |          |           |                |
|   STMeta-Gating   | temporal position |          |           |                |
|   STMeta-Gating   |  weather-holiday  |          |           |                |
|   STMeta-Gating   |    weather-tp     |          |           |                |
|   STMeta-Gating   |    holiday-tp     |          |           |                |
|   STMeta-Gating   |        all        |          |           |                |

| **City: DC**  | external feature  | val-rmse | test-rmse | Converged Time |
| :-----------: | :---------------: | :------: | :-------: | :------------: |
|    STMeta     |      not use      |          |           |                |
| STMeta-Gating |      weather      |          |           |                |
| STMeta-Gating |      holiday      |          |           |                |
| STMeta-Gating | temporal position |          |           |                |
| STMeta-Gating |  weather-holiday  |          |           |                |
| STMeta-Gating |    weather-tp     |          |           |                |
| STMeta-Gating |    holiday-tp     |          |           |                |
| STMeta-Gating |        all        |          |           |                |

## Results on DiDi Dataset

| **City: Xian** | external feature  | val-rmse | test-rmse |      Converged Time      |
| :------------: | :---------------: | :------: | :-------: | :----------------------: |
|     STMeta     |      not use      | 7.62051  |  5.82054  | 3.68 hour / 4367 epochs  |
| STMeta-Gating  |      weather      | 6.56913  |  6.14120  | 13.27 hour / 7498 epochs |
| STMeta-Gating  |      holiday      | 7.54557  |  5.78980  | 3.27 hour / 1608 epochs  |
| STMeta-Gating  | temporal position | 6.53068  |  5.68496  | 8.61 hour / 4878 epochs  |
| STMeta-Gating  |  weather-holiday  | 7.42879  |  6.06445  | 2.53 hour / 1208 epochs  |
| STMeta-Gating  |    weather-tp     | 6.41114  |  5.94091  | 6.36 hour / 3164 epochs  |
| STMeta-Gating  |    holiday-tp     | 6.75393  |  5.69865  | 11.33 hour / 6350 epochs |
| STMeta-Gating  |        all        | 6.62653  |  5.80114  |  1.57 hour / 410 epochs  |

| **City: Chengdu** | external feature  | val-rmse | test-rmse |     Converged Time      |
| :---------------: | :---------------: | :------: | :-------: | :---------------------: |
|      STMeta       |      not use      |          |           |                         |
|   STMeta-Gating   |      weather      | 7.06867  |  6.98848  | 1.19 hour / 184 epochs  |
|   STMeta-Gating   |      holiday      | 6.78676  |  6.84083  | 3.87 hour / 2778 epochs |
|   STMeta-Gating   | temporal position | 6.77283  |  6.96706  | 9.08 hour / 6428 epochs |
|   STMeta-Gating   |  weather-holiday  | 6.90914  |  6.89400  | 1.30 hour / 477 epochs  |
|   STMeta-Gating   |    weather-tp     | 6.88513  |  6.96674  | 1.63 hour / 816 epochs  |
|   STMeta-Gating   |    holiday-tp     | 6.67799  |  6.92909  | 3.57 hour / 2278 epochs |
|   STMeta-Gating   |        all        |          |           |                         |

## Results on Metro Dataset

| **City: Shanghai** | external feature  | val-rmse  | test-rmse |      Converged Time       |
| :----------------: | :---------------: | :-------: | :-------: | :-----------------------: |
|       STMeta       |      not use      | 108.01402 | 154.47606 |  5.01 hour / 4661 epochs  |
|   STMeta-Gating    |      weather      | 111.37406 | 170.38507 |  2.43 hour / 1057 epochs  |
|   STMeta-Gating    |      holiday      | 102.33872 | 155.98723 | 15.34 hour / 7944 epochs  |
|   STMeta-Gating    | temporal position | 97.73984  |  131.662  | 36.09 hour / 19476 epochs |
|   STMeta-Gating    |  weather-holiday  | 114.22076 | 164.31705 | 10.04 hour / 4660 epochs  |
|   STMeta-Gating    |    weather-tp     | 114.11836 | 143.5678  | 16.89 hour / 7919 epochs  |
|   STMeta-Gating    |    holiday-tp     | 96.05388  | 124.23711 | 41.68 hour / 20000 epochs |
|   STMeta-Gating    |        all        | 106.15893 | 145.45236 |  6.00 hour / 2563 epochs  |

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
|    STMeta-Gating    |  weather-holiday  |          |           |                |
|    STMeta-Gating    |    weather-tp     |          |           |                |
|    STMeta-Gating    |    holiday-tp     |          |           |                |
|    STMeta-Gating    |        all        | 0.74789 | 0.78317 | 9.68 hour / 4563 epochs |