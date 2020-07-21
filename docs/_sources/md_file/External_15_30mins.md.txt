# 15&30 mins External Results

## Results on Bike Dataset

注：15 mins 暂时不跑，30mins 的跑Chicago/Chengdu

### 15 mins

| **City: NYC 15 mins** | Version | test-rmse |      Converged Time      |
| :-------------------: | :-----: | :-------: | :----------------------: |
|        STMeta         |   V1    |  1.65939  | 49.28 hour / 2280 epochs |
|     STMeta-Concat     |   V1    |  1.63254  | 71.23 hour / 3326 epochs |
|      STMeta-Emb       |   V1    |           |                          |
|   STMeta-Multi-Emb    |   V1    |           |                          |
|     STMeta-Gating     |   V1    |  1.62798  | 25.35 hour / 1115 epochs |

| **City: Chicago 15 mins** | Version | test-rmse |     Converged Time      |
| :-----------------------: | :-----: | :-------: | :---------------------: |
|          STMeta           |   V1    |  1.60743  | 11.26 hour / 775 epochs |
|       STMeta-Concat       |   V1    |  1.59956  | 12.18 hour / 812 epochs |
|        STMeta-Emb         |   V1    |           |                         |
|     STMeta-Multi-Emb      |   V1    |           |                         |
|       STMeta-Gating       |   V1    |  1.60033  | 6.89 hour / 405 epochs  |

| **City: DC 15 mins** | Version | test-rmse |      Converged Time      |
| :------------------: | :-----: | :-------: | :----------------------: |
|        STMeta        |   V1    |  1.52698  | 26.81 hour / 2929 epochs |
|    STMeta-Concat     |   V1    |  1.54041  | 59.64 hour / 5149 epochs |
|      STMeta-Emb      |   V1    |           |                          |
|   STMeta-Multi-Emb   |   V1    |           |                          |
|    STMeta-Gating     |   V1    |  1.52386  | 15.97 hour / 1211 epochs |

### 30 mins

| **City: NYC 30 mins** | Version | test-rmse |      Converged Time      |
| :-------------------: | :-----: | :-------: | :----------------------: |
|        STMeta         |   V1    |  2.40976  |       6764 epochs        |
|     STMeta-Concat     |   V1    |  2.55894  | 65.41 hour / 2578 epochs |
|      STMeta-Emb       |   V1    |           |                          |
|   STMeta-Multi-Emb    |   V1    |           |                          |
|     STMeta-Gating     |   V1    |  2.47428  | 18.95 hour / 647 epochs  |

| **City: Chicago 30 mins** | Version | test-rmse |      Converged Time      |
| :-----------------------: | :-----: | :-------: | :----------------------: |
|          STMeta           |   V1    |  2.17032  |  6.67 hour / 332 epochs  |
|       STMeta-Concat       |   V1    |  2.22892  | 31.58 hour / 1822 epochs |
|        STMeta-Emb         |   V1    |           |                          |
|     STMeta-Multi-Emb      |   V1    |           |                          |
|       STMeta-Gating       |   V1    |  2.17295  |  9.93 hour / 505 epochs  |

| **City: DC 30 mins** | Version | test-rmse |      Converged Time       |
| :------------------: | :-----: | :-------: | :-----------------------: |
|        STMeta        |   V1    |  1.85628  | 192.52 hour / 4576 epochs |
|    STMeta-Concat     |   V1    |  1.88718  | 71.17 hour / 4681 epochs  |
|      STMeta-Emb      |   V1    |           |                           |
|   STMeta-Multi-Emb   |   V1    |           |                           |
|    STMeta-Gating     |   V1    |  1.86528  |  15.86 hour / 992 epoch   |
## Results on DiDi Dataset

### 15 mins

| **City: Xian 15 mins** | Version | val-rmse | test-rmse |      Converged Time      |
| :--------------------: | :-----: | :------: | :-------: | :----------------------: |
|         STMeta         |   V1    | 2.45115  |  2.65320  | 24.12 hour / 7082 epochs |
|     STMeta-Concat      |   V1    | 2.73301  |  2.69591  | 28.49 hour / 8977 epochs |
|       STMeta-Emb       |   V1    |          |           |                          |
|    STMeta-Multi-Emb    |   V1    |          |           |                          |
|     External-LSTM      |   V1    |          |           |                          |
|     STMeta-Gating      |   V1    | 2.59751  |  2.65727  | 14.29 hour / 1158 epochs |

| **City: Chengdu 15 mins** | Version | val-rmse | test-rmse |     Converged Time      |
| :-----------------------: | :-----: | :------: | :-------: | :---------------------: |
|          STMeta           |   V1    | 2.75397  |  3.24408  | 7.10 hour / 1940 epochs |
|       STMeta-Concat       |   V1    | 3.30697  |  3.31828  | 8.26 hour / 1433 epochs |
|        STMeta-Emb         |   V1    |          |           |                         |
|     STMeta-Multi-Emb      |   V1    |          |           |                         |
|       External-LSTM       |   V1    |          |           |                         |
|       STMeta-Gating       |   V1    | 3.19681  |  3.24355  | 14.80 hour / 514 epochs |

### 30 mins

