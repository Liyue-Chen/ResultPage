# 60 mins External Results

#### 一些经验

1.虽然小batch_size容易抖动，但速度快，效果甚至更好，尽量不要实验太大的batch，如64。

2.可以先用大lr，小batch，训练至快收敛，然后换小lr，大batch。

## Results on Bike Dataset

|     **City: NYC**      | Version |  test-rmse  |       Converged Time       |
| :--------------------: | :-----: | :---------: | :------------------------: |
|         STMeta         |   V1    |   3.60479   |  74.15 hour / 2307 epochs  |
|     STMeta-Concat      |   V1    | **3.37618** | 144.60 hour / 5362 epochs  |
|   STMeta-Emb-Concat    |   V1    |   3.38310   | 127.81 hour / 4876 epochs  |
| STMeta-MultiEmb-Concat |   V1    |   3.38418   | 153.24 hour / 4638 epochs  |
|       STMeta-Add       |   V1    |   3.40535   | 223.17 hour / 9094 epochs  |
|    STMeta-LSTM-Add     |   V1    |   3.39712   |  65.97 hour / 2578 epochs  |
|     STMeta-Gating      |   V1    | **3.37795** | 120.89 hour / 4043 epochs  |
|     STMeta-Emb-Add     |   V1    |  3.4132757  | 244.73 hour / 10000 epochs |
|   STMeta-Emb-Gating    |   V1    |   3.41039   | 134.83 hour / 5460 epochs  |
|  STMeta-MultiEmb-Add   |   V1    | 3.45203434  | 164.15 hour / 6655 epochs  |
| STMeta-MultiEmb-Gating |   V1    |   3.39172   | 170.83 hour / 6897 epochs  |
|   STMeta-LSTM-Concat   |   V1    |   3.39019   |  89.02 hour / 3580 epochs  |
|   STMeta-LSTM-Gating   |   V1    | **3.36740** | 142.84 hour / 5840 epochs  |

| **City: Chicago** | Version |  test-rmse  |      Converged Time       |
| :---------------: | :-----: | :---------: | :-----------------------: |
|      STMeta       |   V1    |   2.73998   | 22.00 hour / 1430 epochs  |
|   STMeta-Concat   |   V1    |   2.66504   | 165.83 hour / 9360 epochs |
| STMeta-Emb-Concat |   V1    |   2.62967   |  12.22 hour / 718 epochs  |
| STMeta-Multi-Emb  |   V1    | **2.59255** |  13.46 hour / 783 epochs  |
|    STMeta-Add     |   V1    |   2.63242   | 103.44 hour / 6511 epochs |
|    STMeta-LSTM-Add    |   V1    | **2.58002** | 53.36 hour / 3226 epochs  |
|   STMeta-Gating   |   V1    |   2.59783   | 67.95 hour / 3888 epochs  |
|     STMeta-Emb-Add     |   V1    | 2.700740582 | 146.93 hour / 9534 epochs |
|   STMeta-Emb-Gating    |   V1    | 2.60807 | 36.35 hour / 2227 epochs |
|  STMeta-MultiEmb-Add   |   V1    | 2.634200370 | 136.58 hour / 8885 epochs |
| STMeta-MultiEmb-Gating |   V1    | 2.69037 | 85.24 hour / 5162 epochs |
|   STMeta-LSTM-Concat   |   V1    | 2.59444 | 62.99 hour / 3974 epochs |
|   STMeta-LSTM-Gating   |   V1    | 2.58462 | 46.48 hour / 2890 epochs |

