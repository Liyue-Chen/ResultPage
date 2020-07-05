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
| :------------------------: | :-----: | :------: | :-------: | :------------: |
|     Only Functionality     |   V3    |          |           |                |
|       Only Proximity       |   V3    |          |           |                |
| Only Interaction/Same-line |   V3    |          |           |                |
|    Aggregation Together    |   V3    |    -     |  2.42338  |                |

## Results on DiDi Dataset（云上运行）

|       **City: Xian**       | Version | val-rmse |  test-rmse  |      Converged Time      |
| :------------------------: | :-----: | :------: | :---------: | :----------------------: |
|     Only Functionality     |   V3    | 7.23334  |   5.80516   | 2.33 hour / 7982 epochs  |
|       Only Proximity       |   V3    | 7.07511  | **5.78975** | 6.31 hour / 46461 epochs |
| Only Interaction/Same-line |   V3    | 7.36363  |   5.80832   | 6.35 hour / 27936 epochs |
|    Aggregation Together    |   V3    | 7.14426  |   5.90812   | 3.37 hour / 2393 epochs  |

|     **City: Chengdu**      | Version | val-rmse |  test-rmse  |      Converged Time      |
| :------------------------: | :-----: | :------: | :---------: | :----------------------: |
|     Only Functionality     |   V3    | 6.36493  | **6.87754** | 0.69 hour / 1869 epochs  |
|       Only Proximity       |   V3    | 6.43997  |   6.91376   | 0.76 hour / 2075 epochs  |
| Only Interaction/Same-line |   V3    | 6.37446  |   6.87930   | 3.24 hour / 10274 epochs |
|    Aggregation Together    |   V3    | 6.30479  |   6.90394   | 1.76 hour / 1052 epochs  |

## Results on Metro Dataset

|     **City: Shanghai**     | Version | val-rmse  |   test-rmse   |      Converged Time       |
| :------------------------: | :-----: | :-------: | :-----------: | :-----------------------: |
|     Only Functionality     |   V3    | 125.55458 |   148.25241   | 6.86 hour / 20000 epochs  |
|       Only Proximity       |   V3    | 127.04750 |   153.98045   | 6.77 hour / 20000 epochs  |
| Only Interaction/Same-line |   V3    | 123.43643 |   151.37936   | 7.05 hour / 20000 epochs  |
|    Aggregation Together    |   V3    | 117.82761 | **143.18166** | 30.38 hour / 20000 epochs |

|    **City: Chongqing**     | Version | val-rmse  |  test-rmse   |      Converged Time       |
| :------------------------: | :-----: | :-------: | :----------: | :-----------------------: |
|     Only Functionality     |   V3    | 129.72735 |  114.56845   | 8.66 hour / 10000 epochs  |
|       Only Proximity       |   V3    | 144.16608 |  106.26378   | 8.67 hour / 10000 epochs  |
| Only Interaction/Same-line |   V3    | 150.75353 |  110.13376   | 8.38 hour / 10000 epochs  |
|    Aggregation Together    |   V3    | 88.32695  | **94.77593** | 40.19 hour / 10004 epochs |

## Results on EV Dataset（云上运行）

|     **City: Beijing**      | Version | val-rmse |  test-rmse  |      Converged Time       |
| :------------------------: | :-----: | :------: | :---------: | :-----------------------: |
|     Only Functionality     |   V3    | 0.57105  |   0.81333   | 16.07 hour / 20000 epochs |
|       Only Proximity       |   V3    | 0.60764  |   0.83504   | 12.69 hour / 15189 epochs |
| Only Interaction/Same-line |   V3    |    -     |      -      |             -             |
|    Aggregation Together    |   V3    | 0.57685  | **0.80259** | 23.76 hour / 10497 epochs |

