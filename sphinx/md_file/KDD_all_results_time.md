# Time Cost on Different Datasets

## Results on Bike 

| <font color='red'>**Fitness: 15 mins**</font> |            NYCⅠ            |          ChicagoⅡ          |            DCⅢ             | Converged Time                                               |
| :-------------------------------------------: | :------------------------: | :------------------------: | :------------------------: | ------------------------------------------------------------ |
|                      HM                       |                            |                            |                            |                                                              |
|                   ARIMA(C)                    |                            |                            |                            |                                                              |
|                    XGBoost                    |                            |                            |                            |                                                              |
|                     GBRT                      |                            |                            |                            |                                                              |
|                ST_MGCN (G/DCI)                |          1.68659           |          1.64642           |          1.54455           | 7.63 hour / 152 epochsⅠ<br />14.95 hour / 57 epochsⅡ<br />6.37 hour / 140 epochsⅢ |
|                 DCRNN(G/D C)                  |          1.71223           |          1.71789           |          1.59412           | 25.89 hour / 9999 epochsⅠ<br />0.86 hour / 542 epochsⅡ<br />12.72 hour / 9999 epochsⅢ |
|                   LSTM (C)                    | 0.0240446 hour / 10 epochs | 0.0149686 hour / 10 epochs | 0.0136856 hour / 10 epochs | 14.87 hour / 986 epochsⅠ<br />15.79 hour / 9167 epochsⅡ<br />0.30 hour / 199 epochsⅢ |
|                TMeta-LSTM-GAL                 | 0.0419362 hour / 10 epochs | 0.0264753 hour / 10 epochs | 0.0238060 hour / 10 epochs | 361 epochsⅠ<br />4.50 hour / 1278 epochsⅡ<br />0.51 hour / 199 epochsⅢ |
|               AMulti-GCLSTM-V1                | 0.1702106 hour / 10 epochs | 0.0941956 hour / 10 epochs | 0.0860629 hour / 10 epochs | 49.28 hour / 2280 epochsⅠ<br />11.26 hour / 775 epochsⅡ<br />26.81 hour / 2929 epochsⅢ |
|               AMulti-GCLSTM-V2                | 0.1362924 hour / 10 epochs | 0.0745592 hour / 10 epochs | 0.0684167 hour / 10 epochs | 84.40 hour / 6088 epochsⅠ<br />13.97 hour / 1269 epochsⅡ<br />51.15 hour / 7015 epochsⅢ |
|               AMulti-GCLSTM-V3                | 0.2228201 hour / 10 epochs | 0.1308789 hour / 10 epochs | 0.1202026 hour / 10 epochs | 26.27 hour / 930 epochsⅠ<br />6.14 hour / 287 epochsⅡ<br />9.48 hour / 664 epochsⅢ |