|   **City: DC**    | Version | test-rmse |      Converged Time      |
| :---------------: | :-----: | :-------: | :----------------------: |
|      STMeta       |   V1    |  2.44287  | 78.61 hour / 5750 epochs |
|   STMeta-Concat   |   V1    |  2.40469  | 66.71 hour / 4361 epochs |
| STMeta-Emb-Concat |   V1    |  2.42240  | 72.54 hour / 5321 epochs |
| STMeta-Multi-Emb  |   V1    |  2.42558  | 55.53 hour / 4023 epochs |
|    STMeta-Add     |   V1    |  2.44094  | 70.82 hour / 5269 epochs |
|  STMeta-LSTM-Add  |   V1    |  2.42381  | 19.98 hour / 1367 epochs |
|   STMeta-Gating   |   V1    |  2.43501  | 54.22 hour / 3563 epochs |
|     STMeta-Emb-Add     |   V1    | 2.42680735 | 59.17 hour / 4536 epochs |
|   STMeta-Emb-Gating    |   V1    | 2.39913 | 36.75 hour / 2676 epochs |
|  STMeta-MultiEmb-Add   |   V1    | 2.42924388 | 49.12 hour / 3785 epochs |
| STMeta-MultiEmb-Gating |   V1    | 2.40581 | 24.49 hour / 1708 epochs |
|   STMeta-LSTM-Concat   |   V1    | 2.39950 | 41.82 hour / 2991 epochs |
|   STMeta-LSTM-Gating   |   V1    | 2.40208 | 29.91 hour / 2168 epochs |

## Results on DiDi Dataset

|  **City: Xian**   | Version | val-rmse |  test-rmse  |       Converged Time       |
| :---------------: | :-----: | :------: | :---------: | :------------------------: |
|      STMeta       |   V1    | 7.62051  |   5.82054   |  3.68 hour / 4367 epochs   |
|   STMeta-Concat   |   V1    | 15.56313 |   5.93437   |  5.10 hour / 6029 epochs   |
| STMeta-Emb-Concat |   V1    | 6.51017  |   5.81860   |  4.33 hour / 4536 epochs   |
| STMeta-Multi-Emb  |   V1    | 7.01359  |   5.82937   |  4.40 hour / 4688 epochs   |
|    STMeta-Add     |   V1    | 7.06727  | **5.77572** |  9.46 hour / 7853 epochs   |
|  STMeta-LSTM-Add  |   V1    | 7.99094  |   5.83680   | **0.83 hour / 383 epochs** |
|   STMeta-Gating   |   V1    | 6.62653  | **5.80114** |   1.57 hour / 410 epochs   |
|     STMeta-Emb-Add     |   V1    | 7.5391045 | 5.968069 |4.77 hour / 4919 epochs|
|   STMeta-Emb-Gating    |   V1    | 7.42862 | 6.17998 |6.51 hour / 6140 epochs|
|  STMeta-MultiEmb-Add   |   V1    | 11.777396 | 6.0611196 |8.21 hour / 9008 epochs|
| STMeta-MultiEmb-Gating |   V1    | 6.79001 | 6.13171 |7.68 hour / 8105 epochs|
|   STMeta-LSTM-Concat   |   V1    | 7.08333 | 5.86691 |10.67 hour / 10115 epochs|
|   STMeta-LSTM-Gating   |   V1    | 7.15130 | 6.02032 |5.56 hour / 5132 epochs|

| **City: Chengdu** | Version | val-rmse | test-rmse |     Converged Time      |
| :---------------: | :-----: | :------: | :-------: | :---------------------: |
|      STMeta       |   V1    | 6.81043  |  6.90155  | 1.58 hour / 1218 epochs |
|   STMeta-Concat   |   V1    | 7.07804  |  7.51672  | 5.75 hour / 5944 epochs |
| STMeta-Emb-Concat |   V1    | 6.86758  |  7.01818  | 2.00 hour / 1388 epochs |
| STMeta-Multi-Emb  |   V1    | 7.21825  |  7.36653  | 4.63 hour / 4033 epochs |
|    STMeta-Add     |   V1    | 6.77974  |  6.98959  | 1.53 hour / 767 epochs  |
|  STMeta-LSTM-Add  |   V1    | 6.89801  |  7.00606  | 1.87 hour / 1187 epochs |
|   STMeta-Gating   |   V1    | 6.84756  |  6.95486  | 1.49 hour / 1300 epochs |
|     STMeta-Emb-Add     |   V1    | 6.9952435 | 7.038321 |1.84 hour / 1581 epochs|
|   STMeta-Emb-Gating    |   V1    | 6.86497 | 6.95586 |9.92 hour / 9463 epochs|
|  STMeta-MultiEmb-Add   |   V1    | 7.224133 | 7.32032 |2.37 hour / 1782 epochs|
| STMeta-MultiEmb-Gating |   V1    | 7.11000 | 7.03295 |7.76 hour / 8144 epochs|
|   STMeta-LSTM-Concat   |   V1    | 6.88248 | 7.01486 |1.37 hour / 866 epochs|
|   STMeta-LSTM-Gating   |   V1    | 6.91026 | 6.99974 |2.15 hour / 1566 epochs|

