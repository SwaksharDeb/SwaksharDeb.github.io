---
title: "Graph Convolutional Networks for Assessment of Physical Rehabilitation Exercises"
date: 2023-06-18
publishDate:  2023-06-18
authors: ["**Swakshar Deb**", "Md Fokhrul Islam", "Shafin Rahman", "Sejuti Rahman"]
publication_types: ["1"]
abstract: "Health professionals often prescribe patients to perform specific exercises for rehabilitation of several diseases (e.g., stroke, Parkinson, backpain). When patients perform those exercises in the absence of an expert (e.g., physicians/therapists), they cannot assess the correctness of the performance. Automatic assessment of physical rehabilitation exercises aims to assign a quality score given an RGBD video of the body movement as input. Recent deep learning approaches address this problem by extracting CNN features from co-ordinate grids of skeleton data (body-joints) obtained from videos. However, they could not extract rich spatio-temporal features from variable-length inputs. To address this issue, we investigate Graph Convolutional Networks (GCNs) for this task. We adapt spatio-temporal GCN to predict continuous scores(assessment) instead of discrete class labels. Our model can process variable-length inputs so that users can perform any number of repetitions of the prescribed exercise. Moreover, our novel design also provides self-attention of body-joints, indicating their role in predicting assessment scores. It guides the user to achieve a better score in future trials by matching the same attention weights of expert users. Our model successfully outperforms existing exercise assessment methods on KIMORE and UI-PRMD datasets."
featured: true
tags:
- Deep learning
- Computer vision
publication: "2022 IEEE Transaction on Neural Systems and Rehabilitation Engineering (TNSRE)"
links:
  - icon_pack: fas
    icon: scroll
    name: Paper
    url: 'https://doi.org/10.1109/IJCNN54540.2023.10191500'
  - icon_pack: ai
    icon: open-data
    name: Code
    url: 'https://github.com/TahsinTariq/GEMM'
  - icon_pack: fas
    icon: video
    name: Video
    url: 'https://youtu.be/HjJh5guZLDQ'
---

![gemm_architecture](https://user-images.githubusercontent.com/62146852/232325513-e9de077e-49d3-4ce0-b090-6360054c55ca.png)
<p style="text-align:center"> Figure. The GEMM Architecture </p>