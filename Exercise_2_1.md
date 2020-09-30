# Exercise 2.1

## A comprehensive Survey on Graph Neural Networks

**1. How are network embeddings and GCNs related?**

With Network Embeddings a low-dimensional representation of the nodes within a network can be represented while preserving the network structure. Further, these representations can be used for training common machine learning algorithms for downstream tasks such as classification, clustering…
One of approaches to generate Network embeddings are autoencoder algorithms.  In this system, the encoder uses Graph Convolutional Network layers  to get the representations of each node.

**2. What are the potential outputs of GCNs? Please describe one use-case for each potential output.**


**3. What value is added by Graph Attention Networks over GCNs? What are the potential disadvantages?**


**4. Why are GCNs relevant for computer vision?**

Many computer vision tasks can leverage on the semantic relationships of objects inside a picture or video. For instance, point clouds can represent different objects in a 2D or 3D space, and its topologies can be explored with graph convolution networks.
Alternative approaches are human action recognition, where human bodies ar a set of connected edges which represent the human skeleton. Further, spatial-temporal analysis of the skeleton can represent action patterns.
