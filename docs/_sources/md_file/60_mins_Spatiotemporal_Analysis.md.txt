# 60 mins Spatiotemporal Analysis

## 60 mins Single Graph

Spatial knowledge evaluation (60-minute). The base model is STMeta-DCGRU-GAL. The best result is in bold.

### Results on Bike Dataset

|       **City: NYC**        | Version | val-rmse |  test-rmse  |     Converged Time      |
| :------------------------: | :-----: | :------: | :---------: | :---------------------: |
|     Only Functionality     |   V3    | 1.93778  | **3.47656** | 8.09 hour / 5962 epochs |
|       Only Proximity       |   V3    | 1.92778  |   3.50875   | 7.42 hour / 5355 epochs |
| Only Interaction/Same-line |   V3    | 1.95641  |   3.54281   | 4.86 hour / 3671 epochs |
|    Aggregation Together    |   V3    |    -     |   3.52124   |       7438 epochs       |

|     **City: Chicago**      | Version | val-rmse |  test-rmse  |      Converged Time       |
| :------------------------: | :-----: | :------: | :---------: | :-----------------------: |
|     Only Functionality     |   V3    | 1.23264  |   2.69441   | 92.22 hour / 20000 epochs |
|       Only Proximity       |   V3    | 1.23732  |   2.71102   | 92.37 hour / 20000 epochs |
| Only Interaction/Same-line |   V3    | 1.22759  |   2.71795   | 86.25 hour / 20000 epochs |
|    Aggregation Together    |   V3    |    -     | **2.65204** |        4403 epochs        |

|        **City: DC**        |   Version    | val-rmse |  test-rmse  |      Converged Time       |
| :------------------------: | :----------: | :------: | :---------: | :-----------------------: |
|     Only Functionality     |      V3      | 1.66894  |   2.44463   | 74.57 hour / 19882 epochs |
|       Only Proximity       | patience 700 | 1.67569  |   2.44057   | 70.80 hour / 17702 epochs |
| Only Interaction/Same-line | patience 700 | 1.64630  | **2.41991** | 59.54 hour / 14425 epochs |
|    Aggregation Together    |      V3      |    -     |   2.42338   |        2993 epochs        |

### Results on DiDi Dataset

|       **City: Xian**        |   Version    | val-rmse |  test-rmse  |      Converged Time      |
| :-------------------------: | :----------: | :------: | :---------: | :----------------------: |
|     Only Functionality      |      V3      | 7.23334  |   5.80516   | 2.33 hour / 7982 epochs  |
|       Only Proximity        |      V3      | 7.07511  | **5.78975** | 6.31 hour / 46461 epochs |
| Only Interaction/Same-line  |      V3      | 7.36363  |   5.80832   | 6.35 hour / 27936 epochs |
| Aggregation Together`Check` |      V3      | 7.14426  |   5.90812   | 3.37 hour / 2393 epochs  |
|    Aggregation Together     | patience 700 | 6.97737  |   5.93810   | 6.45 hour / 4560 epochs  |
|    Aggregation Together     | patience 500 | 7.09199  |   5.81854   | 7.72 hour / 4307 epochs  |
|    Aggregation Together     |    BS 32     |  `运行`  |             |                          |

|     **City: Chengdu**      |   Version    | val-rmse |  test-rmse  |      Converged Time      |
| :------------------------: | :----------: | :------: | :---------: | :----------------------: |
|     Only Functionality     |      V3      | 6.36493  | **6.87754** | 0.69 hour / 1869 epochs  |
|       Only Proximity       |      V3      | 6.43997  |   6.91376   | 0.76 hour / 2075 epochs  |
| Only Interaction/Same-line |      V3      | 6.37446  |   6.87930   | 3.24 hour / 10274 epochs |
|    Aggregation Together    |      V3      | 6.30479  |   6.90394   | 1.76 hour / 1052 epochs  |
|    Aggregation Together    | patience 700 | 6.37813  |   6.92010   | 2.20 hour / 1105 epochs  |

### Results on Metro Dataset

|     **City: Shanghai**     | Version | val-rmse  |   test-rmse   |      Converged Time       |
| :------------------------: | :-----: | :-------: | :-----------: | :-----------------------: |
|     Only Functionality     |   V3    | 125.55458 |   148.25241   | 6.86 hour / 20000 epochs  |
|       Only Proximity       |   V3    | 127.04750 |   153.98045   | 6.77 hour / 20000 epochs  |
| Only Interaction/Same-line |   V3    | 123.43643 |   151.37936   | 7.05 hour / 20000 epochs  |
|    Aggregation Together    |   V3    | 117.82761 | **143.18166** | 30.38 hour / 20000 epochs |

|        **City: Chongqing**         | Version | val-rmse  |  test-rmse   |      Converged Time       |
| :--------------------------------: | :-----: | :-------: | :----------: | :-----------------------: |
|     Only Functionality`未收敛`     |   V3    | 129.72735 |  114.56845   | 8.66 hour / 10000 epochs  |
|       Only Proximity`未收敛`       |   V3    | 144.16608 |  106.26378   | 8.67 hour / 10000 epochs  |
| Only Interaction/Same-line`未收敛` |   V3    | 150.75353 |  110.13376   | 8.38 hour / 10000 epochs  |
|        Aggregation Together        |   V3    | 88.32695  | **94.77593** | 40.19 hour / 10004 epochs |

