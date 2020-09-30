# Exercise 2.1

## A comprehensive Survey on Graph Neural Networks

**1. How are network embeddings and GCNs related?**

With Network Embeddings a low-dimensional representation of the nodes within a network can be represented while preserving the network structure. Further, these representations can be used for training common machine learning algorithms for downstream tasks such as classification, clustering…
One of approaches to generate Network embeddings are autoencoder algorithms.  In this system, the encoder uses Graph Convolutional Network layers  to get the representations of each node.

**2. What are the potential outputs of GCNs? Please describe one use-case for each potential output.**

GCNs can look at three different levels in graphs; node-, edge-, and graph-level.

Node-level:
- This can be as simple as classifying nodes. This has a wide range of use-cases, an example could be detection of malicious actors in a network.

Edge-level:
- Again, this can be classification, like the node-level, but for edges instead. Another use-case could be finding connection values in a similarity graph, something that is often found in biological networks.

Graph-level:
- Instead of looking at the individual nodes or edges, we look at the entire graph. Use-cases for this could be community classification. One could imagine a scenario in which we have graphs of different cities, and some nodes in each graph describing which political party a person would vote for. We could imagine that the political a person/node has, is influenced by their neighbors. We could thus classify which party a city would vote for.

**3. What value is added by Graph Attention Networks over GCNs? What are the potential disadvantages?**

This describes the 2017 paper Graph Attention Networks by Petar Veličković et. al., there has since been done further research.

GATs increase the expressive power by not assuming the contribution of neighboring nodes are pre-determined like the GCN. A GAT can, by it's attention mechanism, have different weights for different nodes in a given neighborhood.

The main drawback of the GAT is the high compute cost, as the cost is O(n^4), where n is the amount of nodes in a graph. This makes it unviable for larger networks.

**4. Why are GCNs relevant for computer vision?**

Many computer vision tasks can leverage on the semantic relationships of objects inside a picture or video. For instance, point clouds can represent different objects in a 2D or 3D space, and its topologies can be explored with graph convolution networks.
Alternative approaches are human action recognition, where human bodies ar a set of connected edges which represent the human skeleton. Further, spatial-temporal analysis of the skeleton can represent action patterns.
