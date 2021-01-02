# External Feature Ablation Results

Default granularity is 60 mins.

## Results on Bike Dataset

| **City: NYC** | external feature  | val-rmse |  test-rmse  |      Converged Time       |
| :-----------: | :---------------: | :------: | :---------: | :-----------------------: |
|    STMeta     |      not use      |    -     |    3.605    |        5930 epochs        |
|  Raw-Gating   |      weather      | 3.17885  |   3.45162   | 266.52 hour / 8060 epochs |
|  Raw-Gating   |      holiday      | 3.18443  |   3.51716   | 292.43 hour / 9057 epochs |
|  Raw-Gating   | temporal position | 3.03264  |   3.40923   | 40.62 hour / 1142 epochs  |
|  Raw-Gating   |  weather-holiday  | 3.23032  |   3.45488   |  30.39 hour / 736 epochs  |
|  Raw-Gating   |    weather-tp     | 3.01989  | **3.36129** | 133.19 hour / 4452 epochs |
|  Raw-Gating   |    holiday-tp     | 3.06666  |   3.40982   | 120.52 hour / 3967 epochs |
|  Raw-Gating   |        all        |    -     | **3.37795** | 120.89 hour / 4043 epochs |

| **City: Chicago** | external feature  | val-rmse | test-rmse |      Converged Time      |
| :---------------: | :---------------: | :------: | :-------: | :----------------------: |
|      STMeta       |      not use      |    -     |  2.73998  | 22.00 hour / 1430 epochs |
|    Raw-Gating     |      weather      | 2.18217  |  2.66780  |  9.18 hour / 420 epochs  |
|    Raw-Gating     |      holiday      | 2.11500  |  2.65086  | 13.59 hour / 720 epochs  |
|    Raw-Gating     | temporal position | 2.04238  |  2.58757  | 14.68 hour / 781 epochs  |
|    Raw-Gating     |  weather-holiday  | 2.12527  |  2.65247  | 10.54 hour / 459 epochs  |
|    Raw-Gating     |    weather-tp     | 2.03994  |  2.55323  |  7.43 hour / 335 epochs  |
|    Raw-Gating     |    holiday-tp     | 2.04882  |  2.55389  |  6.93 hour / 315 epochs  |
|    Raw-Gating     |        all        |    -     |  2.59783  | 67.95 hour / 3888 epochs |

| **City: DC** | external feature  | val-rmse | test-rmse |      Converged Time      |
| :----------: | :---------------: | :------: | :-------: | :----------------------: |
|    STMeta    |      not use      |    -     |  2.44287  | 78.61 hour / 5750 epochs |
|  Raw-Gating  |      weather      | 2.64569  |  2.44860  | 20.68 hour / 1267 epochs |
|  Raw-Gating  |      holiday      | 2.59700  |  2.45220  | 56.99 hour / 3534 epochs |
|  Raw-Gating  | temporal position | 2.50228  |  2.39943  | 31.97 hour / 1840 epochs |
|  Raw-Gating  |  weather-holiday  | 2.61706  |  2.44108  | 39.66 hour / 2299 epochs |
|  Raw-Gating  |    weather-tp     | 2.54364  |  2.40836  | 25.07 hour / 1420 epochs |
|  Raw-Gating  |    holiday-tp     | 2.50821  |  2.40522  | 28.31 hour / 1607 epochs |
|  Raw-Gating  |        all        | 2.54658  |  2.43501  | 54.22 hour / 3563 epochs |

DC站点的Weather特征有问题，基本全错。

## Results on DiDi Dataset

