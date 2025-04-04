![f1](f-vis.jpg)
**Figure 1：Effectiveness of Geometric-Aware Prototype.** The second row in the figure represents the prototype clustering method used in the EUMS, while the third row illustrates the use of geometric-aware prototypes for constructing hypergraphs to facilitate novel class inference. As shown in the figure, the geometric-aware prototypes more effectively capture the contours and local structures of target objects. This enables the model to better focus on foreground objects, enhancing its ability to distinguish them from the background.


**Table 1: Comparison with Open-Vocabulary Method.** For the Open-vocabulary Method (UNI3D), the model is trained on the base classes in the SemanticPOSS dataset on Split 0, and new class inference is performed using the textual names of the new classes. The bolded portions in the table represent the new classes.
| Method  | bike | **build** | **car** | cone | fence | **grou** | pers| plants | pole| rider | traf. | trashc. | trunk | Novel | Known | All   |
|---------|------|-------|---------|----------|-------|------|----------|--------|----------|-------|-------|---------|-------|-------|-------|-------|
| Full    | 46.9 | **85.9**  | **55.4** | 37.3 | 48.9  | **80.0** | 64.5 | **79.4**  | 35.8 | 59.4  | 31.9  | 7.8     | 25.2  | --    | 50.6  |       |
| UNI3D[1]  | 43.9 | **30.4**  | **3.2**  | 35.2 | 45.6  | **68.4** | 62.8 | **32.4**  | 42.8 | 59.2  | 33.4  | 12.9    | 18.8  | **33.6**  | 39.4  | 37.6  |
| Ours    | 44.7 |**58.3**  | **4.4**  | 28.4 | 47.4  | **80.9** | 65.4 | **45.3**  | 41.6 | 57.9  | 34.1  | 10.8    | 17.9  | **47.2**  | 38.7  | 41.3  |

[1] Zhou J, Wang J, Ma B, et al. Uni3D: Exploring Unified 3D Representation at Scale[C]//ICLR. 2024.

**Table 2: The ablation experiment for learnable centroids.** Fixed centroids refer to the method where the Euclidean distance from each point to its assigned cluster center is directly computed, and the centroids are not updated afterward, making them highly influenced by the initial data distribution. In contrast, learnable centroids are adjusted during the training process, allowing them to better adapt to the point cloud data distribution and capture both the semantic and structural information of the point cloud data more effectively.
| Method              | **Build** | **Car** | **Grou** | **Plants** | **AVG** |
|---------------------|-----------|---------|----------|------------|---------|
| Fixed Centroid      | 56.2      | 4.1     | 76.4     | 45.2       | 45.5    |
| Learnable Centroid  | **58.3**  | **4.4** | **80.9** | **45.3**   | **47.2** |


**Table 3: The Impact of Batch Size on Experimental Performance.**
| Batch Size | **Build** | **Car** | **Grou** | **Plants** | **AVG** |
|------------|-----------|---------|----------|------------|---------|
| 1          | 58.1      | 3.7     | 80.4     | 43.7       |  46.5   |
| 2          | **58.3**  | 5.6    | 78.4      | 45.1       | 46.9 |
| 4          | **58.3**   | 4.4     |**80.9**     | 45.3       | **47.2**    |
| 8          | 57.4      | **6.2** | 77.4     | **45.6**   |    46.7 |
