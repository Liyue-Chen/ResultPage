# 120 mins External Results

## Results on Bike Dataset

|  **City: NYC**   | Version | test-rmse | Converged Time |
| :--------------: | :-----: | :-------: | :------------: |
|      STMeta      |   V1    |           |                |
|  STMeta-Concat   |   V1    |           |                |
|    STMeta-Emb    |   V1    |           |                |
| STMeta-Multi-Emb |   V1    |           |                |
|   STMeta-LSTM    |         |           |                |
|  STMeta-Gating   |   V1    |           |                |

| **City: Chicago** | Version | test-rmse | Converged Time |
| :---------------: | :-----: | :-------: | :------------: |
|      STMeta       |   V1    |           |                |
|   STMeta-Concat   |   V1    |           |                |
|    STMeta-Emb     |   V1    |           |                |
| STMeta-Multi-Emb  |   V1    |           |                |
|   STMeta-Gating   |   V1    |           |                |

|   **City: DC**   | Version | test-rmse | Converged Time |
| :--------------: | :-----: | :-------: | :------------: |
|      STMeta      |   V1    |           |                |
|  STMeta-Concat   |   V1    |           |                |
|    STMeta-Emb    |   V1    |           |                |
| STMeta-Multi-Emb |   V1    |           |                |
|  STMeta-Gating   |   V1    |           |                |

## Results on DiDi Dataset

|  **City: Xian**  |      Version      | val-rmse  | test-rmse |      Converged Time      |
| :--------------: | :---------------: | :-------: | :-------: | :----------------------: |
|      STMeta      |        V1         | 13.502524 | 9.447995  | 8.33 hour / 14016 epochs |
|  STMeta-Concat   |        V1         | 28.22483  | 9.286061  | 3.43 hour / 5509 epochs  |
|    STMeta-Emb    | V1（bs:8 ,emb:6） |           |           |                          |
| STMeta-Multi-Emb |        V1         |           |           |                          |
|   STMeta-LSTM    |        V1         |           |           |                          |
|  STMeta-Gating   |        V1         | 12.468161 | 9.993015  | 2.73 hour / 1491 epochs  |

| **City: Chengdu** | Version | val-rmse  | test-rmse |     Converged Time      |
| :---------------: | :-----: | :-------: | :-------: | :---------------------: |
|      STMeta       |   V1    | 10.729795 | 10.769929 | 0.81 hour / 697 epochs  |
|   STMeta-Concat   |   V1    | 13.459796 | 13.395845 | 2.84 hour / 4146 epochs |
|    STMeta-Emb     |   V1    |           |           |                         |
| STMeta-Multi-Emb  |   V1    |           |           |                         |
|    STMeta-LSTM    |   V1    |           |           |                         |
|   STMeta-Gating   |   V1    | 10.692179 | 10.87996  | 1.71 hour / 949 epochs  |



## Results on Metro Dataset

| **City: Shanghai** |      Version       | val-rmse  | test-rmse |     Converged Time      |
| :----------------: | :----------------: | :-------: | :-------: | :---------------------: |
|       STMeta       |         V1         | 182.8238  | 339.61798 | 4.74 hour / 6271 epochs |
|   STMeta-Concat    |     V1（bs:8）     | 346.38525 | 544.8269  | 3.86 hour / 5404 epochs |
|     STMeta-Emb     | V1（bs:8,emb:10）  |           |           |                         |
|  STMeta-Multi-Emb  |     V1(10-1-6)     |           |           |                         |
|    STMeta-LSTM     | V1(batch_size:64)  |           |           |                         |
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

| **City: Beijing** | Version |  val-rmse  | test-rmse  |      Converged Time       |
| :---------------: | :-----: | :--------: | :--------: | :-----------------------: |
|      STMeta       |   V1    | 0.95491284 | 0.9550355  |  3.99 hour / 3778 epochs  |
|   STMeta-Concat   |   V1    | 0.9040738  | 0.95508784 |  7.94 hour / 7838 epochs  |
|    STMeta-Emb     |   V1    |            |            |                           |
| STMeta-Multi-Emb  |   V1    |            |            |                           |
|    STMeta-LSTM    |   V1    |            |            |                           |
|   STMeta-Gating   |   V1    | 0.8755816  | 0.90612376 | 12.07 hour / 11702 epochs |

默认bs:64 

## LSTM Windows Size

| **City: Xian** | window size | val-rmse | test-rmse | Converged Time |
| :------------: | :---------: | :------: | :-------: | :------------: |
|     STMeta     |      -      |          |           |                |
| STMeta-Gating  |      -      |          |           |                |
|  STMeta-LSTM   |      4      |          |           |                |
|  STMeta-LSTM   |      6      |          |           |                |
|  STMeta-LSTM   |      8      |          |           |                |



| **City: Beijing** | window size | val-rmse | test-rmse | Converged Time |
| :---------------: | :---------: | :------: | :-------: | :------------: |
|      STMeta       |      -      |          |           |                |
|   STMeta-Gating   |      -      |          |           |                |
|    STMeta-LSTM    |      4      |          |           |                |
|    STMeta-LSTM    |      6      |          |           |                |
|    STMeta-LSTM    |      8      |          |           |                |