| <font color='red'>**Fitness: 30 mins**</font> |            NYCⅠ            |          ChicagoⅡ          |            DCⅢ             | Converged Time                                               |
| :-------------------------------------------: | :------------------------: | :------------------------: | :------------------------: | ------------------------------------------------------------ |
|                      HM                       |      2.68564 `2-1-2`       |       2.22987`3-2-1`       |       1.95601`3-1-4`       |                                                              |
|                   ARIMA(C)                    |          3.17849           |          2.42798           |          2.22804           |                                                              |
|                    XGBoost                    |   2.70377 `12-8-1-36-3`    |    2.37553`7-5-2-24-2`     |   1.95560`12-13-4-27-2`    |                                                              |
|                     GBRT                      |   2.68164 `12-10-0-72-4`   |    2.35532`9-13-2-91-2`    |   1.92799`13-15-5-140-1`   |                                                              |
|                ST_MGCN (G/DCI)                |          2.51288           |          2.17659           |          1.90305           | 24.25 hour / 183 epochsⅠ<br />18.32 hour / 39 epochsⅡ<br />8.40 hour / 171 epochsⅢ |
|                 DCRNN(G/D C)                  |          2.61848           |          2.24642           |          2.11771           | 56.82 hour / 10034 epochsⅠ<br />16.44 hour / 10000 epochsⅡ<br />8.98 hour / 6077 epochsⅢ |
|                   LSTM (C)                    | 0.0246239 hour / 10 epochs | 0.0150254 hour / 10 epochs | 0.0137515 hour / 10 epochs | 93.77 hour / 14343 epochsⅠ<br />1.56 hour / 797 epochsⅡ<br />0.61 hour / 18 epochsⅢ |
|                TMeta-LSTM-GAL                 | 0.0513773 hour / 10 epochs | 0.0323770 hour / 10 epochs | 0.0290520 hour / 10 epochs | 10839 epochsⅠ<br />1.01 hour / 138 epochsⅡ<br />26.25 hour / 3224 epochsⅢ |
|               AMulti-GCLSTM-V1                | 0.2074239 hour / 10 epochs | 0.1159768 hour / 10 epochs | 0.1063082 hour / 10 epochs | 6764 epochsⅠ<br />6.67 hour / 332 epochsⅡ<br />192.52 hour / 4576 epochsⅢ |
|               AMulti-GCLSTM-V2                | 0.1669437 hour / 10 epochs | 0.0919488 hour / 10 epochs | 0.0840447 hour / 10 epochs | 7100 epochsⅠ<br />5.28 hour / 310 epochsⅡ<br />53.36 hour / 2247 epochsⅢ |
|               AMulti-GCLSTM-V3                | 0.3163193 hour / 10 epochs | 0.1602899 hour / 10 epochs | 0.1473914 hour / 10 epochs | 244.95 hour / 2848 epochsⅠ<br />8.40 hour / 308 epochsⅡ<br />48.27 hour / 1208 epochsⅢ |



| <font color='red'>**Fitness: 60 mins**</font> |            NYCⅠ            |          ChicagoⅡ          |            DCⅢ             | Converged Time                                               |
| :-------------------------------------------: | :------------------------: | :------------------------: | :------------------------: | ------------------------------------------------------------ |
|                      HM                       |      3.99224 `1-1-3`       |       3.10445`1-1-1`       |       2.63169`2-1-3`       |                                                              |
|                   ARIMA(C)                    |          5.28928           |          3.74440           |          3.18296           |                                                              |
|                    XGBoost                    |   4.10211 `13-7-0-103-3`   |    3.00349`11-8-0-35-4`    |    2.64322`11-9-5-28-3`    |                                                              |
|                     GBRT                      |    4.03881`12-6-1-58-5`    |    2.98366`11-8-1-92-5`    |    2.61127`11-8-5-54-3`    |                                                              |
|                ST_MGCN (G/DCI)                |          3.72337           |          2.90369           |          2.51839           | 15.00 hour / 207 epochsⅠ<br />100.82 hour / 100 epochsⅡ<br />40.97 hour / 63 epochsⅢ |
|                 DCRNN(G/D C)                  |          4.18666           |  3.08066`重新运行的结果`   |  3.01575`重新运行的结果`   | 15.32 hourⅡ<br />0.36 hourⅢ                                  |
|                   LSTM (C)                    | 0.0246095 hour / 10 epochs | 0.0150423 hour / 10 epochs | 0.0137477 hour / 10 epochs | <br />48.23 hour / 20000 epochsⅡ<br />2.94 hour / 1783 epochsⅢ |
|                TMeta-LSTM-GAL                 | 0.0556675 hour / 10 epochs | 0.0347836 hour / 10 epochs | 0.0315096 hour / 10 epochs | 115.19 hour / 16343 epochsⅠ<br />594 epochsⅡ<br />28.50 hour / 7194 epochsⅢ |
|               AMulti-GCLSTM-V1                | 0.2250637 hour / 10 epochs | 0.1261709 hour / 10 epochs | 0.1153249 hour / 10 epochs | 5930 epochsⅠ<br />16.82 hour / 946 epochsⅡ<br />104.21 hour / 3875 epochsⅢ |
|               AMulti-GCLSTM-V2                | 0.1812923 hour / 10 epochs | 0.0997709 hour / 10 epochs | 0.0914019 hour / 10 epochs | 15000 epochsⅠ<br /><br />211.76 hour / 14588 epochsⅡ<br />99.59 hour / 4087 epochsⅢ |
|               AMulti-GCLSTM-V3                | 0.3444768 hour / 10 epochs | 0.1739124 hour / 10 epochs | 0.1600614 hour / 10 epochs | 7438 epochsⅠ<br />4403 epochsⅡ<br />96.94 hour / 2993 epochsⅢ |