注：默认lr为1e-5

**One-hot VS Directly digitize**

|   **City: Xian**    |        Version        |                         dim                         | val-rmse | test-rmse |      Converged Time       |
| :-----------------: | :-------------------: | :-------------------------------------------------: | :------: | :-------: | :-----------------------: |
| one embedding layer |      V1(one-hot)      | 63(30 weather+24 hourofday+ 7 dayofweek +2 holiday) | 7.91567  |  6.06816  | 29.40 hour / 29326 epochs |
| one embedding layer | V1(directly digitize) | 33(30 weather+1 hourofday+ 1 dayofweek + 1 holiday) | 8.64882  |  7.19601  |       20005 epochs        |

## Results on Metro Dataset

| **City: Shanghai** |      Version      | val-rmse  |   test-rmse   |     Converged Time      |
| :----------------: | :---------------: | :-------: | :-----------: | :---------------------: |
|       STMeta       |        V1         | 108.01402 |   154.47606   | 5.01 hour / 4661 epochs |
|   STMeta-Concat    |    V1（bs:8）     | 130.72882 |   173.28693   | 1.87 hour / 593 epochs  |
| STMeta-Emb-Concat  | V1（bs:8,emb:10） | 110.38365 |   154.38785   | 7.39 hour / 3280 epochs |
|  STMeta-Multi-Emb  |    V1(10-1-6)     | 113.25427 |   156.60223   | 10.11 hour / 927 epochs |
|     STMeta-Add     |        V1         | 109.79260 |   162.10060   | 3.25 hour / 2174 epochs |
|  STMeta-LSTM-Add   |        V1         | 108.04737 |   162.77530   | 5.48 hour / 3850 epochs |
|   STMeta-Gating    |        V1         | 106.15893 | **145.45236** | 6.00 hour / 2563 epochs |
|     STMeta-Emb-Add     |   V1    | 109.50246 | 162.56137 |6.96 hour / 6071 epochs|
|   STMeta-Emb-Gating    |   V1    | 122.47356 | 193.16714 |1.55 hour / 1060 epochs|
|  STMeta-MultiEmb-Add   |   V1    | 116.852875 | 175.7444 |6.54 hour / 4384 epochs|
| STMeta-MultiEmb-Gating |   V1    | 145.63090 | 231.93188 |0.96 hour / 587 epochs|
|   STMeta-LSTM-Concat   |   V1    | 109.59708 | 163.38629 |2.82 hour / 2025 epochs|
|   STMeta-LSTM-Gating   |   V1    | 110.60793 | 156.36403 |5.15 hour / 3723 epochs|

| **City: Chongqing** | Version | val-rmse  |  test-rmse   |      Converged Time       |
| :-----------------: | :-----: | :-------: | :----------: | :-----------------------: |
|       STMeta        |   V1    | 96.49490  |   92.83833   | 108.53 hour / 9808 epochs |
|    STMeta-Concat    |   V1    | 90.67642  |   90.54800   | 38.79 hour / 10000 epochs |
|  STMeta-Emb-Concat  |   V1    | 92.78490  | **84.36934** | 74.88 hour / 6481 epochs  |
|  STMeta-Multi-Emb   |   V1    | 88.46373  | **86.56753** | 129.20 hour / 9958 epochs |
|     STMeta-Add      |         | 92.31516  |   90.19092   | 61.63 hour / 10000 epochs |
|   STMeta-LSTM-Add   |   V1    | 101.02728 |   93.65583   | 29.31 hour / 4357 epochs  |
|    STMeta-Gating    |   V1    | 94.25858  |   87.03069   | 39.27 hour / 10000 epochs |
|     STMeta-Emb-Add     |   V1    | 90.5653 | 87.3754609 |49.11 hour / 9974 epochs|
|   STMeta-Emb-Gating    |   V1    | 92.22450 | 86.33407 |50.52 hour / 10000 epochs|
|  STMeta-MultiEmb-Add   |   V1    | 87.24216 | 91.136903475 |53.33 hour / 10000 epochs|
| STMeta-MultiEmb-Gating |   V1    | 89.99853 | 89.33861 |48.82 hour / 10000 epochs|
|   STMeta-LSTM-Concat   |   V1    | 92.33357 |   98.19508   |53.57 hour / 9618 epochs|
|   STMeta-LSTM-Gating   |   V1    | 98.98814 | 90.47805 |39.89 hour / 7041 epochs|

