# 120 mins External Results

注：120 mins 跑Chicago/Chengdu/Shanghai/Beijing

## Results on Bike Dataset

|  **City: NYC**   | Version | val-rmse | test-rmse |       Converged Time       |
| :--------------: | :-----: | :------: | :-------: | :------------------------: |
|      STMeta      |   V1    | 5.01944  |  5.23612  | 138.05 hour / 10000 epochs |
|  STMeta-Concat   |   V1    |          |           |                            |
|    STMeta-Emb    |   V1    |          |           |                            |
| STMeta-Multi-Emb |   V1    |          |           |                            |
|    STMeta-Add    |         |          |           |                            |
|   STMeta-LSTM    |         |          |           |                            |
|  STMeta-Gating   |   V1    |          |           |                            |

| **City: Chicago** | Version | val-rmse |  test-rmse  |      Converged Time       |
| :---------------: | :-----: | :------: | :---------: | :-----------------------: |
|      STMeta       |   V1    | 3.08181  |   3.82970   | 86.84 hour / 10000 epochs |
|   STMeta-Concat   |   V1    | 2.87774  |   3.83360   | 88.61 hour / 9978 epochs  |
|    STMeta-Emb     |   V1    | 2.98297  |   3.83958   | 50.20 hour / 5610 epochs  |
| STMeta-Multi-Emb  |   V1    | 2.81446  |   3.80049   | 87.35 hour / 10000 epochs |
|    STMeta-Add     |   V1    | 2.88667  |   3.79740   | 48.57 hour / 5471 epochs  |
|    STMeta-LSTM    |   V1    | 2.79867  | **3.69101** | 54.46 hour / 5771 epochs  |
|   STMeta-Gating   |   V1    | 2.85412  |   3.74107   | 66.16 hour / 7660 epochs  |

|   **City: DC**   | Version | test-rmse |      Converged Time      |
| :--------------: | :-----: | :-------: | :----------------------: |
|      STMeta      |   V1    |  3.33518  | 56.03 hour / 7718 epochs |
|  STMeta-Concat   |   V1    |  3.33535  | 46.25 hour / 6334 epochs |
|    STMeta-Emb    |   V1    |           |                          |
| STMeta-Multi-Emb |   V1    |           |                          |
|    STMeta-Add    |   V1    |           |                          |
|   STMeta-LSTM    |   V1    |           |                          |
|  STMeta-Gating   |   V1    |  3.30508  | 22.60 hour / 2969 epochs |

## Results on DiDi Dataset

|  **City: Xian**  |      Version      | val-rmse | test-rmse |      Converged Time      |
| :--------------: | :---------------: | :------: | :-------: | :----------------------: |
|      STMeta      |        V1         | 13.50252 |  9.44800  | 8.33 hour / 14016 epochs |
|  STMeta-Concat   |        V1         | 28.22483 |  9.28606  | 3.43 hour / 5509 epochs  |
|    STMeta-Emb    | V1（bs:8, emb:6） | 12.13475 |  9.33355  | 2.88 hour / 4336 epochs  |
| STMeta-Multi-Emb |        V1         | 12.62340 |  9.63350  | 2.34 hour / 3736 epochs  |
|    STMeta-Add    |        V1         | 56.90548 | 12.29506  |  1.71 hour / 850 epochs  |
|   STMeta-LSTM    |        V1         | 12.39611 |  9.37409  | 8.01 hour / 14829 epochs |
|  STMeta-Gating   |        V1         | 12.46816 |  9.99302  | 2.73 hour / 1491 epochs  |

| **City: Chengdu** | Version | val-rmse | test-rmse |     Converged Time      |
| :---------------: | :-----: | :------: | :-------: | :---------------------: |
|      STMeta       |   V1    | 10.72980 | 10.76993  | 0.81 hour / 697 epochs  |
|   STMeta-Concat   |   V1    | 13.45980 | 13.39585  | 2.84 hour / 4146 epochs |
|    STMeta-Emb     |   V1    | 11.26255 | 11.10817  | 1.74 hour / 2490 epochs |
| STMeta-Multi-Emb  |   V1    | 11.41368 | 11.36948  | 2.78 hour / 4291 epochs |
|    STMeta-Add     |   V1    | 11.32658 | 12.04818  | 1.40 hour / 1929 epochs |
|    STMeta-LSTM    |   V1    | 10.89169 | 11.14222  | 1.32 hour / 1639 epochs |
|   STMeta-Gating   |   V1    | 10.69218 | 10.87996  | 1.71 hour / 949 epochs  |



## Results on Metro Dataset

| **City: Shanghai** |  Version   | val-rmse  |   test-rmse   |     Converged Time      |
| :----------------: | :--------: | :-------: | :-----------: | :---------------------: |
|       STMeta       |     V1     | 182.82380 |   339.61798   | 4.74 hour / 6271 epochs |
|   STMeta-Concat    |     V1     | 357.76083 |   456.72226   | 6.15 hour / 9334 epochs |
|     STMeta-Emb     |     V1     | 191.13057 |   375.82062   |       1754 epochs       |
|  STMeta-Multi-Emb  | V1(10-1-6) | 190.68219 |   343.36005   | 2.33 hour / 2562 epochs |
|     STMeta-Add     |            | 253.07149 | **330.59137** |       6977 epochs       |
|    STMeta-LSTM     |     V1     | 190.68219 |   343.36005   | 2.33 hour / 2562 epochs |
|   STMeta-Gating    |     V1     | 189.36467 | **321.42722** | 2.87 hour / 2349 epochs |

| **City: Chongqing** | Version | val-rmse  | test-rmse |      Converged Time       |
| :-----------------: | :-----: | :-------: | :-------: | :-----------------------: |
|       STMeta        |   V1    | 285.77374 | 233.04099 |  6.39 hour / 2853 epochs  |
|    STMeta-Concat    |   V1    | 211.15181 | 218.11572 | 20.86 hour / 10000 epochs |
|     STMeta-Emb      |   V1    |           |           |                           |
|  STMeta-Multi-Emb   |   V1    |           |           |                           |
|     STMeta-Add      |         |           |           |                           |
|     STMeta-LSTM     |   V1    |           |           |                           |
|    STMeta-Gating    |   V1    | 198.58571 | 200.45142 | 21.21 hour / 10000 epochs |



## Results on EV Dataset

| **City: Beijing** | Version | val-rmse | test-rmse |      Converged Time       |
| :---------------: | :-----: | :------: | :-------: | :-----------------------: |
|      STMeta       |   V1    | 0.95491  |  0.95504  |  3.99 hour / 3778 epochs  |
|   STMeta-Concat   |   V1    | 0.90407  |  0.95509  |  7.94 hour / 7838 epochs  |
|    STMeta-Emb     |   V1    | 0.85593  |  0.89916  | 9.95 hour / 10000 epochs  |
| STMeta-Multi-Emb  |   V1    | 0.90135  |  0.92913  |  8.84 hour / 8949 epochs  |
|    STMeta-Add     |   V1    | 0.92325  |  1.04500  |  3.83 hour / 3866 epochs  |
|    STMeta-LSTM    |   V1    | 0.87795  |  0.88907  | 10.17 hour / 9802 epochs  |
|   STMeta-Gating   |   V1    | 0.87558  |  0.90612  | 12.07 hour / 11702 epochs |

默认bs:64 

