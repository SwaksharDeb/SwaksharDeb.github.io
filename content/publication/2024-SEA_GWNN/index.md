---
title: "SEA-GWNN: Simple and Effective Adaptive Graph Wavelet Neural Network"
date: 2024-02-01
publishDate:  2023-11-24
authors: ["Swakshar Deb", "Shafin Rahman", "Sejuti Rahman"]
publication_types: ["1"]
abstract: "The utilization of wavelet-based techniques in graph neural networks (GNNs) has gained considerable attention, particularly in the context of node classification. Although existing wavelet-based approaches have shown promise, they are constrained by their reliance on pre-defined wavelet filters, rendering them incapable of effectively adapting to signals that reside on graphs based on tasks at hand. Recent research endeavors address this issue through the introduction of a wavelet lifting transform. However, this technique necessitates the use of bipartite graphs, causing a transformation of the original graph structure into a bipartite configuration. This alteration of graph topology results in the generation of undesirable wavelet filters, thereby undermining the effectiveness of the method. In response to these challenges, we propose a novel simple and effective adaptive graph wavelet neural network (SEA-GWNN) class that employs the lifting scheme on arbitrary graph structures while upholding the original graph topology by leveraging multi-hop computation trees. A noteworthy aspect of the approach is the focus on local substructures represented as acyclic trees, wherein the lifting strategy is applied in a localized manner. This locally defined lifting scheme effectively combines high-pass and low-pass frequency information to enhance node representations. Furthermore, to reduce computing costs, we propose to decouple the higher-order lifting operators and induce them from the lower-order structures. Finally, we benchmark our model on several real-world datasets spanning four distinct categories, including citation networks, webpages, the film industry, and large-scale graphs and the experimental results showcase the efficacy of the proposed SEA-GWNN."
featured: true
tags:
- Graph Neural Network
- Node Classification
publication: "Association for the Advancement of Artiﬁcial Intelligence (AAAI), 2024"
links:
  - icon_pack: fas
    icon: scroll
    name: Paper
    url: 'https://drive.google.com/file/d/15YUHR1Z-2i4Z0QPjsKji1WEER-ZnBsoL/view'
  
  - icon_pack: fas
    icon: scroll
    name: Supplementary
    url: 'https://drive.google.com/file/d/1R-0uceA6eUMvAq0sJXmQ1k6kucq9dWRF/view'
  
  - icon_pack: ai
    icon: open-data
    name: Code
    url: 'https://github.com/AnonymousTEA/SEA-GWNN'
---

<!-- ![gemm_architecture](/img/GA_GWNN.PNG)
<p style="text-align:center"> Figure: An overview of the GA-GWNN. The red and yellow colored ball represents nodes with high and low-frequency information respectively, color gradient ball indicates the fusion of both low and high-frequency information, L is the total number of layers. Symbols over the right arrows indicate particular operations. </p> -->