## Results on DiDi

#### Xi'an

| <font color='red'>**City: Xi'an <br />Fitness: 15 mins**</font> |       Params       |         Time Cost          | # Params |      Converged Time       |
| :----------------------------------------------------------: | :----------------: | :------------------------: | :------: | :-----------------------: |
|                              HM                              |      `5-0-4`       |          2.82784           |   ---    |            ---            |
|                           ARIMA(C)                           |         --         |          3.08823           |    --    |            --             |
|                           XGBoost                            |   `7-14-0-10-4`    |          2.79919           |   ---    |            ---            |
|                             GBRT                             |   `11-2-2-45-3`    |          2.77484           |   ---    |            ---            |
|                          ST-ResNet                           |      `待补充`      |          2.68641           | `待补充` |         0.29 hour         |
|                       ST_MGCN (G/DCI)                        |      `待补充`      |          2.71417           |  248985  |  4.78 hour / 290 epochs   |
|                        DCRNN (G/D C)                         |                    |          2.88934           |  50368   | 90.71 hour / 10000 epochs |
|                           LSTM(C)                            |   `1-64-32-2-64`   | 0.0052424 hour / 10 epochs |          |  6.01 hour / 8600 epochs  |
|                          TMeta(TM)                           |                    | 0.0066098 hour / 8 epochs  |          |   0.86 hour / 7 epochs    |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` | 0.0230464 hour / 10 epochs |          | 24.12 hour / 7082 epochs  |
|                   AMulti-GCLSTM-V2(G/DCI)                    | `1-1-1-64-32-2-64` | 0.0182601 hour / 10 epochs |          |  8.34 hour / 2778 epochs  |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    | 0.0292676 hour / 10 epochs |          |  6.50 hour / 941 epochs   |



| <font color='#ff0000'>**City: Xi'an <br />Fitness: 30 mins**</font> |       Params       |         Time Cost          | # Params |      Converged Time       |
| :----------------------------------------------------------: | :----------------: | :------------------------: | :------: | :-----------------------: |
|                              HM                              |      `2-0-2`       |          4.23940           |   ---    |            ---            |
|                           ARIMA(C)                           |         --         |          5.03538           |    --    |            --             |
|                           XGBoost                            |    `9-0-2-25-3`    |          4.17160           |   ---    |            ---            |
|                             GBRT                             |    `9-0-2-80-3`    |          4.13541           |   ---    |            ---            |
|                          ST-ResNet                           |   `4-64-3-32-6`    |          3.90263           | `待补充` |         0.48 hour         |
|                       ST_MGCN (G/DCI)                        |                    |          3.88621           |  248985  |  3.74 hour / 387 epochs   |
|                        DCRNN (G/D C)                         |                    |          4.52889           |  50368   | 47.15 hour / 10000 epochs |
|                           LSTM(C)                            |   `1-64-32-2-64`   | 0.0028906 hour / 10 epochs |          | 10.37 hour / 39614 epochs |
|                            TMeta                             |                    | 0.0037422 hour / 10 epochs |          | 5.25 hour / 10612 epochs  |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` | 0.0123193 hour / 10 epochs |          | 16.23 hour / 9331 epochs  |
|                   AMulti-GCLSTM-V2(G/DCI)                    | `1-1-1-64-32-2-64` | 0.0099675 hour / 10 epochs |          |  9.07 hour / 6312 epochs  |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    | 0.0159268 hour / 10 epochs |          |  7.96 hour / 3184 epochs  |



