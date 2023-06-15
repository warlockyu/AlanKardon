# Awesome Semi-supervised clustering 

## What's Deep Graph Clustering?

Semi-supervised clustering is an approach that combines unsupervised clustering and supervised learning to address clustering problems where both labeled and unlabeled data are available. In traditional clustering algorithms, only unlabeled data is used for clustering, while semi-supervised clustering algorithms leverage the information from labeled data to enhance the clustering performance.

The goal of semi-supervised clustering is to partition the samples in a dataset into different clusters while utilizing the information from labeled data to guide the clustering process. Generally, the workflow of a semi-supervised clustering algorithm involves the following steps:

1. Data preparation: The dataset is divided into labeled and unlabeled data. Labeled data includes class information, while unlabeled data only contains feature information.

2. Unsupervised clustering: Traditional unsupervised clustering algorithms such as K-means, DBSCAN, etc., are used to cluster the unlabeled data, generating initial clusters.

3. Construction of similarity graph: A similarity graph is generated based on the similarities between labeled and unlabeled data. The similarity graph represents the similarity relationships between samples, where the similarity between labeled data is determined by their class labels, and the similarity between unlabeled data can be calculated based on their distances in the feature space.

4. Semi-supervised learning: Using the information from labeled data and the similarity graph, the semi-supervised learning process takes place. Common methods include graph-based semi-supervised learning and distribution-based semi-supervised learning. These methods leverage the label information from labeled data and the similarity information from unlabeled data to optimize and adjust the clustering results.

5. Output of clustering results: Based on the results of semi-supervised learning, the clustering clusters are redefined and adjusted to obtain the final clustering results.

The advantage of semi-supervised clustering lies in its ability to leverage the information from labeled data to improve clustering performance. By incorporating prior knowledge from labeled data, it can better handle uncertainty and noise in unlabeled data, thereby enhancing clustering accuracy and robustness. However, semi-supervised clustering algorithms also face challenges, such as selecting appropriate similarity measures and effectively utilizing limited labeled data.


## Papers

### Graph-based Semi-supervised Learning

