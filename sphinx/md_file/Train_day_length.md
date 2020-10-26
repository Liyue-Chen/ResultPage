# Train Day Length Analysis

## 60 mins train day

The base model is **STMeta-DCGRU-GAL**. The best result is in bold. 原始数据的粒度为60 mins, data_range指定为0.25，时间跨度为一年多一点，context建模方法为$Raw-Gating$ 方法

### Results on Bike Dataset

|   **City: DC**    | Days | val-rmse  |     test-rmse      |      Converged Time      |
| :---------------: | :--: | :-------: | :----------------: | :----------------------: |
| STMeta-V3-Context |  7   | 1.7463906 |     5.73942279     |  0.05 hour / 433 epochs  |
| STMeta-V3-Context |  28  | 3.0149283 |     2.82652771     | 0.72 hour / 1468 epochs  |
| STMeta-V3-Context |  49  | 2.508105  |    2.666094606     |  0.84 hour / 626 epochs  |
| STMeta-V3-Context |  70  | 2.4044392 |     2.5581854      |  1.36 hour / 517 epochs  |
| STMeta-V3-Context |  91  | 2.3253407 | 2.5347000025848483 | 3.72 hour / 1097 epochs  |
| STMeta-V3-Context | 112  | 2.4781277 |     2.5241638      | 4.99 hour / 1128 epochs  |
| STMeta-V3-Context | 133  | 2.4233427 |    2.527435054     | 10.45 hour / 1968 epochs |
| STMeta-V3-Context | 154  | 2.3952448 |    2.536095507     | 6.91 hour / 1048 epochs  |
| STMeta-V3-Context | 196  |           |                    |                          |
| STMeta-V3-Context | 259  |           |                    |                          |
| STMeta-V3-Context | 322  |           |                    |                          |
| STMeta-V3-Context | 385  |           |                    |                          |

|     **City: DC**      | Days |   val-rmse    |  test-rmse   |      Converged Time      |
| :-------------------: | :--: | :-----------: | :----------: | :----------------------: |
| STMeta-V3-w/o context |  7   |   1.8131874   | 3.2362974739 |  0.04 hour / 314 epochs  |
| STMeta-V3-w/o context |  28  |   2.9178348   | 2.6315900720 |  0.18 hour / 304 epochs  |
| STMeta-V3-w/o context |  49  |   2.5159404   |  2.4994903   |  0.55 hour / 371 epochs  |
| STMeta-V3-w/o context |  70  |   2.3288496   |  2.46409958  | 6.76 hour / 3035 epochs  |
| STMeta-V3-w/o context |  91  |   2.4020553   |  2.52117001  |  0.81 hour / 167 epochs  |
| STMeta-V3-w/o context | 112  |   2.4351285   | 2.4607768254 | 24.24 hour / 5766 epochs |
| STMeta-V3-w/o context | 133  |   2.4213538   | 2.461727915  | 10.50 hour / 1952 epochs |
| STMeta-V3-w/o context | 154  |   2.3805287   | 2.4872454319 | 45.22 hour / 7253 epochs |
| STMeta-V3-w/o context | 196  |   2.442964    | 2.487856267  | 26.78 hour / 3190 epochs |
| STMeta-V3-w/o context | 259  |   2.5098527   | 2.496907828  | 76.00 hour / 6757 epochs |
| STMeta-V3-w/o context | 322  |  2.47380803   |  2.46645875  | 53.81 hour / 3728 epochs |
| STMeta-V3-w/o context | 385  | 2.44229955285 | 2.478165765  | 97.09 hour / 6453 epochs |



| **City: template** | Days | val-rmse | test-rmse | Converged Time |
| :----------------: | :--: | :------: | :-------: | :------------: |
| STMeta-V3-Context  |  7   |          |           |                |
| STMeta-V3-Context  |  28  |          |           |                |
| STMeta-V3-Context  |  49  |          |           |                |
| STMeta-V3-Context  |  70  |          |           |                |
| STMeta-V3-Context  |  91  |          |           |                |
| STMeta-V3-Context  | 112  |          |           |                |
| STMeta-V3-Context  | 133  |          |           |                |
| STMeta-V3-Context  | 154  |          |           |                |
| STMeta-V3-Context  | 196  |          |           |                |
| STMeta-V3-Context  | 259  |          |           |                |
| STMeta-V3-Context  | 322  |          |           |                |
| STMeta-V3-Context  | 385  |          |           |                |