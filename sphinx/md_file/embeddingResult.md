# External Results

#### 一些经验

1.虽然小batch_size容易抖动，但速度快，效果甚至更好，尽量不要实验太大的batch，如64。

2.可以先用大lr，小batch，训练至快收敛，然后换小lr，大batch。



## Results on Bike Dataset

|              **City: NYC**              | Version | test-rmse | # Params |      Converged Time       |
| :-------------------------------------: | :-----: | :-------: | :------: | :-----------------------: |
|                 STMeta                  |   V1    |  3.51827  |          |        5930 epochs        |
| 原UTCB（weather & hourofday & holiday） |   V1    |  3.43870  |          |                           |
|              STMeta-Concat              |   V1    |  3.38520  |   ---    | 214.70 hour / 7757 epochs |
|               STMeta-Emb                |   V1    |  3.38310  |          | 127.81 hour / 4876 epochs |
|            STMeta-Multi-Emb             |   V1    |  3.39106  |   ---    | 227.71 hour / 9155 epochs |
|              STMeta-Gating              |   V1    |  3.37795  |          | 120.89 hour / 4043 epochs |

## Results on DiDi Dataset

①外部特征未归一化    ②外部特征归一化    √收敛    ×未收敛，达到了最大epoch

|          **City: Xian**          |      Version      | val-rmse  | test-rmse |       Converged Time       |
| :------------------------------: | :---------------: | :-------: | :-------: | :------------------------: |
|              STMeta              |        V1         | 7.620508  | 5.820535  |  3.68 hour / 4367 epochs   |
| 原UTCB（hour & holiday feature） |        V1         |           |  5.89154  |                            |
|          STMeta-Concat           |        V1         | 15.56313  |  5.93437  |  5.10 hour / 6029 epochs   |
|            STMeta-Emb            | V1（bs:8 ,emb:6） | 6.5101748 | 5.818601  |  4.33 hour / 4536 epochs   |
|         STMeta-Multi-Emb         |        V1         |  7.01359  |  5.82937  |  4.40 hour / 4688 epochs   |
|        External-closeness        |        V1         | 7.9909368 | 5.8367977 | **0.83 hour / 383 epochs** |
|          STMeta-Gating           |        V1         | 6.626533  | 5.8011427 |   1.57 hour / 410 epochs   |

注：默认lr为1e-5



##### one-hot VS directly digitize

|   **City: Xian**    |        Version        |                         dim                         | val-rmse | test-rmse |      Converged Time       |
| :-----------------: | :-------------------: | :-------------------------------------------------: | :------: | :-------: | :-----------------------: |
| one embedding layer |      V1(one-hot)      | 63(30 weather+24 hourofday+ 7 dayofweek +2 holiday) | 7.915668 | 6.0681624 | 29.40 hour / 29326 epochs |
| one embedding layer | V1(directly digitize) | 33(30 weather+1 hourofday+ 1 dayofweek + 1 holiday) | 8.648821 | 7.196011  |       20005 epochs        |





## Results on Metro Dataset

①外部特征未归一化    ②外部特征归一化    √收敛    ×未收敛，达到了最大epoch

|        **City: Shanghai**        |                 Version                  |           val-rmse           |        test-rmse         |                      Converged Time                       |
| :------------------------------: | :--------------------------------------: | :--------------------------: | :----------------------: | :-------------------------------------------------------: |
|              STMeta              |                    V1                    |          108.01402           |        154.47606         |                  5.01 hour / 4661 epochs                  |
| 原UTCB（hour & holiday feature） |                                          |           92.74990           |        151.11746         |                                                           |
|          STMeta-Concat           |                V1（bs:8）                |          130.72882           |        173.28693         |                  1.87 hour / 593 epochs                   |
|            STMeta-Emb            |            V1（bs:8,emb:10）             |          110.38365           |        154.38785         |                  7.39 hour / 3280 epochs                  |
|         STMeta-Multi-Emb         |                V1(10-1-6)                |          113.25427           |        156.60223         |                  10.11 hour / 927 epochs                  |
|        External-closeness        | V1(batch_size:32)<br />V1(batch_size:64) | 106.34441②√<br />108.24415②√ | 164.20714<br />158.71454 | **9.39 hour / 3537 epochs**<br />18.75 hour / 9568 epochs |
|          STMeta-Gating           |            V1（bs:8 lr:5e-5）            |          106.15893           |        145.45236         |                  6.00 hour / 2563 epochs                  |