| Year | Title                                                        | Venue | Paper                                                        | Code |
| ---- | ------------------------------------------------------------ | ----- | ------------------------------------------------------------ | ---- |
| 2022 | **Graph-based Semi-supervised Learning: A Comprehensive Review** | IEEE  | [Link](https://ieeexplore.ieee.org/abstract/document/9737635) | -    |
| 2022 | **Graph-based sparse bayesian broad learning system for semi-supervised learning** | IS    | [Link](https://www.sciencedirect.com/science/article/abs/pii/S0020025522002481) | -    |
| 2023 | **Fairness in graph-based semi-supervised learning**         | KIS   | [Link](https://link.springer.com/article/10.1007/s10115-022-01738-w) | -    |
| 2022 | **A survey of large-scale graph-based semi-supervised classification algorithms** | JCCE  | [Link](https://www.sciencedirect.com/science/article/pii/S2666307422000201) | -    |
| 2023 | **A review on semi-supervised clustering**                   | IS    | [Link](https://www.sciencedirect.com/science/article/abs/pii/S0020025523002840) | -    |
| 2023 | **Noise-robust graph-based semi-supervised learning with dynamic shaving label propagation** | ASC   | [Link](https://www.sciencedirect.com/science/article/pii/S1568494623003897) | -    |

This method utilizes the similarity between data samples to construct a graph structure and uses the information from labeled data to guide the clustering process. Typically, the nodes of the graph represent the data samples, and the edges represent the similarity or connectivity between the samples. Graph-based algorithms can partition the data into different clusters using techniques such as graph cut and spectral clustering.

### Self-training-based semi-supervised clustering

| Year | Title                                                        | Venue | Paper                                                        | Code |
| ---- | ------------------------------------------------------------ | ----- | ------------------------------------------------------------ | :--: |
| 2022 | **Self-Training Based Semi-Supervised and Semi-Paired Hashing Cross-Modal Retrieval** | IJCNN | [Link](https://ieeexplore.ieee.org/abstract/document/9892301) |  -   |
| 2022 | **LaSSL: label-guided self-training for semi-supervised learning** | AAAI  | [Link](https://ojs.aaai.org/index.php/AAAI/article/view/20907) |  -   |
| 2022 | **Twist: Two-way inter-label self-training for semi-supervised 3d instance segmentation** | CVPR  | [Link](https://openaccess.thecvf.com/content/CVPR2022/html/Chu_TWIST_Two-Way_Inter-Label_Self-Training_for_Semi-Supervised_3D_Instance_Segmentation_CVPR_2022_paper.html) |  -   |
| 2022 | **A novel semi-supervised self-training method based on resampling for Twitter fake account identification** | DTA   | [Link](https://www.emerald.com/insight/content/doi/10.1108/DTA-07-2021-0196/full/html) |  -   |
| 2023 | **A Semi-Supervised Self-Training Ensemble Method Based on Clustering** | IEEE  | [Link](https://ieeexplore.ieee.org/abstract/document/10066026) |  -   |
| 2022 | **Semi‐supervised breast histopathological image classification with self‐training based on non‐linear distance metric** | IET   | [Link](https://ietresearch.onlinelibrary.wiley.com/doi/full/10.1049/ipr2.12548) |  -   |

This method utilizes the clustering results from labeled data to label the unlabeled data, and then re-trains the clustering model by incorporating these labeled data along with the original labeled data. Through iterative iterations of this process, the clustering performance can gradually improve. The key to this method lies in selecting appropriate labeling strategies and iterative stopping conditions.

### Self-training-based semi-supervised clustering

| Year | Title                                                        | Venue | Paper                                                        | Code |
| ---- | ------------------------------------------------------------ | ----- | ------------------------------------------------------------ | :--: |
| 2022 | **Self-Training Based Semi-Supervised and Semi-Paired Hashing Cross-Modal Retrieval** | IJCNN | [Link](https://ieeexplore.ieee.org/abstract/document/9892301) |  -   |
| 2022 | **LaSSL: label-guided self-training for semi-supervised learning** | AAAI  | [Link](https://ojs.aaai.org/index.php/AAAI/article/view/20907) |  -   |
| 2022 | **Twist: Two-way inter-label self-training for semi-supervised 3d instance segmentation** | CVPR  | [Link](https://openaccess.thecvf.com/content/CVPR2022/html/Chu_TWIST_Two-Way_Inter-Label_Self-Training_for_Semi-Supervised_3D_Instance_Segmentation_CVPR_2022_paper.html) |  -   |
| 2022 | **A novel semi-supervised self-training method based on resampling for Twitter fake account identification** | DTA   | [Link](https://www.emerald.com/insight/content/doi/10.1108/DTA-07-2021-0196/full/html) |  -   |
| 2023 | **A Semi-Supervised Self-Training Ensemble Method Based on Clustering** | IEEE  | [Link](https://ieeexplore.ieee.org/abstract/document/10066026) |  -   |
| 2022 | **Semi‐supervised breast histopathological image classification with self‐training based on non‐linear distance metric** | IET   | [Link](https://ietresearch.onlinelibrary.wiley.com/doi/full/10.1049/ipr2.12548) |  -   |

This method utilizes the clustering results from labeled data to label the unlabeled data, and then re-trains the clustering model by incorporating these labeled data along with the original labeled data. Through iterative iterations of this process, the clustering performance can gradually improve. The key to this method lies in selecting appropriate labeling strategies and iterative stopping conditions.

### Self-training-based semi-supervised clustering

| Year | Title                                                        | Venue | Paper                                                        | Code |
| ---- | ------------------------------------------------------------ | ----- | ------------------------------------------------------------ | :--: |
| 2022 | **Self-Training Based Semi-Supervised and Semi-Paired Hashing Cross-Modal Retrieval** | IJCNN | [Link](https://ieeexplore.ieee.org/abstract/document/9892301) |  -   |
| 2022 | **LaSSL: label-guided self-training for semi-supervised learning** | AAAI  | [Link](https://ojs.aaai.org/index.php/AAAI/article/view/20907) |  -   |
| 2022 | **Twist: Two-way inter-label self-training for semi-supervised 3d instance segmentation** | CVPR  | [Link](https://openaccess.thecvf.com/content/CVPR2022/html/Chu_TWIST_Two-Way_Inter-Label_Self-Training_for_Semi-Supervised_3D_Instance_Segmentation_CVPR_2022_paper.html) |  -   |
| 2022 | **A novel semi-supervised self-training method based on resampling for Twitter fake account identification** | DTA   | [Link](https://www.emerald.com/insight/content/doi/10.1108/DTA-07-2021-0196/full/html) |  -   |
| 2023 | **A Semi-Supervised Self-Training Ensemble Method Based on Clustering** | IEEE  | [Link](https://ieeexplore.ieee.org/abstract/document/10066026) |  -   |
| 2022 | **Semi‐supervised breast histopathological image classification with self‐training based on non‐linear distance metric** | IET   | [Link](https://ietresearch.onlinelibrary.wiley.com/doi/full/10.1049/ipr2.12548) |  -   |

This method utilizes the clustering results from labeled data to label the unlabeled data, and then re-trains the clustering model by incorporating these labeled data along with the original labeled data. Through iterative iterations of this process, the clustering performance can gradually improve. The key to this method lies in selecting appropriate labeling strategies and iterative stopping conditions.

### Co-training-based semi-supervised clustering

| Year | Title                                                        | Venue | Paper                                                        | Code |
| ---- | ------------------------------------------------------------ | ----- | ------------------------------------------------------------ | :--: |
| 2022 | **When Less is More: On the Value of" Co-training" for Semi-Supervised Software Defect Predictors** | arXiv | [Link](https://arxiv.org/abs/2211.05920)                     |  -   |
| 2022 | **Improving the co-training algorithm to enhance semi-supervised learning results** | IEEE  | [Link](https://ieeexplore.ieee.org/abstract/document/10020477) |  -   |
| 2022 | **Self-Paced Co-Training of Graph Neural Networks for Semi-Supervised Node Classification** | IEEE  | [Link](https://ieeexplore.ieee.org/abstract/document/9738732) |  -   |
| 2022 | **Energy-efficient semi-supervised learning framework for subchannel allocation in non-orthogonal multiple access systems** | ETRI  | [Link](https://onlinelibrary.wiley.com/doi/full/10.4218/etrij.2022-0251) |  -   |
| 2023 | **ProtoCon: Pseudo-Label Refinement via Online Clustering and Prototypical Consistency for Efficient Semi-Supervised Learning** | CVPR  | [Link](https://openaccess.thecvf.com/content/CVPR2023/html/Nassar_ProtoCon_Pseudo-Label_Refinement_via_Online_Clustering_and_Prototypical_Consistency_for_CVPR_2023_paper.html) |  -   |
| 2019 | **Co-training based on semi-supervised ensemble classification approach for multi-label data stream** | IEEE  | [Link](https://scholar.google.co.uk/scholar?as_ylo=2019&q=Co-training-based+semi-supervised+clustering&hl=zh-CN&as_sdt=0,5&as_vis=1) |  -   |

This method utilizes multiple mutually independent clustering algorithms for semi-supervised clustering. Each clustering algorithm is trained on different subsets of labeled and unlabeled data, and the results from each clustering algorithm are integrated using ensemble strategies. Through co-training, the accuracy and robustness of clustering can be improved.

### Constraint-based semi-supervised clustering

| Year | Title                                                        | Venue | Paper                                                        | Code |
| ---- | ------------------------------------------------------------ | ----- | ------------------------------------------------------------ | :--: |
| 2023 | **Stratification-based semi-supervised clustering algorithm for arbitrary shaped datasets** | IS    | [Link](https://www.sciencedirect.com/science/article/abs/pii/S0020025523005893) |  -   |
| 2023 | **Semi-supervised Clustering with Two Types of Background Knowledge: Fusing Pairwise Constraints and Monotonicity Constraints** | arXiv | [Link](https://arxiv.org/abs/2302.14060)                     |  -   |
| 2020 | **Tackling noise in active semi-supervised clustering**      | LNAI  | [Link](https://link.springer.com/chapter/10.1007/978-3-030-67661-2_8) |  -   |
| 2022 | **Semi-Supervised Clustering Ensemble Based on Cluster Consensus Selection** | CS    | [Link](https://www.tandfonline.com/doi/abs/10.1080/01969722.2022.2159150) |  -   |

This method guides the clustering process by utilizing domain knowledge or constraints defined by experts. Constraints can be either hard constraints (conditions that must be satisfied) or soft constraints (conditions that are prioritized), ensuring that the clustering results align with prior knowledge. Common constraints include class constraints (specifying which samples belong to specific categories) and similarity constraints (specifying the similarity relationships between samples).
