![f1](f-vis.jpg)
**Figure 1：Effectiveness of Geometric-Aware Prototype.** The second row in the figure represents the prototype clustering method used in the EUMS, while the third row illustrates the use of geometric-aware prototypes for constructing hypergraphs to facilitate novel class inference. As shown in the figure, the geometric-aware prototypes more effectively capture the contours and local structures of target objects. This enables the model to better focus on foreground objects, enhancing its ability to distinguish them from the background.
### Table 2. Comparison of Computational Complexity of Different Methods on the SemanticKITTI Dataset

| Method | Training Time (hours) | Test Time (hours) | GPU Memory (GB) |
|--------|----------------------|------------------|----------------|
| NOPS   | 11.41                | 0.46             | 11             |
| DASL   | 20.76                | 0.90             | 23.02          |
| Ours   | 29.69                | 2.13             | 41.68          |