##### different embedding size（default batch_size: 4）

| **City: Shanghai** | embedding size |  val-rmse  | test-rmse |     Converged Time     |
| :----------------: | :------------: | :--------: | :-------: | :--------------------: |
|     STMeta-Emb     |       6        | 121.75984  | 204.3386  | 0.71 hour / 74 epochs  |
|     STMeta-Emb     |       8        | 115.21622  | 180.94931 | 1.00 hour / 194 epochs |
|     STMeta-Emb     |       10       | 114.940994 | 170.57361 | 1.26 hour / 265 epochs |
|     STMeta-Emb     |       12       | 135.88895  | 188.44237 | 1.01 hour / 200 epochs |
|     STMeta-Emb     |       14       | 112.716415 | 175.08072 | 2.41 hour / 511 epochs |

##### different temporal position embedding size（default batch_size: 8，weather_emb:10）

| **City: Shanghai** | embedding size | val-rmse  | test-rmse |     Converged Time      |
| :----------------: | :------------: | :-------: | :-------: | :---------------------: |
|  STMeta-Multi-Emb  |       4        | 114.76000 | 171.56076 | 1.94 hour / 280 epochs  |
|  STMeta-Multi-Emb  |       6        | 113.25427 | 156.60223 | 10.11 hour / 927 epochs |
|  STMeta-Multi-Emb  |       8        | 115.36623 | 180.37663 | 1.21 hour / 534 epochs  |
|  STMeta-Multi-Emb  |       10       | 112.31456 | 177.23885 | 1.43 hour / 620 epochs  |

##### different weather embedding size（default batch_size: 8 tp_emb:6）

| **City: Shanghai** | embedding size |  val-rmse  | test-rmse |     Converged Time     |
| :----------------: | :------------: | :--------: | :-------: | :--------------------: |
|  STMeta-Multi-Emb  |       4        | 109.41055  | 171.02711 | 0.80 hour / 348 epochs |
|  STMeta-Multi-Emb  |       6        | 123.74634  | 166.39934 | 1.34 hour / 683 epochs |
|  STMeta-Multi-Emb  |       8        | 123.71514  | 182.98827 | 0.93 hour / 418 epochs |
|  STMeta-Multi-Emb  |       10       | 121.60524  | 179.5985  | 0.85 hour / 398 epochs |
|  STMeta-Multi-Emb  |       12       | 115.262344 | 171.73476 | 1.35 hour / 718 epochs |





##### different batch effect

| **City: Shanghai** | batch | val-rmse  | test-rmse |     Converged Time      |
| :----------------: | :---: | :-------: | :-------: | :---------------------: |
|  STMeta-Multi-Emb  |  16   | 113.86533 | 181.91652 | 1.39 hour / 498 epochs  |
|  STMeta-Multi-Emb  |   8   | 123.13991 | 181.91342 | 4.90 hour / 2032 epochs |
|  STMeta-Multi-Emb  |   4   | 122.49625 | 179.65306 | 1.01 hour / 242 epochs  |
|  STMeta-Multi-Emb  |   2   | 112.73404 | 178.33081 | 1.67 hour / 290 epochs  |







## Results on EV Dataset

|        **City: Beijing**         |   Version   |               val-rmse               |        test-rmse         |                  Converged Time                  |
| :------------------------------: | :---------: | :----------------------------------: | :----------------------: | :----------------------------------------------: |
|              STMeta              | V1（bs:64） |               0.79145                |         0.81805          |             10.58 hour / 6205 epochs             |
| 原UTCB（hour & holiday feature） |             |               0.57868                |         0.81552          |            26.27 hour / 20000 epochs             |
|          STMeta-Concat           | V1（bs:32） |               0.74699                |         0.78338          |             9.13 hour / 4339 epochs              |
|            STMeta-Emb            |     V1      |               0.75199                |         0.78521          |             15.59 hour / 9970 epochs             |
|         STMeta-Multi-Emb         |     V1      |               0.75170                |         0.79257          |            16.18 hour / 10332 epochs             |
|        External-closeness        |     V1      | 0.9059565（32）<br />0.8711627（16） | 0.8864132<br />0.8617136 | 0.25 hour / 81 epochs<br />0.50 hour / 91 epochs |
|          STMeta-Gating           | V1（bs:32） |               0.74789                |         0.78317          |             9.68 hour / 4563 epochs              |

默认bs:64 

