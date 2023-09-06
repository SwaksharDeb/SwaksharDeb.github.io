---
date: 2023-07-10
publishDate: 2023-07-10
external_link: ""
image:
  caption: RMEDU logo
  focal_point: Smart
slides: example
summary: Empowering Graph Wavelet Convolution for
Node Classification A Novel Approach with
Local Lifting Scheme
tags:
- Personal
title: I have successfuly defended my M.Sc Thesis
links:
  - icon_pack: fas
    icon: scroll
    name: M.Sc. Thesis Book
    url: 'https://drive.google.com/file/d/1zC25Aa1AUdb0Nx130DVzreLP8mHYM6yf/view'
---
**Topic.** The title of my M.Sc. thesis was **" Empowering Graph Wavelet Convolution for
Node Classification: A Novel Approach with
Local Lifting Scheme"**. In this thesis work we focused to the phenomenon of production of undesirable wavelet filters within graph wavelet based neural networks and presented a solution framework to overcome this phenemonenon with with our proposed Tree Lifting Scheme. 

**Summary.** Wavelet-based graph neural networks have received increasing attention in various graph machine learning tasks. However, in node classification, existing graph wavelet-based methods are limited in their ability to generalize to arbitrary graphs due to their implementation of predefined wavelet filters with inherent homophilic assumptions while ignoring heterophily. Recent studies have attempted to address this issue through a wavelet lifting transform that requires the bipartite graph, therefore, altering the graph topology, and leading to undesirable wavelet filters. In this thesis, we introduce a novel class of graph wavelet neural network based on our proposed tree-lifting scheme that is able to learn adaptive wavelet filters over arbitrary graphs. Our proposed generalized adaptive graph wavelet network (GA-GWNN) preserves the graph topology through computation trees while implementing the lifting scheme on arbitrary graph structures. Additionally, we concentrate on the local substructure as an acyclic tree while implementing the lifting strategy locally. Moreover, this locally defined lifting scheme incorporates and fuses both high-pass and low-pass frequency components to enhance the feature representation. We further benchmark our proposed GA-GWNN model with three homophilic datasets (Cora, Citeseer, PubMed), and four heterophilic datasets (Film, Cornell, Texas, Wisconsin) and to demonstrate the scalability of our proposed GA-GWNN we evaluated our model on two large-scale datasets namely, Ogbn-Arxiv and Ogbn-Products. In addition, we further introduce a more scaleable and computationally efficient version of GA-GWNN, namely simple and efficient adaptive graph wavelet neural network (SEA-GWNN).
SEA-GWNN incorporates higher-order neighborhoods to extract multiscale information and implements the lifting scheme without the need for an inverse transform. Additionally, SEA-GWNN introduces an attention detachment strategy, enabling the computation of attention parameters only once and re-utilizing them in successive layers, thus making SEA-GWNN more scalable compared to GA-GWNN. Finally, we benchmark this proposed SEA-GWNN on nine real-world homophilic and heterophilic datasets from three categories (i.e., citation, webpage, and film industry graphs) and four large-scale graphs, including Ogbn-Arxiv, Arxiv, Genius, and Penn94. The experimental results from these datasets demonstrate the effectiveness of our method.

**Future Direction.** This work presents Generalized Adaptive Wavelet Network that extends the vanilla lifting scheme on any arbitrary graph thus producing an adaptive graph wavelet based on the signal residing on the graph. *(1)* Extending the work on this topic is an attempt to further reduce the computation cost associated with tree lifting structures. This approach will result in a more fine-grained rehab system. *(2)* One can generalize the proposed framework into many other sectors. For example, the novelty of our framework also can be extended to human activity recognition, augmented reality, gaming, driving, etc. where designing wavelet filters based on the task at hand is crucial. *(3)* Taking one step further, one can extend this proposed fusion model with a learnable aggregation function, where instead of aggregating with a fixed set of edge weights (fixed normalized adjacency matrix), one can learn these edge weights with an attention-based network. But one needs to be careful about the over-parametrization of the entire framework. *(4)* From the theoretical viewpoint, one can further study the effect of over-smoothing on our proposed network. This may result in further analysis of the effect of our two-channel filter bank that was learned through successive lifting structures. This can be observed with the help of the node profile, that analysis the node behavior at each layer.  

More information:
- https://benoitcoasne.github.io/ (Coasne’s research group website)
- https://www.yann-magnin.fr/ (research website)