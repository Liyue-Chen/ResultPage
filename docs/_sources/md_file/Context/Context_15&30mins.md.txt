# 15&30 mins External Results

## Results on Bike Dataset

注：15 mins 暂时不跑，30mins 的跑Chicago/Chengdu/Shanghai/Beijing

### 15 mins

| **City: NYC 15 mins**  | Version | test-rmse |      Converged Time      |
| :--------------------: | :-----: | :-------: | :----------------------: |
|         STMeta         |   V1    |  1.65939  | 49.28 hour / 2280 epochs |
|   STMeta-Raw-Concat    |   V1    |  1.63254  | 71.23 hour / 3326 epochs |
|   STMeta-Emb-Concat    |   V1    |           |                          |
| STMeta-MultiEmb-Concat |   V1    |           |                          |
|   STMeta-Raw-Gating    |   V1    |  1.62798  | 25.35 hour / 1115 epochs |

| **City: Chicago 15 mins** | Version | test-rmse |     Converged Time      |
| :-----------------------: | :-----: | :-------: | :---------------------: |
|          STMeta           |   V1    |  1.60743  | 11.26 hour / 775 epochs |
|     STMeta-Raw-Concat     |   V1    |  1.59956  | 12.18 hour / 812 epochs |
|     STMeta-Emb-Concat     |   V1    |           |                         |
|  STMeta-MultiEmb-Concat   |   V1    |           |                         |
|     STMeta-Raw-Gating     |   V1    |  1.60033  | 6.89 hour / 405 epochs  |

|  **City: DC 15 mins**  | Version | test-rmse |      Converged Time      |
| :--------------------: | :-----: | :-------: | :----------------------: |
|         STMeta         |   V1    |  1.52698  | 26.81 hour / 2929 epochs |
|   STMeta-Raw-Concat    |   V1    |  1.54041  | 59.64 hour / 5149 epochs |
|   STMeta-Emb-Concat    |   V1    |           |                          |
| STMeta-MultiEmb-Concat |   V1    |           |                          |
|   STMeta-Raw-Gating    |   V1    |  1.52386  | 15.97 hour / 1211 epochs |

### 30 mins

| **City: NYC 30 mins**  | Version | test-rmse |      Converged Time      |
| :--------------------: | :-----: | :-------: | :----------------------: |
|         STMeta         |   V1    |  2.40976  |       6764 epochs        |
|   STMeta-Raw-Concat    |   V1    |  2.55894  | 65.41 hour / 2578 epochs |
|   STMeta-Emb-Concat    |   V1    |           |                          |
| STMeta-MultiEmb-Concat |   V1    |           |                          |
|   STMeta-Raw-Gating    |   V1    |  2.47428  | 18.95 hour / 647 epochs  |

| **City: Chicago 30 mins** | Version |  test-rmse  |      Converged Time      |
| :-----------------------: | :-----: | :---------: | :----------------------: |
|          STMeta           |   V1    |   2.17036   |  6.24 hour / 282 epochs  |
|       STMeta-Raw-Concat       |   V1    |   2.22892   | 31.58 hour / 1822 epochs |
|     STMeta-Emb-Concat     |   V1    |   2.19917   | 24.60 hour / 1429 epochs |
|  STMeta-MultiEmb-Concat   |   V1    |   2.13325   | 15.22 hour / 836 epochs  |
|        STMeta-Raw-Add     |   V1    |   2.20548   | 22.47 hour / 1291 epochs |
|      STMeta-LSTM-Add      |   V1    | **2.10940** |  8.18 hour / 388 epochs  |
|       STMeta-Raw-Gating       |   V1    |   2.17295   |  9.93 hour / 505 epochs  |
|     STMeta-Emb-Add     |   V1    |             |                           |
|   STMeta-Emb-Gating    |   V1    |      |  |
|  STMeta-MultiEmb-Add   |   V1    |             |                           |
| STMeta-MultiEmb-Gating |   V1    |      |  |
|   STMeta-LSTM-Concat   |   V1    |      |   |
|   STMeta-LSTM-Gating   |   V1    |      |  |

|  **City: DC 30 mins**  | Version | test-rmse |      Converged Time       |
| :--------------------: | :-----: | :-------: | :-----------------------: |
|         STMeta         |   V1    |  1.85628  | 192.52 hour / 4576 epochs |
|   STMeta-Raw-Concat    |   V1    |  1.88718  | 71.17 hour / 4681 epochs  |
|   STMeta-Emb-Concat    |   V1    |           |                           |
| STMeta-MultiEmb-Concat |   V1    |           |                           |
|   STMeta-Raw-Gating    |   V1    |  1.86528  |  15.86 hour / 992 epoch   |
## Results on DiDi Dataset

### 15 mins

