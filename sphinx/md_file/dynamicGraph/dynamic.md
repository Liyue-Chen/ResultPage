# Results on dynamic Graph

## Results on Metro

#### Chongqing

| <font color='red'>**City: Chongqing<br />Fitness: 5 mins**</font> | Params | val-rmse | test-rmse | Converged Time |
| :----------------------------------------------------------: | :----: | :------: | :-------: | :------------: |
|                        distance graph                        |        |          |           |                |
|                    static reachable graph                    |        |          |           |                |
|                   dynamic reachable graph                    |        |          |           |                |

#### Shanghai

使用一个月(30天)的数据进行训练，***C/P/T=6/0/0***，实验基于STMeta-V1(GCLSTM-GAL-GAL)

| <font color='red'>**City: Shanghai<br />Fitness: 5 mins**</font> | Params | val-rmse | test-rmse |      Converged Time      |
| :----------------------------------------------------------: | :----: | :------: | :-------: | :----------------------: |
|                        distance graph                        |        | 25.51274 | 25.99594  |       3188 epochs        |
|                    static reachable graph                    | 1-hop  | 41.23481 | 37.46707  | 25.20 hour / 2039 epochs |
|                    static reachable graph                    | 2-hop  | 40.99424 | 37.32953  | 22.53 hour / 1819 epochs |
|                   dynamic reachable graph                    |        |          |           |                          |

* distance graph : 根据站点的欧氏距离计算的静态图.
* static reachable graph  : 根据站点之间的运行时间确定的5分钟可达图，这是一张静态图，因为站点与站点的距离是固定的.
* dynamic reachable graph：根据发车间隔和运行时间共同确定的5分钟可达图，这是一张动态图，因为列车的是动态的.