| <font color='red'>**City: Xi'an <br />Fitness: 60mins**</font> |       Params       |         Time Cost          | # Params |      Converged Time      |
| :----------------------------------------------------------: | :----------------: | :------------------------: | :------: | :----------------------: |
|                              HM                              |      `1-1-2`       |          6.18623           |   ---    |           ---            |
|                           ARIMA(C)                           |         --         |          9.47478           |    --    |            --            |
|                           XGBoost                            |   `12-0-2-10-5`    |          6.73346           |   ---    |           ---            |
|                             GBRT                             |    `9-0-2-50-2`    |          6.44639           |   ---    |           ---            |
|                          ST-ResNet                           |      `待补充`      |          6.07471           |   ---    |        0.23 hour         |
|                       ST_MGCN (G/DCI)                        |      `待补充`      |          5.87769           |  248942  |  1.18 hour / 259 epochs  |
|                        DCRNN (G/D C)                         |                    |          8.20254           |  50368   | 2.10 hour / 10000 epochs |
|                           LSTM(C)                            |   `1-64-32-2-64`   | 0.0017866 hour / 10 epochs |          | 2.37 hour / 11776 epochs |
|                            TMeta                             |                    | 0.0022845 hour / 10 epochs |          | 1.25 hour / 4265 epochs  |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` | 0.0070913 hour / 10 epochs |          | 6.64 hour / 6911 epochs  |
|                   AMulti-GCLSTM-V2(G/DCI)                    | `1-1-1-64-32-2-64` | 0.0058139 hour / 10 epochs |          | 2.52 hour / 2956 epochs  |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    | 0.0093339 hour / 10 epochs |          | 3.37 hour / 2393 epochs  |

#### Chengdu

| <font color='red'>**City: Chengdu  Fitness: 15 mins**</font> |       Params       |         Time Cost          | # Params |      Converged Time       |
| :----------------------------------------------------------: | :----------------: | :------------------------: | :------: | :-----------------------: |
|                              HM                              |      `2-7-4`       |          3.34701           |   ---    |            ---            |
|                           ARIMA(C)                           |         --         |          3.94791           |    --    |            --             |
|                           XGBoost                            |   `12-14-1-27-3`   |          3.42954           |   ---    |            ---            |
|                             GBRT                             |   `13-15-5-39-3`   |          3.36292           |   ---    |            ---            |
|                          ST-ResNet                           |      `待补充`      |          3.31394           | `待补充` |         0.38 hour         |
|                       ST_MGCN (G/DCI)                        |      `待补充`      |          3.29300           |  248985  |   2.98 hour / 60 epochs   |
|                        DCRNN (G/D C)                         |                    |          3.74328           |  50368   | 96.21 hour / 10000 epochs |
|                           LSTM(C)                            |   `1-64-32-2-64`   | 0.0074623 hour / 10 epochs |          | 21.24 hour / 40609 epochs |
|                          TMeta(TM)                           |                    | 0.0086796 hour / 10 epochs |          |  2.48 hour / 2244 epochs  |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` | 0.0255353 hour / 10 epochs |          |  7.10 hour / 1940 epochs  |
|                   AMulti-GCLSTM-V2(G/DCI)                    | `1-1-1-64-32-2-64` | 0.0204378 hour / 10 epochs |          |  6.88 hour / 2060 epochs  |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    | 0.0308494 hour / 10 epochs |          |  5.23 hour / 802 epochs   |



