# External Results

## Results on Bike Dataset

|          **City: NYC**           | Version | test-rmse | # Params |      Converged Time       |
| :------------------------------: | :-----: | :-------: | :------: | :-----------------------: |
|       No external feature        |   V1    |  3.51827  |          |        5930 epochs        |
| 原UTCB（hour & holiday feature） |         |  3.43870  |          |                           |
|           dense layer            |   V1    |  3.38520  |   ---    | 214.70 hour / 7757 epochs |
|       one embedding layer        |   V1    |  3.38310  |          | 127.81 hour / 4876 epochs |
|       classified Embedding       |   V1    |  3.39106  |   ---    | 227.71 hour / 9155 epochs |

## Results on DiDi Dataset

①外部特征未归一化    ②外部特征归一化    √收敛    ×未收敛，达到了最大epoch

|          **City: Xian**          | Version |           val-rmse           |        test-rmse         |                      Converged Time                      |
| :------------------------------: | :-----: | :--------------------------: | :----------------------: | :------------------------------------------------------: |
|       No external feature        |   V1    |                              |         5.871044         |                 6.64 hour / 6911 epochs                  |
| 原UTCB（hour & holiday feature） |         |                              |         5.89154          |                                                          |
|           dense layer            |   V1    |   9.764658<br />15.373072    | 5.807899<br />6.3856196  | 13.70 hour / 14188 epochs<br />15.20 hour / 15163 epochs |
|       one embedding layer        |   V1    |   7.86501①<br />7.915668②    | 6.0782647<br />6.0681624 | 29.30 hour / 29223 epochs<br />29.40 hour / 29326 epochs |
|       classified Embedding       |   V1    | 7.6469483​① √<br />7.570738②√ | 5.851229<br />5.8357115  | 39.18 hour / 40001 epochs<br />49.32 hour / 50001 epochs |
|        External-closeness        |   V1    |          7.9909368           |        5.8367977         |                **0.83 hour / 383 epochs**                |

注：默认lr为1e-5



##### one-hot VS directly digitize

|   **City: Xian**    |        Version        |                         dim                         | val-rmse | test-rmse |      Converged Time       |
| :-----------------: | :-------------------: | :-------------------------------------------------: | :------: | :-------: | :-----------------------: |
| one embedding layer |      V1(one-hot)      | 63(30 weather+24 hourofday+ 7 dayofweek +2 holiday) | 7.915668 | 6.0681624 | 29.40 hour / 29326 epochs |
| one embedding layer | V1(directly digitize) | 33(30 weather+1 hourofday+ 1 dayofweek + 1 holiday) | 8.648821 | 7.196011  |       20005 epochs        |





## Results on Metro Dataset

①外部特征未归一化    ②外部特征归一化    √收敛    ×未收敛，达到了最大epoch

|        **City: Shanghai**        |                 Version                  |                           val-rmse                           |                test-rmse                |                        Converged Time                        |
| :------------------------------: | :--------------------------------------: | :----------------------------------------------------------: | :-------------------------------------: | :----------------------------------------------------------: |
|       No external feature        |                    V1                    |                          125.13439                           |                153.17380                |                   3.59 hour / 3226 epochs                    |
| 原UTCB（hour & holiday feature） |                                          |                           92.74990                           |                151.11746                |                                                              |
|           dense layer            |                    V1                    |         139.64864①√<br />802.6042①×<br />685.7447②×          | 827.4815<br />768.85956<br />536.91705  | 4.95 hour / 3938 epochs<br />24.12 hour / 20000 epochs<br />36.29 hour / 30000 epochs |
|       one embedding layer        |                    V1                    |                 148.48398①×<br />134.51851②×                 |        221.04675<br />204.40411         |    82.71 hour / 69988 epochs<br />82.14 hour 60000 epochs    |
|       classified Embedding       |                    V1                    | 123.484825​①​√<br />271.18738②√(lr:1e-5)<br />132.08806②×(lr:1e-4) | 177.69667<br />328.65323<br />195.32414 | 19.08 hour / 15640 epochs<br />3.55 hour / 2918 epochs<br />37.27 hour / 60000 epochs |
|        External-closeness        | V1(batch_size:32)<br />V1(batch_size:64) |                 106.34441②√<br />108.24415②√                 |        164.20714<br />158.71454         |  **9.39 hour / 3537 epochs**<br />18.75 hour / 9568 epochs   |



## Results on EV Dataset

|        **City: Beijing**         | Version |               val-rmse               |        test-rmse         |                  Converged Time                  |
| :------------------------------: | :-----: | :----------------------------------: | :----------------------: | :----------------------------------------------: |
|       No external feature        |   V1    |               0.58684                |         0.83100          |             5.51 hour / 2648 epochs              |
| 原UTCB（hour & holiday feature） |         |               0.57868                |         0.815518         |            26.27 hour / 20000 epochs             |
|           dense layer            |   V1    |               3.162586               |        3.3826275         |              1.41 hour / 703 epochs              |
|       one embedding layer        |   V1    |              3.4991612               |        3.5420315         |              1.03 hour / 519 epochs              |
|       classified Embedding       |   V1    |              1.2894919               |         1.269317         |             5.88 hour / 2956 epochs              |
|        External-closeness        |   V1    | 0.9059565（32）<br />0.8711627（16） | 0.8864132<br />0.8617136 | 0.25 hour / 81 epochs<br />0.50 hour / 91 epochs |

大batch_size(64 32) train_loss 抖动，尝试16（16较为稳定），数据有很多有效记录值站点较少，检查减少情况。