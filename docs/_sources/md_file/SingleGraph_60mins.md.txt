# 60 mins Single Graph

## Results on Bike Dataset

|       **City: NYC**        | Version | val-rmse |  test-rmse  |     Converged Time      |
| :------------------------: | :-----: | :------: | :---------: | :---------------------: |
|     Only Functionality     |   V3    | 1.93778  | **3.47656** | 8.09 hour / 5962 epochs |
|       Only Proximity       |   V3    | 1.92778  |   3.50875   | 7.42 hour / 5355 epochs |
| Only Interaction/Same-line |   V3    | 1.95641  |   3.54281   | 4.86 hour / 3671 epochs |
|    Aggregation Together    |   V3    |    -     |   3.52124   |       7438 epochs       |

|     **City: Chicago**      | Version | val-rmse | test-rmse | Converged Time |
| :------------------------: | :-----: | :------: | :-------: | :------------: |
|     Only Functionality     |   V3    |          |           |                |
|       Only Proximity       |   V3    |          |           |                |
| Only Interaction/Same-line |   V3    |          |           |                |
|    Aggregation Together    |   V3    |    -     |  2.65204  |  4403 epochs   |

|        **City: DC**        | Version | val-rmse | test-rmse | Converged Time |
| :------------------------: | :-----: | -------- | :-------: | :------------: |
|     Only Functionality     |   V3    |          |           |                |
|       Only Proximity       |   V3    |          |           |                |
| Only Interaction/Same-line |   V3    |          |           |                |
|    Aggregation Together    |   V3    |          |  2.42338  |                |

## Results on DiDi Dataset

|       **City: Xian**       | Version | val-rmse | test-rmse |     Converged Time      |
| :------------------------: | :-----: | :------: | :-------: | :---------------------: |
|     Only Functionality     |   V3    |          |           |                         |
|       Only Proximity       |   V3    |          |           |                         |
| Only Interaction/Same-line |   V3    |          |           |                         |
|    Aggregation Together    |   V3    | 7.14426  |  5.90812  | 3.37 hour / 2393 epochs |

|     **City: Chengdu**      | Version | val-rmse | test-rmse |     Converged Time      |
| :------------------------: | :-----: | :------: | :-------: | :---------------------: |
|     Only Functionality     |   V3    |          |           |                         |
|       Only Proximity       |   V3    |          |           |                         |
| Only Interaction/Same-line |   V3    |          |           |                         |
|    Aggregation Together    |   V3    | 6.30479  |  6.90394  | 1.76 hour / 1052 epochs |

## Results on Metro Dataset

|     **City: Shanghai**     | Version | val-rmse  | test-rmse |      Converged Time       |
| :------------------------: | :-----: | :-------: | :-------: | :-----------------------: |
|     Only Functionality     |   V3    |           |           |                           |
|       Only Proximity       |   V3    |           |           |                           |
| Only Interaction/Same-line |   V3    |           |           |                           |
|    Aggregation Together    |   V3    | 117.82761 | 143.18166 | 30.38 hour / 20000 epochs |

|    **City: Chongqing**     | Version | val-rmse | test-rmse |      Converged Time       |
| :------------------------: | :-----: | :------: | :-------: | :-----------------------: |
|     Only Functionality     |   V3    |          |           |                           |
|       Only Proximity       |   V3    |          |           |                           |
| Only Interaction/Same-line |   V3    |          |           |                           |
|    Aggregation Together    |   V3    | 88.32695 | 94.77593  | 40.19 hour / 10004 epochs |

## Results on EV Dataset

|     **City: Beijing**      | Version | val-rmse | test-rmse |      Converged Time       |
| :------------------------: | :-----: | :------: | :-------: | :-----------------------: |
|     Only Functionality     |   V3    |          |           |                           |
|       Only Proximity       |   V3    |          |           |                           |
| Only Interaction/Same-line |   V3    |    -     |     -     |             -             |
|    Aggregation Together    |   V3    | 0.57685  |  0.80259  | 23.76 hour / 10497 epochs |