| <font color='red'>**City: Chengdu  Fitness: 30 mins**</font> |       Params       |         Time Cost          | # Params |      Converged Time       |
| :----------------------------------------------------------: | :----------------: | :------------------------: | :------: | :-----------------------: |
|                              HM                              |      `1-7-4`       |          4.85059           |   ---    |            ---            |
|                           ARIMA(C)                           |         --         |          6.61832           |    --    |            --             |
|                           XGBoost                            |   `9-14-3-16-3`    |          4.91460           |   ---    |            ---            |
|                             GBRT                             |   `10-10-5-34-3`   |          4.87335           |   ---    |            ---            |
|                          ST-ResNet                           |   `4-64-3-32-6`    |          4.67278           | `待补充` |         0.24 hour         |
|                       ST_MGCN (G/DCI)                        |                    |          4.73162           |  248985  |  3.77 hour / 433 epochs   |
|                        DCRNN (G/D C)                         |                    |          6.25836           |  50368   | 25.24 hour / 5113 epochs  |
|                           LSTM(C)                            |   `1-64-32-2-64`   | 0.0040148 hour / 10 epochs |          | 11.24 hour / 50000 epochs |
|                            TMeta                             |                    | 0.0048443 hour / 10 epochs |          |  2.17 hour / 3919 epochs  |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` | 0.0137651 hour / 10 epochs |          |  5.25 hour / 2649 epochs  |
|                   AMulti-GCLSTM-V2(G/DCI)                    | `1-1-1-64-32-2-64` | 0.0111266 hour / 10 epochs |          |  2.79 hour / 1472 epochs  |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    | 0.0168225 hour / 10 epochs |          |  5.97 hour / 2398 epochs  |



| <font color='red'>**City: Chengdu Fitness: 60mins**</font> |       Params       |         Time Cost          | # Params |      Converged Time       |
| :--------------------------------------------------------: | :----------------: | :------------------------: | :------: | :-----------------------: |
|                             HM                             |      `0-7-4`       |          7.51214           |   ---    |            ---            |
|                          ARIMA(C)                          |         --         |          13.25890          |    --    |            --             |
|                          XGBoost                           |    `9-6-2-14-3`    |          7.59180           |   ---    |            ---            |
|                            GBRT                            |   `9-12-2-50-5`    |          7.51148           |   ---    |            ---            |
|                         ST-ResNet                          |      `待补充`      |          7.15462           |   ---    |         0.19 hour         |
|                      ST_MGCN (G/DCI)                       |      `待补充`      |          7.06687           |          |  1.12 hour / 181 epochs   |
|                       DCRNN (G/D C)                        |                    |          11.44437          |          | 23.94 hour / 10000 epochs |
|                          LSTM(C)                           |   `1-64-32-2-64`   | 0.0023025 hour / 10 epochs |          | 3.48 hour / 17464 epochs  |
|                           TMeta                            |                    | 0.0028853 hour / 10 epochs |          | 3.68 hour / 13715 epochs  |
|                  AMulti-GCLSTM-V1 (G/DCI)                  | `1-1-1-64-32-2-64` | 0.0077573 hour / 10 epochs |          |  2.54 hour / 2285 epochs  |
|                  AMulti-GCLSTM-V2(G/DCI)                   | `1-1-1-64-32-2-64` | 0.0064104 hour / 10 epochs |          |  1.40 hour / 1445 epochs  |
|                  AMulti-GCLSTM-V3(G/DCI)                   |                    | 0.0098129 hour / 10 epochs |          |  1.76 hour / 1052 epochs  |



## Results on Metro

#### Chongqing

| **<font color='#ff0000'>City: Chongqing <br />Fitness: 15mins</font>** |       Params       |         Time Cost          | # Params |       Converged Time       |
| :----------------------------------------------------------: | :----------------: | :------------------------: | :------: | :------------------------: |
|                              HM                              |      `2-1-4`       |          45.25524          |   ---    |            ---             |
|                           ARIMA(C)                           |        ---         |          67.11072          |   ---    |            ---             |
|                           XGBoost                            |   `12-6-4-51-8`    |          35.69683          |   ---    |            ---             |
|                             GBRT                             |  `12-14-1-182-7`   |          33.28726          |   ---    |            ---             |
|                       ST_MGCN (G/DCI)                        |      `待补充`      |          32.71874          |  248985  |  64.83 hour / 605 epochs   |
|                         DCRNN(G/D C)                         |        ---         |          37.06903          |          | 149.65 hour / 8784 epochs  |
|                           LSTM(C)                            |   `1-64-32-2-64`   | 0.0251394 hour / 10 epochs |          | 70.41 hour / 20000 epochs  |
|                            TMeta                             | `1-1-1-64-32-2-64` | 0.0556251 hour / 10 epochs |  62789   | 190.09 hour / 19897 epochs |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` | 0.1108510 hour / 10 epochs |  189521  | 138.15 hour / 8515 epochs  |
|                   AMulti-GCLSTM-V2 (G/DCI)                   |    patience 400    | 0.0918776 hour / 10 epochs |          | 138.45 hour / 10000 epochs |
|                   AMulti-GCLSTM-V3(G/DCI)                    |    patience 400    | 0.1062242 hour / 10 epochs |          |  84.73 hour / 6355 epochs  |