| **City: Xian** |   external feature   |     val-rmse      |  test-rmse  |      Converged Time      |
| :------------: | :------------------: | :---------------: | :---------: | :----------------------: |
|     STMeta     |       not use        |      7.62051      |   5.82054   | 3.68 hour / 4367 epochs  |
|   Raw-Gating   |       weather        |      6.56913      |   6.14120   | 13.27 hour / 7498 epochs |
|   Raw-Gating   |       holiday        |      7.54557      |   5.78980   | 3.27 hour / 1608 epochs  |
|   Raw-Gating   |  temporal position   |      6.53068      | **5.68496** | 8.61 hour / 4878 epochs  |
|   Raw-Gating   |      POIs(1km)       |         -         |   5.82147   | 9.29 hour / 4367 epochs  |
|   Raw-Gating   |      POIs(5km)       |         -         |   5.86587   |  5.31 hour/ 2168 epochs  |
|   Raw-Gating   |     POIs-weather     | `running 2080 Ti` |             |                          |
|   Raw-Gating   |     POIs-holiday     |                   |             |                          |
|   Raw-Gating   |       POIs-tp        |                   |             |                          |
|   Raw-Gating   |   weather-holiday    |      7.42879      |   6.06445   | 2.53 hour / 1208 epochs  |
|   Raw-Gating   |      weather-tp      |      6.41114      |   5.94091   | 6.36 hour / 3164 epochs  |
|   Raw-Gating   |      holiday-tp      |      6.75393      | **5.69865** | 11.33 hour / 6350 epochs |
|   Raw-Gating   | POIs-weather-holiday |                   |             |                          |
|   Raw-Gating   |   POIs-weather-tp    |                   |             |                          |
|   Raw-Gating   |  weather-holiday-tp  |      6.62653      |   5.80114   |  1.57 hour / 410 epochs  |
|   Raw-Gating   |         all          |                   |             |                          |

| **City: Chengdu** | external feature  | val-rmse |  test-rmse  |     Converged Time      |
| :---------------: | :---------------: | :------: | :---------: | :---------------------: |
|      STMeta       |      not use      | 6.81043  |   6.90155   | 1.58 hour / 1218 epochs |
|    Raw-Gating     |      weather      | 7.06867  |   6.98848   | 1.19 hour / 184 epochs  |
|    Raw-Gating     |      holiday      | 6.78676  | **6.84083** | 3.87 hour / 2778 epochs |
|    Raw-Gating     | temporal position | 6.77283  |   6.96706   | 9.08 hour / 6428 epochs |
|    Raw-Gating     |     POIs(1km)     |    -     |   6.91176   | 3.44 hour / 2102 epochs |
|    Raw-Gating     |     POIs(5km)     |    -     |   6.94793   | 3.07 hour / 1720 epochs |
|   Raw-Gating   |     POIs-weather     |          |             |                          |
|   Raw-Gating   |     POIs-holiday     |          |             |                          |
|   Raw-Gating   |       POIs-tp        |          |             |                          |
|    Raw-Gating     |  weather-holiday  | 6.90914  | **6.89400** | 1.30 hour / 477 epochs  |
|    Raw-Gating     |    weather-tp     | 6.88513  |   6.96674   | 1.63 hour / 816 epochs  |
|    Raw-Gating     |    holiday-tp     | 6.67799  |   6.92909   | 3.57 hour / 2278 epochs |
| Raw-Gating | POIs-weather-holiday |  |  |  |
| Raw-Gating | POIs-weather-tp |  |  |  |
| Raw-Gating | weather-holiday-tp | 6.84756 |   6.95486   | 1.49 hour / 1300 epochs |
|    Raw-Gating     |        all        |          |             |                         |

## Results on Metro Dataset