### Results on EV Dataset

|     **City: Beijing**      | Version | val-rmse |  test-rmse  |      Converged Time       |
| :------------------------: | :-----: | :------: | :---------: | :-----------------------: |
|     Only Functionality     |   V3    | 0.57105  |   0.81333   | 16.07 hour / 20000 epochs |
|       Only Proximity       |   V3    | 0.60764  |   0.83504   | 12.69 hour / 15189 epochs |
| Only Interaction/Same-line |   V3    |    -     |      -      |             -             |
|    Aggregation Together    |   V3    | 0.57685  | **0.80259** | 23.76 hour / 10497 epochs |

## 60 mins Temporal Abalation

Temporal abalation evaluation (60-minute). The base model is STMeta-DCGRU-GAL. The best result is in bold.

### Results on Bike Dataset

|       **City: NYC**        | Version | val-rmse |  test-rmse  |       Converged Time       |
| :------------------------: | :-----: | :------: | :---------: | :------------------------: |
|       Only Closeness       |   V3    | 2.38088  |   4.20527   | 298.35 hour / 20000 epochs |
|     Closeness & Period     |   V3    | 2.23290  |   3.63138   | 113.66 hour / 3880 epochs  |
| Closeness & Period & Trend |   V3    |    --    | **3.52124** |        7438 epochs         |

|     **City: Chicago**      | Version | val-rmse |  test-rmse  | Converged Time |
| :------------------------: | :-----: | :------: | :---------: | :------------: |
|       Only Closeness       |   V3    |          |             |                |
|     Closeness & Period     |   V3    |          |             |                |
| Closeness & Period & Trend |   V3    |    -     | **2.65204** |  4403 epochs   |

|       **City: DC **        | Version | val-rmse | test-rmse | Converged Time |
| :------------------------: | :-----: | :------: | :-------: | :------------: |
|       Only Closeness       |   V3    |          |           |                |
|     Closeness & Period     |   V3    |          |           |                |
| Closeness & Period & Trend |   V3    |    -     |  2.42338  |  2993 epochs   |

### Results on DiDi Dataset

|       **City: Xian**       |   Version    | val-rmse |  test-rmse  |      Converged Time      |
| :------------------------: | :----------: | :------: | :---------: | :----------------------: |
|       Only Closeness       |   V3    | 6.00043 | 6.77654 | 13.53 hour / 14464 epochs |
|     Closeness & Period     |   V3    | 6.13271 | 6.03849 | 12.81 hour / 7437 epochs |
| Closeness & Period & Trend | V3 patience 700 | 5.93810  | **5.81854** |  7.72 hour / 4307 epochs  |

|     **City: Chengdu**      |   Version    | val-rmse |  test-rmse  |      Converged Time      |
| :------------------------: | :----------: | :------: | :---------: | :----------------------: |
|       Only Closeness       |   V3    | 7.08731 | 8.38027 | 27.98 hour / 45576 epochs |
|     Closeness & Period     |   V3    | 7.04953 | 7.51730 | 17.40 hour / 8857 epochs |
| Closeness & Period & Trend | V3 patience 700 | **6.37813** |  **6.92010**  | 2.20 hour / 1105 epochs |

### Results on Metro Dataset

|     **City: Shanghai**     | Version | val-rmse  |   test-rmse   |      Converged Time       |
| :------------------------: | :-----: | :-------: | :----------: | :-----------------------: |
|       Only Closeness       |   V3    | 286.59168 |   328.80800   | 18.86 hour / 18891 epochs |
|     Closeness & Period     |   V3    | 105.21594 |   **140.66922**   | 37.01 hour / 20000 epochs |
| Closeness & Period & Trend |   V3    | 117.82761 | 143.18166`未完全收敛` | 30.38 hour / 20000 epochs |

|    **City: Chongqing**     | Version | val-rmse  |  test-rmse   |      Converged Time       |
| :------------------------: | :-----: | :-------: | :----------: | :-----------------------: |
|       Only Closeness       |   V3    | 129.81330 | 163.90320 | 16.70 hour / 10000 epochs |
|     Closeness & Period     |   V3    | 103.09416 |   98.78082   | 25.61 hour / 8025 epochs |
| Closeness & Period & Trend |   V3    | 88.32695 | **94.77593** | 40.19 hour / 10004 epochs |

### Results on EV Dataset

|     **City: Beijing**      | Version | val-rmse |  test-rmse  |      Converged Time       |
| :------------------------: | :-----: | :------: | :---------: | :-----------------------: |
|       Only Closeness       |   V3    | 2.33941 | 3.42340 | 0.59 hour / 75 epochs |
|     Closeness & Period     |   V3    | 0.57576 | 0.80900 | 12.81 hour / 4474 epochs |
| Closeness & Period & Trend |   V3    | 0.57685  | **0.80259** | 23.76 hour / 10497 epochs |

### Results on EV Dataset

|     **City: METR-LA**      | Version | val-rmse |  test-rmse  |     Converged Time      |
| :------------------------: | :-----: | :------: | :---------: | :---------------------: |
|       Only Closeness       |   V3    | 11.33555 |  10.67190   | 2.69 hour / 1785 epochs |
|     Closeness & Period     |   V3    | 10.66494 |  10.11732   | 2.97 hour / 1475 epochs |
| Closeness & Period & Trend |   V3    | 6.33248  | **8.99345** | 0.80 hour / 2387 epochs |