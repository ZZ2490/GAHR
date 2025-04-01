![f1](f-vis.jpg)
**Figure 1：Effectiveness of Geometric-Aware Prototype.** The second row in the figure represents the prototype clustering method used in the EUMS, while the third row illustrates the use of geometric-aware prototypes for constructing hypergraphs to facilitate novel class inference. As shown in the figure, the geometric-aware prototypes more effectively capture the contours and local structures of target objects. This enables the model to better focus on foreground objects, enhancing its ability to distinguish them from the background.


**Table1：Effectiveness of Geometric-Aware Prototype.** 
| Method                        | bike | build | car  | cone | fence | grou | pers | plants | pole | rider | traf. | trashc. | trunk | Novel | Known | All   |
|-------------------------------|------|-------|------|------|-------|------|------|--------|------|-------|-------|---------|-------|-------|-------|-------|
| Full                          |  46.9|  85.9 |  55.4|  37.3|  48.9 |  80.0|  64.5|  79.4  |  35.8|  59.4 |  31.9 |  7.8    |  25.2 | --    |  50.6 |       |
| EUMS                          |  25.7|   4.0 |   0.6|  16.4|  29.4 |  36.8|  43.8|  28.5  |  13.1|  26.8 |  18.2 |  3.3    |  16.9 |  17.4 |  21.5 |  20.3 |
| NOPS                          |  35.5|  30.4 |   1.2|  13.5|  24.1 |  69.1|  44.7|  42.1  |  19.2|  47.7 |  24.4 |  8.2    |  21.8 |  35.7 |  26.6 |  29.4 |
| DASL                          |  46.3|  51.5 |   6.0|  35.7|  48.5 |  83.0|  67.9|  53.1  |  35.5|  59.3 |  31.0 |  2.8    |  15.5 |  48.4 |  38.0 |  41.2 |
| Ours                          |  44.7| **58.3** |   4.4|  28.4|  47.4 |  80.9|  65.4|  45.3  |  41.6|  57.9 |  34.1 |  10.8   |  17.9 |  47.2 |  38.7 |  41.3 |