| **City: Xian 15 mins** | Version | val-rmse | test-rmse |      Converged Time      |
| :--------------------: | :-----: | :------: | :-------: | :----------------------: |
|         STMeta         |   V1    | 2.45115  |  2.65320  | 24.12 hour / 7082 epochs |
|   STMeta-Raw-Concat    |   V1    | 2.73301  |  2.69591  | 28.49 hour / 8977 epochs |
|   STMeta-Emb-Concat    |   V1    |          |           |                          |
| STMeta-MultiEmb-Concat |   V1    |          |           |                          |
|    STMeta-LSTM-Add     |   V1    |          |           |                          |
|   STMeta-Raw-Gating    |   V1    | 2.59751  |  2.65727  | 14.29 hour / 1158 epochs |

| **City: Chengdu 15 mins** | Version | val-rmse | test-rmse |     Converged Time      |
| :-----------------------: | :-----: | :------: | :-------: | :---------------------: |
|          STMeta           |   V1    | 2.75397  |  3.24408  | 7.10 hour / 1940 epochs |
|     STMeta-Raw-Concat     |   V1    | 3.30697  |  3.31828  | 8.26 hour / 1433 epochs |
|     STMeta-Emb-Concat     |   V1    |          |           |                         |
|  STMeta-MultiEmb-Concat   |   V1    |          |           |                         |
|      STMeta-LSTM-Add      |   V1    |          |           |                         |
|     STMeta-Raw-Gating     |   V1    | 3.19681  |  3.24355  | 14.80 hour / 514 epochs |

### 30 mins

| **City: Xian 30 mins** | Version | val-rmse | test-rmse |      Converged Time      |
| :--------------------: | :-----: | :------: | :-------: | :----------------------: |
|         STMeta         |   V1    | 4.36484  |  3.79985  | 2.92 hour / 1308 epochs  |
|   STMeta-Raw-Concat |   V1    | 4.18382  |  3.90704  | 15.14 hour / 8650 epochs |
|   STMeta-Emb-Concat    |   V1    | 4.17580  |  3.79393  | 5.76 hour / 2998 epochs  |
| STMeta-MultiEmb-Concat |   V1    | 4.18736  |  3.85414  | 2.86 hour / 1172 epochs  |
|       STMeta-Raw-Add       |   V1    | 10.49953 |  3.90578  | 4.18 hour / 1882 epochs  |
|     STMeta-LSTM-Add    |   V1    | 4.11285  |  3.76667  | 7.82 hour / 3371 epochs  |
|     STMeta-Raw-Gating  |   V1    | 4.01627  |  3.82246  | 4.02 hour / 2040 epochs  |
|     STMeta-Emb-Add     |   V1    |             |                           ||
|   STMeta-Emb-Gating    |   V1    |      |  ||
|  STMeta-MultiEmb-Add   |   V1    |             |                           ||
| STMeta-MultiEmb-Gating |   V1    |      |  ||
|   STMeta-LSTM-Concat   |   V1    |      |   ||
|   STMeta-LSTM-Gating   |   V1    |      |  ||

| **City: Chengdu 30 mins** | Version | val-rmse | test-rmse |      Converged Time      |
| :-----------------------: | :-----: | :------: | :-------: | :----------------------: |
|          STMeta           |   V1    | 4.18897  |  4.64988  | 5.25 hour / 2649 epochs  |
|       STMeta-Raw-Concat       |   V1    | 4.78195  |  4.75291  | 5.91 hour / 2049 epochs  |
|     STMeta-Emb-Concat     |   V1    | 4.62221  |  4.69700  | 3.64 hour / 1258 epochs  |
|  STMeta-MultiEmb-Concat   |   V1    | 4.73740  |  4.75409  | 12.78 hour / 5636 epochs |
|        STMeta-Raw-Add     |   V1    | 4.81093  |  4.89697  | 9.55 hour / 4434 epochs  |
|       STMeta-LSTM-Add       |   V1    | 4.61116  |  4.68287  |  2.87 hour / 664 epochs  |
|       STMeta-Raw-Gating       |   V1    | 4.55898  |  4.64184  |  5.93 hour / 437 epochs  |
|     STMeta-Emb-Add     |   V1    |             |                           ||
|   STMeta-Emb-Gating    |   V1    |      |  ||
|  STMeta-MultiEmb-Add   |   V1    |             |                           ||
| STMeta-MultiEmb-Gating |   V1    |      |  ||
|   STMeta-LSTM-Concat   |   V1    |      |   ||
|   STMeta-LSTM-Gating   |   V1    |      |  ||

## Results on Metro Dataset

### 15 mins

| **City: Shanghai 15 mins** | Version | val-rmse | test-rmse |      Converged Time       |
| :------------------------: | :-----: | :------: | :-------: | :-----------------------: |
|           STMeta           |   V1    | 35.83386 | 41.66834  | 87.67 hour / 20000 epochs |
|     STMeta-Raw-Concat      |   V1    | 36.28684 | 44.62159  | 41.66 hour / 10645 epochs |
|     STMeta-Emb-Concat      |   V1    |          |           |                           |
|   STMeta-MultiEmb-Concat   |   V1    |          |           |                           |
|      STMeta-LSTM-Add       |   V1    |          |           |                           |
|     STMeta-Raw-Gating      |   V1    | 35.95238 | 42.11205  | 18.62 hour / 1529 epochs  |