| <font color='#ff0000'>**City: Chongqing Fitness:30mins**</font> |       Params       |         Time Cost          | # Params |       Converged Time       |
| :----------------------------------------------------------: | :----------------: | :------------------------: | :------: | :------------------------: |
|                              HM                              |      `1-0-4`       |          74.54662          |   ---    |            ---             |
|                           ARIMA(C)                           |        ---         |         180.53262          |   ---    |            ---             |
|                           XGBoost                            |   `11-5-0-45-8`    |          69.50227          |   ---    |            ---             |
|                             GBRT                             |   `10-3-0-107-8`   |          72.98518          |   ---    |            ---             |
|                       ST_MGCN (G/DCI)                        |      `待补充`      |          50.95764          |  248985  |                            |
|                         DCRNN(G/D C)                         |        ---         |          65.71969          |  50368   | 165.58 hour / 19050 epochs |
|                           LSTM(C)                            |   `1-64-32-2-64`   | 0.0129002 hour / 10 epochs |          | 81.92 hour / 39999 epochs  |
|                            TMeta                             |                    | 0.0282905 hour / 10 epochs |          | 109.74 hour / 24069 epochs |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` | 0.0561989 hour / 10 epochs |  189521  | 84.38 hour / 10387 epochs  |
|                   AMulti-GCLSTM-V2 (G/DCI)                   |                    | 0.0468043 hour / 10 epochs |  180561  | 101.56 hour / 15000 epochs |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    | 0.0542460 hour / 10 epochs |  488447  |  53.57 hour / 7148 epochs  |



| <font color='#ff0000'>**City: Chongqing <br />Fitness: 60mins**</font> |        Params        |         Time Cost          | \# Params |      Converged Time       |
| :----------------------------------------------------------: | :------------------: | :------------------------: | :-------: | :-----------------------: |
|                              HM                              |      `0-1-4` ✅       |         119.85931          |    ---    |            ---            |
|                           ARIMA(C)                           |         ---          |         578.18563          |    ---    |            ---            |
|                           XGBoost                            |   `9-14-2-200-5` ✅   |         117.05069          |    ---    |            ---            |
|                             GBRT                             |  `12-10-4-200-5 `✅   |         113.92276          |    ---    |            ---            |
|                       ST_MGCN (G/DCI)                        |       `待补充`       |         104.87059          |  248985   | 52.48 hour / 1757 epochs  |
|                         DCRNN(G/D C)                         |         ---          |         122.31121          |           |                           |
|                           LSTM(C)                            |    `1-64-32-2-64`    | 0.0067899 hour / 10 epochs |           | 25.73 hour / 24338 epochs |
|                            TMeta                             |    `1-64-32-2-64`    | 0.0146863 hour / 10 epochs |   62789   | 47.22 hour / 20000 epochs |
|                   AMulti-GCLSTM-V1 (G/DCI)                   |  `1-1-1-64-32-2-64`  | 0.0291288 hour / 10 epochs |  189521   | 81.89 hour / 19970 epochs |
|                   AMulti-GCLSTM-V2 (G/DCI)                   | 未完全收敛$\Uparrow$ | 0.0243668 hour / 10 epochs |  180561   | 69.72 hour / 20000 epochs |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                      | 0.0282677 hour / 10 epochs |  488447   | 40.19 hour / 10004 epochs |

#### Shanghai

| <font color='#ff0000'>**City: Shanghai  Fitness: 15mins**</font> |       Params       |         Time Cost          | # Params |      Converged Time       |
| :----------------------------------------------------------: | :----------------: | :------------------------: | :------: | :-----------------------: |
|                              HM                              |      `1-0-4`       |          49.74561          |   ---    |            ---            |
|                           ARIMA(C)                           |        ---         |          83.53750          |   ---    |            ---            |
|                           XGBoost                            |   `11-10-4-31-7`   |          47.88690          |   ---    |            ---            |
|                             GBRT                             |   `12-7-1-148-5`   |          44.55068          |   ---    |            ---            |
|                       ST_MGCN (G/DCI)                        |      `待补充`      |          46.54292          |  248985  |  7.40 hour / 637 epochs   |
|                         DCRNN(G/D C)                         |        ---         |          56.00411          |          |        12.26 hour         |
|                           LSTM(C)                            |   `1-64-32-2-64`   | 0.0054067 hour / 10 epochs |          | 15.89 hour / 20000 epochs |
|                            TMeta                             | `1-1-1-64-32-2-64` | 0.0082920 hour / 10 epochs |  62789   | 11.62 hour / 9178 epochs  |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` | 0.0296992 hour / 10 epochs |  189521  | 87.67 hour / 20000 epochs |
|                   AMulti-GCLSTM-V2 (G/DCI)                   |                    | 0.0236432 hour / 10 epochs |  180561  | 48.30 hour / 14488 epochs |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    | 0.0401897 hour / 10 epochs |  488447  | 65.16 hour / 12285 epochs |