**Different embedding size**（default batch_size: 4）

| **City: Shanghai** | embedding size | val-rmse  | test-rmse |     Converged Time     |
| :----------------: | :------------: | :-------: | :-------: | :--------------------: |
| STMeta-Emb-Concat  |       6        | 121.75984 | 204.3386  | 0.71 hour / 74 epochs  |
| STMeta-Emb-Concat  |       8        | 115.21622 | 180.94931 | 1.00 hour / 194 epochs |
| STMeta-Emb-Concat  |       10       | 114.94099 | 170.57361 | 1.26 hour / 265 epochs |
| STMeta-Emb-Concat  |       12       | 135.88895 | 188.44237 | 1.01 hour / 200 epochs |
| STMeta-Emb-Concat  |       14       | 112.71642 | 175.08072 | 2.41 hour / 511 epochs |

**Different temporal position embedding size**（default batch_size: 8，weather_emb:10）

| **City: Shanghai** | embedding size | val-rmse  | test-rmse |     Converged Time      |
| :----------------: | :------------: | :-------: | :-------: | :---------------------: |
|  STMeta-Multi-Emb  |       4        | 114.76000 | 171.56076 | 1.94 hour / 280 epochs  |
|  STMeta-Multi-Emb  |       6        | 113.25427 | 156.60223 | 10.11 hour / 927 epochs |
|  STMeta-Multi-Emb  |       8        | 115.36623 | 180.37663 | 1.21 hour / 534 epochs  |
|  STMeta-Multi-Emb  |       10       | 112.31456 | 177.23885 | 1.43 hour / 620 epochs  |

**Different weather embedding size**（default batch_size: 8 tp_emb:6）

| **City: Shanghai** | embedding size | val-rmse  | test-rmse |     Converged Time     |
| :----------------: | :------------: | :-------: | :-------: | :--------------------: |
|  STMeta-Multi-Emb  |       4        | 109.41055 | 171.02711 | 0.80 hour / 348 epochs |
|  STMeta-Multi-Emb  |       6        | 123.74634 | 166.39934 | 1.34 hour / 683 epochs |
|  STMeta-Multi-Emb  |       8        | 123.71514 | 182.98827 | 0.93 hour / 418 epochs |
|  STMeta-Multi-Emb  |       10       | 121.60524 | 179.59850 | 0.85 hour / 398 epochs |
|  STMeta-Multi-Emb  |       12       | 115.26234 | 171.73476 | 1.35 hour / 718 epochs |

**Different batch effect **

| **City: Shanghai** | batch | val-rmse  | test-rmse |     Converged Time      |
| :----------------: | :---: | :-------: | :-------: | :---------------------: |
|  STMeta-Multi-Emb  |  16   | 113.86533 | 181.91652 | 1.39 hour / 498 epochs  |
|  STMeta-Multi-Emb  |   8   | 123.13991 | 181.91342 | 4.90 hour / 2032 epochs |
|  STMeta-Multi-Emb  |   4   | 122.49625 | 179.65306 | 1.01 hour / 242 epochs  |
|  STMeta-Multi-Emb  |   2   | 112.73404 | 178.33081 | 1.67 hour / 290 epochs  |

## Results on EV Dataset

