![f1](f-vis.jpg)
**Figure 1：Effectiveness of Geometric-Aware Prototype.** The second row in the figure represents the prototype clustering method used in the EUMS, while the third row illustrates the use of geometric-aware prototypes for constructing hypergraphs to facilitate novel class inference. As shown in the figure, the geometric-aware prototypes more effectively capture the contours and local structures of target objects. This enables the model to better focus on foreground objects, enhancing its ability to distinguish them from the background.


**Table1: Effectiveness of Geometric-Aware Prototype.**

| Method  | bike | build | <span style="color: gray;">car</span> | <span style="color: gray;">cone</span> | fence | grou | <span style="color: gray;">pers</span> | plants | <span style="color: gray;">pole</span> | rider | traf. | trashc. | trunk | Novel | Known | All   |
|---------|------|-------|-------------------------------------|---------------------------------------|-------|------|--------------------------------------|--------|--------------------------------------|-------|-------|---------|-------|-------|-------|-------|
| Full    | 46.9 | 85.9  | <span style="color: gray;">55.4</span>| <span style="color: gray;">37.3</span>| 48.9  | 80.0 | <span style="color: gray;">64.5</span>  | 79.4  | <span style="color: gray;">35.8</span>| 59.4  | 31.9  | 7.8     | 25.2  | --    | 50.6  |       |
| UNI3D   | 43.9 | 30.4  | <span style="color: gray;">3.2</span> | <span style="color: gray;">31.2</span>| 45.6  | 68.4 | <span style="color: gray;">60.8</span> | 32.4  | <span style="color: gray;">42.8</span>| 57.2  | 33.4  | 12.9    | 14.8  | 48.4  | 38.0  | 41.2  |
| Ours    | 44.7 | 58.3  | <span style="color: gray;">4.4</span> | <span style="color: gray;">28.4</span>| 47.4  | 80.9 | <span style="color: gray;">65.4</span> | 45.3  | <span style="color: gray;">41.6</span>| 57.9  | 34.1  | 10.8    | 17.9  | 47.2  | 38.7  | 41.3  |

