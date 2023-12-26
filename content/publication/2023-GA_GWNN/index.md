---
title: "GA-GWNN: Generalized Adaptive Graph Wavelet Neural Network"
date: 2023-11-24
publishDate:  2023-11-24
authors: ["Swakshar Deb", "Shafin Rahman", "Sejuti Rahman"]
publication_types: ["2"]
abstract: "Wavelet-based graph neural networks have received increasing attention in the node classification task. Existing graph wavelet-based approaches, however, are not applicable to arbitrary graphs as they use
predefined wavelet filters with built-in homophilic assumptions and disregard heterophily. Recent
studies attempted to address this issue through a wavelet lifting transform, which requires a bipartite
graph, therefore altering the graph topology and leading to undesirable wavelet filters. This paper
proposes a generalized adaptive graph wavelet network that preserves the graph topology through computational trees while implementing the lifting scheme on arbitrary graphs. Moreover, this locally defined lifting scheme integrates both high-pass and low-pass frequency components to further enhance feature representation. Finally, we benchmark our model using nine homophilic and heterophilic datasets, and the results demonstrate the effectiveness of our method."
featured: true
tags:
- Graph Neural Network
- Node Classification
publication: "2023 Pattern Recognition Letters (PRL)"
links:
  - icon_pack: fas
    icon: scroll
    name: Paper
    url: 'https://www.sciencedirect.com/science/article/pii/S0167865523003355?dgcid=coauthor'
  
  - icon_pack: fas
    icon: scroll
    name: Supplementary
    url: 'https://drive.google.com/file/d/1g2PnWIb4FrOGribcyYXBkIWkglj02-5_/view?usp=sharing'
  
  - icon_pack: ai
    icon: open-data
    name: Code
    url: 'https://github.com/SwaksharDeb/GA-GWNN'
---

![gemm_architecture](/img/GA_GWNN.PNG)
<p style="text-align:center"> Figure: An overview of the GA-GWNN. The red and yellow colored ball represents nodes with high and low-frequency information respectively, color gradient ball indicates the fusion of both low and high-frequency information, L is the total number of layers. Symbols over the right arrows indicate particular operations. </p>