| **City: Xian 30 mins** | Version | val-rmse | test-rmse |      Converged Time      |
| :--------------------: | :-----: | :------: | :-------: | :----------------------: |
|         STMeta         |   V1    | 4.00090  |  3.80812  | 16.23 hour / 9331 epochs |
|     STMeta-Concat      |   V1    | 5.06592  |  3.88665  | 15.84 hour / 9540 epochs |
|       STMeta-Emb       |   V1    |          |           |                          |
|    STMeta-Multi-Emb    |   V1    |          |           |                          |
|     External-LSTM      |   V1    |          |           |                          |
|     STMeta-Gating      |   V1    | 4.06786  |  3.83840  | 9.65 hour / 1748 epochs  |

| **City: Chengdu 30 mins** | Version | val-rmse | test-rmse |     Converged Time      |
| :-----------------------: | :-----: | :------: | :-------: | :---------------------: |
|          STMeta           |   V1    | 4.18897  |  4.64988  | 5.25 hour / 2649 epochs |
|       STMeta-Concat       |   V1    | 4.78195  |  4.75291  | 5.91 hour / 2049 epochs |
|        STMeta-Emb         |   V1    |          |           |                         |
|     STMeta-Multi-Emb      |   V1    |          |           |                         |
|       External-LSTM       |   V1    |          |           |                         |
|       STMeta-Gating       |   V1    | 4.55898  |  4.64184  | 5.93 hour / 437 epochs  |

## Results on Metro Dataset

### 15 mins

| **City: Shanghai 15 mins** | Version | val-rmse | test-rmse |      Converged Time       |
| :------------------------: | :-----: | :------: | :-------: | :-----------------------: |
|           STMeta           |   V1    | 35.83386 | 41.66834  | 87.67 hour / 20000 epochs |
|       STMeta-Concat        |   V1    | 36.28684 | 44.62159  | 41.66 hour / 10645 epochs |
|         STMeta-Emb         |   V1    |          |           |                           |
|      STMeta-Multi-Emb      |   V1    |          |           |                           |
|       External-LSTM        |   V1    |          |           |                           |
|       STMeta-Gating        |   V1    | 35.95238 | 42.11205  | 18.62 hour / 1529 epochs  |

| **City: Chongqing 15 mins** | Version | val-rmse |   test-rmse   |       Converged Time       |
| :-------------------------: | :-----: | :------: | :-----------: | :------------------------: |
|           STMeta            |   V1    | 26.21625 | **31.39239**  | 138.15 hour / 8515 epochs  |
|        STMeta-Concat        |   V1    | 30.35257 |   31.36279    | 164.13 hour / 10000 epochs |
|         STMeta-Emb          |   V1    |          |               |                            |
|      STMeta-Multi-Emb       |   V1    |          |               |                            |
|        External-LSTM        |   V1    |          |               |                            |
|        STMeta-Gating        |   V1    | 30.37934 | 31.4809276004 |  97.41 hour / 6514 epochs  |

### 30 mins

| **City: Shanghai 30 mins** | Version | val-rmse | test-rmse |      Converged Time       |
| :------------------------: | :-----: | :------: | :-------: | :-----------------------: |
|           STMeta           |   V1    | 64.99845 | 75.36282  | 39.91 hour / 20000 epochs |
|       STMeta-Concat        |   V1    | 72.80131 | 90.50749  | 26.67 hour / 12928 epochs |
|         STMeta-Emb         |   V1    |          |           |                           |
|      STMeta-Multi-Emb      |   V1    |          |           |                           |
|       External-LSTM        |   V1    |          |           |                           |
|       STMeta-Gating        |   V1    | 62.23307 | 75.05776  |  5.34 hour / 763 epochs   |

| **City: Chongqing 30 mins** | Version |   val-rmse   | test-rmse |      Converged Time       |
| :-------------------------: | :-----: | :----------: | :-------: | :-----------------------: |
|           STMeta            |   V1    |   42.03588   | 49.46800  | 84.38 hour / 10387 epochs |
|        STMeta-Concat        |   V1    |   46.38776   | 49.06065  | 74.54 hour / 10000 epochs |
|         STMeta-Emb          |   V1    |              |           |                           |
|      STMeta-Multi-Emb       |   V1    |              |           |                           |
|        External-LSTM        |   V1    |              |           |                           |
|        STMeta-Gating        |   V1    | 47.083429625 | 49.07846  |  4.82 hour / 6166 epochs  |

## Results on EV Dataset

### 30 mins

| **City: Beijing 30 mins** | Version | val-rmse | test-rmse |      Converged Time       |
| :-----------------------: | :-----: | :------: | :-------: | :-----------------------: |
|          STMeta           |   V1    | 0.46154  |  0.66985  | 16.48 hour / 4242 epochs  |
|       STMeta-Concat       |   V1    | 0.61911  |  0.65943  | 37.11 hour / 10206 epochs |
|        STMeta-Emb         |   V1    |          |           |                           |
|     STMeta-Multi-Emb      |   V1    |          |           |                           |
|       External-LSTM       |   V1    |          |           |                           |
|       STMeta-Gating       |   V1    | 0.61833  |  0.66038  | 27.23 hour / 7167 epochs  |

