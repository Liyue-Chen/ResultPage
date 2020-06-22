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
| STMeta-Gating  |  weather-holiday  |          |           |                          |
| STMeta-Gating  |    weather-tp     |          |           |                          |
| STMeta-Gating  |    holiday-tp     |          |           |                          |
| STMeta-Gating  |        all        | 6.626533 | 5.8011427 |  1.57 hour / 410 epochs  |

| **City: Chengdu** | external feature  | val-rmse | test-rmse | Converged Time |
| :---------------: | :---------------: | :------: | :-------: | :------------: |
|      STMeta       |      not use      |          |           |                |
|   STMeta-Gating   |      weather      |          |           |                |
|   STMeta-Gating   |      holiday      |          |           |                |
|   STMeta-Gating   | temporal position |          |           |                |
|   STMeta-Gating   |  weather-holiday  |          |           |                |
|   STMeta-Gating   |    weather-tp     |          |           |                |
|   STMeta-Gating   |    holiday-tp     |          |           |                |
|   STMeta-Gating   |        all        |          |           |                |

## Results on Metro Dataset

| **City: Shanghai** | external feature  | val-rmse  | test-rmse |      Converged Time       |
| :----------------: | :---------------: | :-------: | :-------: | :-----------------------: |
|       STMeta       |      not use      | 108.01402 | 154.47606 |  5.01 hour / 4661 epochs  |
|   STMeta-Gating    |      weather      | 111.37406 | 170.38507 |  2.43 hour / 1057 epochs  |
|   STMeta-Gating    |      holiday      | 102.33872 | 155.98723 | 15.34 hour / 7944 epochs  |
|   STMeta-Gating    | temporal position | 97.73984  |  131.662  | 36.09 hour / 19476 epochs |
|   STMeta-Gating    |  weather-holiday  |           |           |                           |
|   STMeta-Gating    |    weather-tp     |           |           |                           |
|   STMeta-Gating    |    holiday-tp     |           |           |                           |
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