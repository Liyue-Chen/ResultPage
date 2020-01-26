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

|          **City: Xian**          | Params |              val-rmse              | test-rmse |      Converged Time       |
| :------------------------------: | :----: | :--------------------------------: | :-------: | :-----------------------: |
|       No external feature        |   V1   |                                    | 5.871044  |  6.64 hour / 6911 epochs  |
| 原UTCB（hour & holiday feature） |        |                                    |  5.89154  |                           |
|           dense layer            |   V1   |              9.764658              | 5.807899  | 13.70 hour / 14188 epochs |
|       one embedding layer        |   V1   | <font color="red">10.548454</font> | 6.1003566 |  2.03 hour / 1531 epochs  |
|       classified Embedding       |   V1   | <font color="red">20.22674</font>  | 17.148306 |  1.00 hour / 366 epochs   |

注：西安的one embedding layer 和classified Embedding不收敛，调小学习率（由1e-5调整为5e-6）正在重新跑。