| **City: Beijing** |   Version   | val-rmse |  test-rmse  |      Converged Time       |
| :---------------: | :---------: | :------: | :---------: | :-----------------------: |
|      STMeta       | V1（bs:64） | 0.79145  |   0.81805   | 10.58 hour / 6205 epochs  |
|   STMeta-Concat   | V1（bs:32） | 0.74699  |   0.78338   |  9.13 hour / 4339 epochs  |
| STMeta-Emb-Concat |     V1      | 0.75199  |   0.78521   | 15.59 hour / 9970 epochs  |
| STMeta-Multi-Emb  |     V1      | 0.75170  |   0.79257   | 16.18 hour / 10332 epochs |
|    STMeta-Add     |     V1      | 0.76183  |   0.78709   |  9.68 hour / 5556 epochs  |
|  STMeta-LSTM-Add  |  W_SIZE:4   | 0.73958  | **0.78238** | 16.63 hour / 9336 epochs  |
|   STMeta-Gating   | V1（bs:32） | 0.74789  |   0.78317   |  9.68 hour / 4563 epochs  |
|     STMeta-Emb-Add     |   V1    | 0.7383992 | 0.7883851 |16.48 hour / 9997 epochs|
|   STMeta-Emb-Gating    |   V1    | 0.74721 | 0.78733 |11.94 hour / 7008 epochs|
|  STMeta-MultiEmb-Add   |   V1    | 0.75049156 | 0.7777612 |16.55 hour / 9986 epochs|
| STMeta-MultiEmb-Gating |   V1    | 0.74483 | 0.77961 |16.59 hour / 10000 epochs|
|   STMeta-LSTM-Concat   |   V1    | 0.74830 | 0.78860 |10.07 hour / 5722 epochs|
|   STMeta-LSTM-Gating   |   V1    | 0.74321 | 0.78408 |7.15 hour / 4057 epochs|

默认bs:64 

## Effectiveness of train day length

| **City: DC**  | trainday length | val-rmse | test-rmse |      Converged Time      |
| :-----------: | :-------------: | :------: | :-------: | :----------------------: |
| STMeta-Gating |        7        | 1.74639  |  5.73942  |  0.05 hour / 433 epochs  |
| STMeta-Gating |       28        | 3.01493  |  2.82653  | 0.72 hour / 1468 epochs  |
| STMeta-Gating |       49        | 2.50811  |  2.66609  |  0.84 hour / 626 epochs  |
| STMeta-Gating |       70        | 2.40444  |  2.55819  |  1.36 hour / 517 epochs  |
| STMeta-Gating |       91        | 2.32534  |  2.53470  | 3.72 hour / 1097 epochs  |
| STMeta-Gating |       112       | 2.47813  |  2.52416  | 4.99 hour / 1128 epochs  |
| STMeta-Gating |       133       | 2.42334  |  2.52744  | 10.45 hour / 1968 epochs |
| STMeta-Gating |       154       | 2.39524  |  2.53610  | 6.91 hour / 1048 epochs  |
| STMeta-Gating |       196       | 2.42895  |  2.51162  | 7.34 hour / 1126 epochs  |
| STMeta-Gating |       259       | 2.50016  |  2.52670  | 12.70 hour / 1456 epochs |
| STMeta-Gating |       322       | 2.47781  |  2.48798  | 24.38 hour / 2259 epochs |
| STMeta-Gating |       385       | 2.43614  |  2.44860  | 26.27 hour / 2226 epochs |

## LSTM Windows Size

| **City: Xian**  | window size | val-rmse |  test-rmse  |      Converged Time       |
| :-------------: | :---------: | :------: | :---------: | :-----------------------: |
|     STMeta      |      -      | 7.62051  |   5.82054   |  3.68 hour / 4367 epochs  |
|  STMeta-Gating  |      -      | 6.62653  |   5.80114   |  1.57 hour / 410 epochs   |
| STMeta-LSTM-Add |      4      | 6.78389  | **5.72379** |  7.68 hour / 8414 epochs  |
| STMeta-LSTM-Add |      6      | 6.43401  |   5.84958   | 14.54 hour / 16399 epochs |
| STMeta-LSTM-Add |      8      | 6.70062  |   5.78989   |  8.51 hour / 9635 epochs  |

| **City: Beijing** | window size | val-rmse |  test-rmse  |      Converged Time      |
| :---------------: | :---------: | :------: | :---------: | :----------------------: |
|      STMeta       |      -      | 0.79145  |   0.81805   | 10.58 hour / 6205 epochs |
|   STMeta-Gating   |      -      | 0.74789  |   0.78317   | 9.68 hour / 4563 epochs  |
|  STMeta-LSTM-Add  |      4      | 0.73958  | **0.78238** | 16.63 hour / 9336 epochs |
|  STMeta-LSTM-Add  |      6      | 0.74820  |   0.78632   | 15.00 hour / 8452 epochs |
|  STMeta-LSTM-Add  |      8      | 0.74523  |   0.78896   | 17.14 hour / 9717 epochs |