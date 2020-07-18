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

|  **City: Xian**  |      Version      | val-rmse | test-rmse | Converged Time |
| :--------------: | :---------------: | :------: | :-------: | :------------: |
|      STMeta      |        V1         |          |           |                |
|  STMeta-Concat   |        V1         |          |           |                |
|    STMeta-Emb    | V1（bs:8 ,emb:6） |          |           |                |
| STMeta-Multi-Emb |        V1         |          |           |                |
|   STMeta-LSTM    |        V1         |          |           |                |
|  STMeta-Gating   |        V1         |          |           |                |

| **City: Chengdu** | Version | val-rmse | test-rmse | Converged Time |
| :---------------: | :-----: | :------: | :-------: | :------------: |
|      STMeta       |   V1    |          |           |                |
|   STMeta-Concat   |   V1    |          |           |                |
|    STMeta-Emb     |   V1    |          |           |                |
| STMeta-Multi-Emb  |   V1    |          |           |                |
|    STMeta-LSTM    |   V1    |          |           |                |
|   STMeta-Gating   |   V1    |          |           |                |



## Results on Metro Dataset

| **City: Shanghai** |      Version       | val-rmse | test-rmse | Converged Time |
| :----------------: | :----------------: | :------: | :-------: | :------------: |
|       STMeta       |         V1         |          |           |                |
|   STMeta-Concat    |     V1（bs:8）     |          |           |                |
|     STMeta-Emb     | V1（bs:8,emb:10）  |          |           |                |
|  STMeta-Multi-Emb  |     V1(10-1-6)     |          |           |                |
|    STMeta-LSTM     | V1(batch_size:64)  |          |           |                |
|   STMeta-Gating    | V1（bs:8 lr:5e-5） |          |           |                |

| **City: Chongqing** | Version | val-rmse | test-rmse | Converged Time |
| :-----------------: | :-----: | :------: | :-------: | :------------: |
|       STMeta        |   V1    |          |           |                |
|    STMeta-Concat    |   V1    |          |           |                |
|     STMeta-Emb      |   V1    |          |           |                |
|  STMeta-Multi-Emb   |   V1    |          |           |                |
|     STMeta-LSTM     |   V1    |          |           |                |
|    STMeta-Gating    |   V1    |          |           |                |



## Results on EV Dataset

| **City: Beijing** |   Version   | val-rmse | test-rmse | Converged Time |
| :---------------: | :---------: | :------: | :-------: | :------------: |
|      STMeta       | V1（bs:64） |          |           |                |
|   STMeta-Concat   | V1（bs:32） |          |           |                |
|    STMeta-Emb     |     V1      |          |           |                |
| STMeta-Multi-Emb  |     V1      |          |           |                |
|    STMeta-LSTM    | V1（bs:16） |          |           |                |
|   STMeta-Gating   | V1（bs:32） |          |           |                |

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