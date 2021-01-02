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

**以下是使用inflow+outflow 预测inflow+outflow的结果**

| **Fitness: 5 mins<br />Inflow,Outflow :arrow_right:Inflow,Outflow** | Params | val-rmse | test-rmse |      Converged Time      |
| :----------------------------------------------------------: | :----: | :------: | :-------: | :----------------------: |
|                        distance graph                        |        | 27.52427 | 25.81179  | 44.30 hour / 3000 epochs |
|                    static reachable graph                    | 1-hop  | 40.41435 | 36.92094  | 96.88 hour / 7941 epochs |
|                    static reachable graph                    | 2-hop  | 40.71255 | 36.99143  | 39.24 hour / 2979 epochs |
|                   dynamic reachable graph                    | 1-hop  | 41.75912 | 38.00227  | 35.51 hour / 2959 epochs |

* distance graph : 根据站点的欧氏距离计算的静态图.
* static reachable graph  : 根据站点之间的运行时间确定的5分钟可达图，这是一张静态图，因为站点与站点的距离是固定的.
* dynamic reachable graph：根据发车间隔和运行时间共同确定的5分钟可达图，这是一张动态图，因为列车的是动态的.

**以下是使用inflow+outflow 预测outflow的结果**

|                     **Fitness: 5 mins**                      | Params | val-rmse | test-rmse |      Converged Time      |
| :----------------------------------------------------------: | :----: | :------: | :-------: | :----------------------: |
|      distance graph<br />**Inflow:arrow_right:Outflow**      |        | 40.62962 | 40.84833  | 45.21 hour / 3000 epochs |
|  static reachable graph<br />**Inflow:arrow_right:Outflow**  | 2-hop  | 113.3009 | 105.8779  |  7.79 hour / 391 epochs  |
|  distance graph<br />**Inflow,Outflow:arrow_right:Outflow**  |        | 30.88421 | 29.44295  | 44.07 hour / 2994 epochs |
| static reachable graph<br />**Inflow,Outflow:arrow_right:Outflow** | 2-hop  | 49.65576 | 45.66458  | 36.35 hour / 3000 epochs |



