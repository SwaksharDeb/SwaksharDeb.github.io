---
title: "Graph Convolutional Networks for Assessment of Physical Rehabilitation Exercises"
date: 2023-06-18
publishDate:  2023-06-18
authors: ["**Swakshar Deb**", "Md Fokhrul Islam", "Shafin Rahman", "Sejuti Rahman"]
publication_types: ["2"]
abstract: "Health professionals often prescribe patients to perform specific exercises for rehabilitation of several diseases (e.g., stroke, Parkinson, backpain). When patients perform those exercises in the absence of an expert (e.g., physicians/therapists), they cannot assess the correctness of the performance. Automatic assessment of physical rehabilitation exercises aims to assign a quality score given an RGBD video of the body movement as input. Recent deep learning approaches address this problem by extracting CNN features from co-ordinate grids of skeleton data (body-joints) obtained from videos. However, they could not extract rich spatio-temporal features from variable-length inputs. To address this issue, we investigate Graph Convolutional Networks (GCNs) for this task. We adapt spatio-temporal GCN to predict continuous scores(assessment) instead of discrete class labels. Our model can process variable-length inputs so that users can perform any number of repetitions of the prescribed exercise. Moreover, our novel design also provides self-attention of body-joints, indicating their role in predicting assessment scores. It guides the user to achieve a better score in future trials by matching the same attention weights of expert users. Our model successfully outperforms existing exercise assessment methods on KIMORE and UI-PRMD datasets."
featured: true
tags:
- Graph Convolution
- Rehabilitation Exercises
publication: "2022 IEEE Transaction on Neural Systems and Rehabilitation Engineering (TNSRE)"
links:
  - icon_pack: fas
    icon: scroll
    name: Paper
    url: 'https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9709340'
  - icon_pack: ai
    icon: open-data
    name: Code
    url: 'https://github.com/SwaksharDeb/STGN-for-Rehabilitation'
  - icon_pack: fas
    icon: video
    name: Video
    url: 'https://www.youtube.com/playlist?list=PLtuJaRV_ofJArtjv6UVxIefFItN3BG8iw'
---

![Rehab Architecture](https://github.com/SwaksharDeb/swakshardeb.github.io/blob/main/static/img/stgcn_architecture.PNG)

<p style="text-align:center"> Figure. GCN based end-to-end models using (a-b) vanilla STGCN and (c-d) extended STGCN for rehabilitation exercise assessment. </p>