| **City: Chongqing 15 mins** | Version | val-rmse |   test-rmse   |       Converged Time       |
| :-------------------------: | :-----: | :------: | :-----------: | :------------------------: |
|           STMeta            |   V1    | 26.21625 | **31.39239**  | 138.15 hour / 8515 epochs  |
|      STMeta-Raw-Concat      |   V1    | 30.35257 |   31.36279    | 164.13 hour / 10000 epochs |
|      STMeta-Emb-Concat      |   V1    |          |               |                            |
|   STMeta-MultiEmb-Concat    |   V1    |          |               |                            |
|       STMeta-LSTM-Add       |   V1    |          |               |                            |
|      STMeta-Raw-Gating      |   V1    | 30.37934 | 31.4809276004 |  97.41 hour / 6514 epochs  |

### 30 mins

| **City: Shanghai 30 mins** | Version | val-rmse |  test-rmse   |      Converged Time       |
| :------------------------: | :-----: | :------: | :----------: | :-----------------------: |
|           STMeta           |   V1    | 62.62244 |   78.23737   |  7.01 hour / 2702 epochs  |
|       STMeta-Raw-Concat |   V1    | 72.80131 |   90.50749   | 26.67 hour / 12928 epochs |
|     STMeta-Emb-Concat      |   V1    | 65.11606 |   77.34818   |  8.98 hour / 1008 epochs  |
|   STMeta-MultiEmb-Concat   |   V1    | 68.61551 |   78.90988   | 10.14 hour / 3672 epochs  |
|         STMeta-Raw-Add         |   V1    | 65.91428 |   84.62997   | 16.86 hour / 6342 epochs  |
|       STMeta-LSTM-Add      |   V1    | 61.71616 |   76.96026   | 11.83 hour / 4521 epochs  |
|       STMeta-Raw-Gating    |   V1    | 62.23307 | **75.05776** |  5.34 hour / 763 epochs   |
|     STMeta-Emb-Add     |   V1    |             |                           ||
|   STMeta-Emb-Gating    |   V1    |      |  ||
|  STMeta-MultiEmb-Add   |   V1    |             |                           ||
| STMeta-MultiEmb-Gating |   V1    |      |  ||
|   STMeta-LSTM-Concat   |   V1    |      |   ||
|   STMeta-LSTM-Gating   |   V1    |      |  ||

| **City: Chongqing 30 mins** | Version |   val-rmse   | test-rmse |      Converged Time       |
| :-------------------------: | :-----: | :----------: | :-------: | :-----------------------: |
|           STMeta            |   V1    |   42.03588   | 49.46800  | 84.38 hour / 10387 epochs |
|        STMeta-Raw-Concat        |   V1    |   46.38776   | 49.06065  | 74.54 hour / 10000 epochs |
|      STMeta-Emb-Concat      |   V1    |              |           |                           |
|   STMeta-MultiEmb-Concat    |   V1    |              |           |                           |
|        STMeta-LSTM-Add        |   V1    |              |           |                           |
|        STMeta-Raw-Gating        |   V1    | 47.083429625 | 49.07846  |  4.82 hour / 6166 epochs  |
|     STMeta-Emb-Add     |   V1    |             |                           ||
|   STMeta-Emb-Gating    |   V1    |      |  ||
|  STMeta-MultiEmb-Add   |   V1    |             |                           ||
| STMeta-MultiEmb-Gating |   V1    |      |  ||
|   STMeta-LSTM-Concat   |   V1    |      |   ||
|   STMeta-LSTM-Gating   |   V1    |      |  ||

## Results on EV Dataset

### 30 mins

| **City: Beijing 30 mins** | Version | val-rmse |  test-rmse  |      Converged Time       |
| :-----------------------: | :-----: | :------: | :---------: | :-----------------------: |
|          STMeta           |   V1    | 0.63202  |   0.66399   | 32.46 hour / 10000 epochs |
|       STMeta-Raw-Concat       |   V1    | 0.61911  |   0.65943   | 37.11 hour / 10206 epochs |
|     STMeta-Emb-Concat     |   V1    | 0.61829  | **0.65479** | 21.51 hour / 5783 epochs  |
|  STMeta-MultiEmb-Concat   |   V1    | 0.62408  |   0.72312   | 24.78 hour / 6663 epochs  |
|        STMeta-Raw-Add     |   V1    | 0.62057  |   0.68033   | 22.28 hour / 6011 epochs  |
|       STMeta-LSTM-Add       |   V1    | 0.62471  |   0.66289   | 13.86 hour / 3591 epochs  |
|       STMeta-Raw-Gating       |   V1    | 0.61833  |   0.66038   | 27.23 hour / 7167 epochs  |
|     STMeta-Emb-Add     |   V1    |             |                           ||
|   STMeta-Emb-Gating    |   V1    |      |  ||
|  STMeta-MultiEmb-Add   |   V1    |             |                           ||
| STMeta-MultiEmb-Gating |   V1    |      |  ||
|   STMeta-LSTM-Concat   |   V1    |      |   ||
|   STMeta-LSTM-Gating   |   V1    |      |  ||

