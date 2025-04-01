![f1](f-vis.jpg)
**Figure 1：Effectiveness of Geometric-Aware Prototype.** The second row in the figure represents the prototype clustering method used in the EUMS, while the third row illustrates the use of geometric-aware prototypes for constructing hypergraphs to facilitate novel class inference. As shown in the figure, the geometric-aware prototypes more effectively capture the contours and local structures of target objects. This enables the model to better focus on foreground objects, enhancing its ability to distinguish them from the background.


**Table 1: Comparison with Open-Vocabulary Method.** For the Open-vocabulary Method (UNI3D), the model is trained on the base classes in the SemanticPOSS dataset on Split 0, and new class inference is performed using the textual names of the new classes.
| Method  | bike | **build** | **car** | cone | fence | **grou** | pers| plants | pole| rider | traf. | trashc. | trunk | Novel | Known | All   |
|---------|------|-------|---------|----------|-------|------|----------|--------|----------|-------|-------|---------|-------|-------|-------|-------|
| Full    | 46.9 | **85.9**  | **55.4** | 37.3 | 48.9  | **80.0** | 64.5 | **79.4**  | 35.8 | 59.4  | 31.9  | 7.8     | 25.2  | --    | 50.6  |       |
| UNI3D[1]  | 43.9 | **30.4**  | **3.2**  | 35.2 | 45.6  | **68.4** | 62.8 | **32.4**  | 42.8 | 59.2  | 33.4  | 12.9    | 18.8  | **33.6**  | 39.4  | 37.6  |
| Ours    | 44.7 |**58.3**  | **4.4**  | 28.4 | 47.4  | **80.9** | 65.4 | **45.3**  | 41.6 | 57.9  | 34.1  | 10.8    | 17.9  | **47.2**  | 38.7  | 41.3  |
