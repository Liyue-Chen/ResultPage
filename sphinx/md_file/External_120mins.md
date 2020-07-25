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

| **City: Chicago** | Version | val-rmse | test-rmse |      Converged Time       |
| :---------------: | :-----: | :------: | :-------: | :-----------------------: |
|      STMeta       |   V1    | 3.08181  |  3.82970  | 86.84 hour / 10000 epochs |
|   STMeta-Concat   |   V1    | 2.87774  |  3.83360  | 88.61 hour / 9978 epochs  |
|    STMeta-Emb     |   V1    |          |           |                           |
| STMeta-Multi-Emb  |   V1    |          |           |                           |
|    STMeta-Add     |   V1    |          |           |                           |
|    STMeta-LSTM    |   V1    |          |           |                           |
|   STMeta-Gating   |   V1    |          |           |                           |

|   **City: DC**   | Version | test-rmse |      Converged Time      |
| :--------------: | :-----: | :-------: | :----------------------: |
|      STMeta      |   V1    |  3.33518  | 56.03 hour / 7718 epochs |
|  STMeta-Concat   |   V1    |  3.33535  | 46.25 hour / 6334 epochs |
|    STMeta-Emb    |   V1    |           |                          |
| STMeta-Multi-Emb |   V1    |           |                          |
|  STMeta-Gating   |   V1    |  3.30508  | 22.60 hour / 2969 epochs |

## Results on DiDi Dataset

|  **City: Xian**  |      Version      | val-rmse | test-rmse |      Converged Time      |
| :--------------: | :---------------: | :------: | :-------: | :----------------------: |
|      STMeta      |        V1         | 13.50252 |  9.44800  | 8.33 hour / 14016 epochs |
|  STMeta-Concat   |        V1         | 28.22483 |  9.28606  | 3.43 hour / 5509 epochs  |
|    STMeta-Emb    | V1（bs:8, emb:6） |          |           |                          |
| STMeta-Multi-Emb |        V1         |          |           |                          |
|   STMeta-LSTM    |        V1         |          |           |                          |
|  STMeta-Gating   |        V1         | 12.46816 |  9.99302  | 2.73 hour / 1491 epochs  |

| **City: Chengdu** | Version | val-rmse | test-rmse |     Converged Time      |
| :---------------: | :-----: | :------: | :-------: | :---------------------: |
|      STMeta       |   V1    | 10.72980 | 10.76993  | 0.81 hour / 697 epochs  |
|   STMeta-Concat   |   V1    | 13.45980 | 13.39585  | 2.84 hour / 4146 epochs |
|    STMeta-Emb     |   V1    |          |           |                         |
| STMeta-Multi-Emb  |   V1    |          |           |                         |
|    STMeta-LSTM    |   V1    |          |           |                         |
|   STMeta-Gating   |   V1    | 10.69218 | 10.87996  | 1.71 hour / 949 epochs  |



## Results on Metro Dataset

| **City: Shanghai** |      Version       | val-rmse  | test-rmse |     Converged Time      |
| :----------------: | :----------------: | :-------: | :-------: | :---------------------: |
|       STMeta       |         V1         | 182.82380 | 339.61798 | 4.74 hour / 6271 epochs |
|   STMeta-Concat    |         V1         | 346.38525 | 544.8269  | 3.86 hour / 5404 epochs |
|     STMeta-Emb     |         V1         |           |           |                         |
|  STMeta-Multi-Emb  |     V1(10-1-6)     |           |           |                         |
|    STMeta-LSTM     |         V1         |           |           |                         |
|   STMeta-Gating    | V1（bs:8 lr:5e-5） | 188.71114 | 344.93225 | 0.99 hour / 504 epochs  |

| **City: Chongqing** | Version | val-rmse  | test-rmse |      Converged Time       |
| :-----------------: | :-----: | :-------: | :-------: | :-----------------------: |
|       STMeta        |   V1    | 285.77374 | 233.04099 |  6.39 hour / 2853 epochs  |
|    STMeta-Concat    |   V1    | 211.15181 | 218.11572 | 20.86 hour / 10000 epochs |
|     STMeta-Emb      |   V1    |           |           |                           |
|  STMeta-Multi-Emb   |   V1    |           |           |                           |
|     STMeta-LSTM     |   V1    |           |           |                           |
|    STMeta-Gating    |   V1    | 198.58571 | 200.45142 | 21.21 hour / 10000 epochs |



## Results on EV Dataset

| **City: Beijing** | Version | val-rmse | test-rmse |      Converged Time       |
| :---------------: | :-----: | :------: | :-------: | :-----------------------: |
|      STMeta       |   V1    | 0.95491  |  0.95504  |  3.99 hour / 3778 epochs  |
|   STMeta-Concat   |   V1    | 0.90407  |  0.95509  |  7.94 hour / 7838 epochs  |
|    STMeta-Emb     |   V1    |          |           |                           |
| STMeta-Multi-Emb  |   V1    |          |           |                           |
|    STMeta-LSTM    |   V1    |          |           |                           |
|   STMeta-Gating   |   V1    | 0.87558  |  0.90612  | 12.07 hour / 11702 epochs |

默认bs:64 

