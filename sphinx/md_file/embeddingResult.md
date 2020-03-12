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



## Results on Metro Dataset

①外部特征未归一化    ②外部特征归一化    √收敛    ×未收敛，达到了最大epoch

|        **City: Shanghai**        |      Version      |          val-rmse           |        test-rmse        |                     Converged Time                     |
| :------------------------------: | :---------------: | :-------------------------: | :---------------------: | :----------------------------------------------------: |
|       No external feature        |        V1         |                             |                         |                                                        |
| 原UTCB（hour & holiday feature） |                   |          92.74990           |        151.11746        |                                                        |
|           dense layer            |        V1         | 139.64864①√<br />802.6042①× | 827.4815<br />768.85956 | 4.95 hour / 3938 epochs<br />24.12 hour / 20000 epochs |
|       one embedding layer        |        V1         |         148.48398①×         |        221.04675        |               82.71 hour / 69988 epochs                |
|       classified Embedding       |        V1         |        123.484825​①​√         |        177.69667        |               19.08 hour / 15640 epochs                |
|        External-closeness        | V1(batch_size:32) |         106.34441②√         |        164.20714        |              **9.39 hour / 3537 epochs**               |