| <font color='#ff0000'>**City: Shanghai  Fitness: 30mins**</font> |       Params       |         Time Cost          | # Params |      Converged Time       |
| :----------------------------------------------------------: | :----------------: | :------------------------: | :------: | :-----------------------: |
|                              HM                              |      `1-1-3`       |         108.59372          |   ---    |            ---            |
|                           ARIMA(C)                           |        ---         |         212.00777          |   ---    |            ---            |
|                           XGBoost                            |   `12-6-1-206-3`   |          81.82434          |   ---    |            ---            |
|                             GBRT                             |    `7-4-1-58-7`    |          83.93989          |   ---    |            ---            |
|                       ST_MGCN (G/DCI)                        |      `待补充`      |          88.76412          |  248985  |  4.46 hour / 822 epochs   |
|                         DCRNN(G/D C)                         |        ---         |         116.14510          |          |       17391 epochs        |
|                           LSTM(C)                            |   `1-64-32-2-64`   | 0.0029574 hour / 10 epochs |          | 6.40 hour / 20000 epochs  |
|                            TMeta                             | `1-1-1-64-32-2-64` | 0.0045758 hour / 10 epochs |  62789   | 10.95 hour / 20000 epochs |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` | 0.0160158 hour / 10 epochs |  189521  | 39.91 hour / 20000 epochs |
|                   AMulti-GCLSTM-V2 (G/DCI)                   |                    | 0.0129321 hour / 10 epochs |  180561  | 35.27 hour / 20000 epochs |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    | 0.0216294 hour / 10 epochs |  488447  |       19990 epochs        |



| <font color='#ff0000'>**City: Shanghai  Fitness: 60mins**</font> |       Params       |         Time Cost          | # Params |      Converged Time       |
| :----------------------------------------------------------: | :----------------: | :------------------------: | :------: | :-----------------------: |
|                              HM                              |      `0-0-4`       |         172.54974          |   ---    |            ---            |
|                           ARIMA(C)                           |        ---         |         676.78754          |   ---    |            ---            |
|                           XGBoost                            |    `3-7-0-50-5`    |         160.37798          |   ---    |            ---            |
|                             GBRT                             |    `9-5-1-66-6`    |         154.28609          |   ---    |            ---            |
|                       ST_MGCN (G/DCI)                        |      `待补充`      |         159.52248          |  248985  |  3.05 hour / 1121 epochs  |
|                         DCRNN(G/D C)                         |        ---         |         340.25143          |          |       20000 epochs        |
|                           LSTM(C)                            |   `1-64-32-2-64`   | 0.0018055 hour / 10 epochs |          | 3.43 hour / 20000 epochs  |
|                            TMeta                             | `1-1-1-64-32-2-64` | 0.0028042 hour / 10 epochs |  62789   |  1.42 hour / 4633 epochs  |
|                   AMulti-GCLSTM-V1 (G/DCI)                   | `1-1-1-64-32-2-64` | 0.0091284 hour / 10 epochs |  189521  |  3.59 hour / 3226 epochs  |
|                   AMulti-GCLSTM-V2 (G/DCI)                   |                    | 0.0074883 hour / 10 epochs |  180561  | 15.21 hour / 17945 epochs |
|                   AMulti-GCLSTM-V3(G/DCI)                    |                    | 0.0125606 hour / 10 epochs |  488447  | 30.38 hour / 20000 epochs |



## Results on Charge-Station

| <font color='#ff0000'>**City: Beijing <br />TimeFitness: 30mins**</font> |       Params       |         Time Cost          | # Params |      Converged Time       |
| :----------------------------------------------------------: | :----------------: | :------------------------: | :------: | :-----------------------: |
|                              HM                              |      `2-0-0`       |          0.86361           |   ---    |            ---            |
|                           ARIMA(C)                           |                    |          0.75522           |   ---    |            ---            |
|                           XGBoost                            |    `6-6-1-19-2`    |          0.68649           |   ---    |            ---            |
|                             GBRT                             |   `13-3-2-47-3`    |          0.68931           |   ---    |            ---            |
|                        ST_MGCN (G/DC)                        |      `待补充`      |          0.69083           |  166025  |  4.05 hour / 380 epochs   |
|                         DCRNN(G/D C)                         |                    |          0.75740           |  50368   |  0.76 hour / 699 epochs   |
|                           LSTM(C)                            |   `1-64-32-2-64`   | 0.0065771 hour / 10 epochs |  28992   | 14.20 hour / 15135 epochs |
|                            TMeta                             |                    | 0.0096650 hour / 10 epochs |  62789   | 27.48 hour / 20000 epochs |
|                   AMulti-GCLSTM-V1 (G/DC)                    | `1-1-1-64-32-2-64` | 0.0262096 hour / 10 epochs |  130379  | 16.48 hour / 4242 epochs  |
|                   AMulti-GCLSTM-V2 (G/DC)                    |                    | 0.0208481 hour / 10 epochs |  129867  | 48.30 hour / 15543 epochs |
|                   AMulti-GCLSTM-V3 (G/DC)                    |                    | 0.0320221 hour / 10 epochs |  488447  | 30.59 hour / 6990 epochs  |



| <font color='#ff0000'>**City: Beijing <br />TimeFitness: 60mins**</font> |       Params       |         Time Cost          | \# Params |      Converged Time       |
| :----------------------------------------------------------: | :----------------: | :------------------------: | :-------: | :-----------------------: |
|                              HM                              |     `2-0-2` ✅      |          1.01610           |    ---    |            ---            |
|                           ARIMA(C)                           |                    |          0.98236           |    ---    |            ---            |
|                           XGBoost                            |  `12-7-0-20-2` ✅   |          0.83381           |    ---    |            ---            |
|                             GBRT                             | `12-10-0-100-2 `✅  |          0.82814           |    ---    |            ---            |
|                        ST_MGCN (G/DC)                        |    LSTMUnit:32     |           0.827            |  166025   |  3.84 hour / 884 epochs   |
|                         DCRNN(G/D C)                         |                    |          0.98871           |   50368   | 7.20 hour / 10000 epochs  |
|                           LSTM(C)                            |   `1-64-32-2-64`   | 0.0031535 hour / 2 epochs  |   28992   | 8.19 hour / 17309 epochs  |
|                            TMeta                             |   `1-64-32-2-64`   | 0.0053729 hour / 10 epochs |   62789   | 31.53 hour / 39999 epochs |
|                   AMulti-GCLSTM-V1 (G/DC)                    | `1-1-1-64-32-2-64` | 0.0141336 hour / 10 epochs |  130379   |  5.51 hour / 2648 epochs  |
|                   AMulti-GCLSTM-V2 (G/DC)                    |                    | 0.0113272 hour / 10 epochs |  129867   | 41.44 hour / 20000 epochs |
|                   AMulti-GCLSTM-V3 (G/DC)                    |                    | 0.0172101 hour / 10 epochs |  488447   | 23.76 hour / 10497 epochs |

