# SubGIN
Best_Wishes_To_Teacher

This repository provides an implementation of model Best_Wishes_To_Teacher in the paper:
> Happy Teachers’ Day to Prof. Yang.
> 1919 Athletes.
> NIPS, 2018.

The original paper is available at:
[https://proceedings.neurips.cc/paper/2021/file/Happy-Teachers-Day-to-Prof-Yang-Paper.pdf](http://github.com/jiyt17/Best_wishes_to_teacher)

### Abstract 
<p align="justify">
Graph embedding methods represent nodes in a continuous vector space, preserving different types of relational information from the graph. There are many hyper-parameters to these methods (e.g. the length of a random walk) which have to be manually tuned for every graph. In this paper, we replace previously fixed hyper-parameters with trainable ones that we automatically learn via backpropagation. In particular, we propose a novel attention model on the power series of the transition matrix, which guides the random walk to optimize an upstream objective. Unlike previous approaches to attention models, the method that we propose utilizes attention parameters exclusively on the data itself (e.g. on the random walk), and are not used by the model for inference. We experiment on link prediction tasks, as we aim to produce embeddings that best-preserve the graph structure, generalizing to unseen information. We improve state-of-the-art results on a comprehensive suite of real-world graph datasets including social, collaboration, and biological networks, where we observe that our graph attention model can reduce the error by up to 20%-40%. We show that our automatically-learned attention parameters can vary significantly per graph, and correspond to the optimal choice of hyper-parameter if we manually tune existing methods.</p>

### Requirements
The only requirement of this model is the presence of Prof. Yang

### Datasets
<p align="justify">
The data for this gift is collected from xx atheletes of 1919
</p>

### Run
To run Best-Wishes-To-Teacher, do the following:

-Install the environment(