| **City: Shanghai** | external feature  | val-rmse  |  test-rmse   |      Converged Time       |
| :----------------: | :---------------: | :-------: | :----------: | :-----------------------: |
|       STMeta       |      not use      | 108.01402 |   154.4761   |  5.01 hour / 4661 epochs  |
|     Raw-Gating     |      weather      | 111.37406 |   170.3851   |  2.43 hour / 1057 epochs  |
|     Raw-Gating     |      holiday      | 102.33872 |   155.9872   | 15.34 hour / 7944 epochs  |
|     Raw-Gating     | temporal position | 97.73984  |   131.6620   | 36.09 hour / 19476 epochs |
|     Raw-Gating     |     POIs(1km)     |     -     |   161.8094   | 22.32 hour / 10000 epochs |
|     Raw-Gating     |     POIs(5km)     |     -     |   153.2931   | 21.92 hour / 10000 epochs |
|   Raw-Gating   |     POIs-weather     |          |             |                          |
|   Raw-Gating   |     POIs-holiday     | `running 2080 lenovo` |             |                          |
|   Raw-Gating   |       POIs-tp        |          |             |                          |
|     Raw-Gating     |  weather-holiday  | 114.22076 |   164.3171   | 10.04 hour / 4660 epochs  |
|     Raw-Gating     |    weather-tp     | 114.11836 |   143.5678   | 16.89 hour / 7919 epochs  |
|     Raw-Gating     |    holiday-tp     | 96.05388  | **124.2371** | 41.68 hour / 20000 epochs |
| Raw-Gating | POIs-weather-holiday |  |  |  |
| Raw-Gating | POIs-weather-tp |  |  |  |
|     Raw-Gating     |        weather-holiday-tp        | 106.15893 |   145.4524   |  6.00 hour / 2563 epochs  |
| Raw-Gating | all |  |  |  |

| **City: Chongqing** | external feature  | val-rmse  |  test-rmse   |      Converged Time       |
| :-----------------: | :---------------: | :-------: | :----------: | :-----------------------: |
|       STMeta        |      not use      | 96.49490  |   92.83833   | 108.53 hour / 9808 epochs |
|     Raw-Gating      |      weather      | 97.45921  |  108.59510   | 91.03 hour / 10000 epochs |
|     Raw-Gating      |      holiday      | 108.35061 |   95.67088   | 90.25 hour / 9982 epochs  |
|     Raw-Gating      | temporal position | 95.75195  |   91.66337   | 89.86 hour / 9794 epochs  |
|     Raw-Gating      |  weather-holiday  | 116.33015 |  101.04277   | 86.02 hour / 6520 epochs  |
|     Raw-Gating      |    weather-tp     | 97.76533  | **84.95356** | 94.19 hour / 9996 epochs  |
|     Raw-Gating      |    holiday-tp     | 99.32960  |   93.68919   | 79.96 hour / 8468 epochs  |
|     Raw-Gating      |        all        | 94.25858  | **87.03069** | 39.27 hour / 10000 epochs |

## Results on EV Dataset

| **City: Beijing** | external feature  | val-rmse | test-rmse |      Converged Time       |
| :---------------: | :---------------: | :------: | :-------: | :-----------------------: |
|      STMeta       |      not use      | 0.79145  |  0.81805  | 10.58 hour / 6205 epochs  |
|   Raw-Gating   |      weather      | 0.76781  |  0.81634  | 25.75 hour / 13129 epochs |
|   Raw-Gating   |      holiday      | 0.75004  |  0.78205  | 18.80 hour / 9315 epochs  |
|   Raw-Gating   | temporal position | 0.74307  |  0.80274  | 32.46 hour / 18586 epochs |
| Raw-Gating | POIs(1km) | `Dual 2080 Ti` |             |                           |
| Raw-Gating | POIs(5km) |  |  |  |
|   Raw-Gating   |     POIs-weather     |          |             |                          |
|   Raw-Gating   |     POIs-holiday     |          |             |                          |
|   Raw-Gating   |       POIs-tp        |          |             |                          |
|    Raw-Gating    |  weather-holiday  | 0.75671 | 0.79993 | 16.83 hour / 10000 epochs |
|    Raw-Gating    |    weather-tp     | 0.74291 | **0.78019** | 13.59 hour / 7866 epochs |
|    Raw-Gating    |    holiday-tp     | 0.73362 | **0.77900** | 6.93 hour / 10000 epochs |
| Raw-Gating | POIs-weather-holiday |  |  |  |
| Raw-Gating | POIs-weather-tp |  |  |  |
| Raw-Gating | weather-holiday-tp | 0.74789 | 0.78317 | 9.68 hour / 4563 epochs |
|    Raw-Gating    |        all        |          |             |                           |