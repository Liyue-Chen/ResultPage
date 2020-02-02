# External Results

## Results on Bike Dataset

|          **City: NYC**           | Params | test-rmse | # Params |      Converged Time       |
| :------------------------------: | :----: | :-------: | :------: | :-----------------------: |
|       No external feature        |   V1   |           |          |                           |
| 原UTCB（hour & holiday feature） |        |  3.43870  |          |                           |
|           dense layer            |   V1   |  3.38520  |   ---    | 214.70 hour / 7757 epochs |
|       one embedding layer        |   V1   |  3.38310  |          | 127.81 hour / 4876 epochs |
|       classified Embedding       |   V1   |  3.39106  |   ---    | 227.71 hour / 9155 epochs |

## Results on DiDi Dataset

|          **City: Xian**          |    Params     | val-rmse  | test-rmse |      Converged Time       |
| :------------------------------: | :-----------: | :-------: | :-------: | :-----------------------: |
|       No external feature        |      V1       |           | 5.871044  |  6.64 hour / 6911 epochs  |
| 原UTCB（hour & holiday feature） |               |           |  5.89154  |                           |
|           dense layer            |      V1       | 9.764658  | 5.807899  | 13.70 hour / 14188 epochs |
|       one embedding layer        |      V1       | 10.548454 | 6.1003566 |  2.03 hour / 1531 epochs  |
|       classified Embedding       | V1（lr:1e-6） | 18.090849 | 16.203615 |  3.63 hour / 3220 epochs  |

注：默认lr为1e-5



## Results on Metro Dataset

|        **City: Shanghai**        | Params |                           val-rmse                           |                    test-rmse                     |                    Converged Time                    |
| :------------------------------: | :----: | :----------------------------------------------------------: | :----------------------------------------------: | :--------------------------------------------------: |
|       No external feature        |   V1   |                                                              |                                                  |                                                      |
| 原UTCB（hour & holiday feature） |        |                           92.74990                           |                    151.11746                     |                                                      |
|           dense layer            |   V1   | 139.64864(adam )<br /><font color="red">1371.1122(sgd)</font> | 827.4815<br /><font color="red">1346.9358</font> | 4.95 hour / 3938 epochs<br />9.13 hour / 7729 epochs |
|       one embedding layer        |   V1   |                          148.48398                           |                    221.04675                     |              82.71 hour / 69988 epochs               |
|       classified Embedding       |   V1   |                          123.484825                          |                    177.69667                     |              19.08 hour / 15640 epochs               |

