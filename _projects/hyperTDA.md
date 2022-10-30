---
layout: page
title: hyperTDA
description: Topology & Hypergraphs
img: assets/img/PH_hypergraph2.png
importance: 2
category: research
---

Persistence diagrams summarize the presence of loops in data. However, they do not inform us of where the loops are. Can we understand which points are “integral” to the overall structure of the data? The goal is to develop a quantification of each point in the data according to its contribution to the overall structure.There are two challenges. The first is that, given a persistence diagram, localizing the loops in a concise and interpretable way is an NP-hard problem. The second is the lack of methods to consolidate all loop information.
To address the first challenge, I developed a method called <a href="https://github.com/irishryoon/minimal_generators_curves">minimal generators</a> that outputs a small and interpretable collection of data (generators) that represents the loops. I utilize a recent technique of performing the optimization over rational coefficients to circumvent the NP-hardness of the problem. 
To consolidate all generators, my collaborators and I utilized hypergraphs, a generalization of a graph whose edges are collections of two or more vertices. We constructed a PH-hypergraph that has the original data as the vertex set and whose hyperedges are the generators of a persistence diagram. To encode the “importance” of each point of the persistence diagram, we weighed the hyperedge according to the persistence (the distance between a point and the diagonal line in the persistence diagram). Figure 1 illustrates the construction.

<p align="center">
  <img width="750" src="https://irisyoon.com/assets/img/hyperTDA.png">
</p>
<div class="caption">
Figure 1. Pipeline for constructing and analyzing PH-hypergraph. <span style="font-weight:bold">A.</span> Given point cloud data, we compute the persistencediagram that summarizes the presence of loops. For each point in the persistence diagram, we compute the generator (collectionof vertices representing the loops). We then construct a hypergraph whose vertex set is the original data and whose hyperedges are the generators. <span style="font-weight:bold">B.</span> We analyze the PH-hypergraph via hypergraph centrality and community detection.
</div>

We use graph theory and network science to study the PH-hypergraph. We first compute hypergraph centrality, which ranks the original data according to their participation in large loops. We also perform community detection, which partitions the data according to how often a collection of points constitutes ashared loop. See Figure 1B for the complete method. See Figure 2 for examples of outputs.

<p align="center">
  <img width="750" src="https://irisyoon.com/assets/img/hyperTDA_outputs.png">
</p>
<div class="caption">
Figure 2. Outputs of hypergraph analysis on a random curve. (Left) PH-centrality assigns a high importance score to verticesthat constitute the large loop in the center. (Right) PH-community reflects which subsets of data constitute the same loop.
</div>
The method, called <a href="https://github.com/degnbol/hyperTDA">hyperTDA,</a> identifies subsets of data integral to the overall structure and partitions the data into functional modules. We validated our method on simulated and experimental data, including diffusion of particles and animal movement trajectories.

Preprint: <a href="https://arxiv.org/abs/2210.07545">Hypergraphs for multiscale cycles in structured data</a>
 
Code: <a href="https://github.com/degnbol/hyperTDA">github:hyperTDA</a>

*Joint work with Agnese Barbensi (University of Melbourne), Christian Madsen (University of Melbourne), Deborah Ajayi (University of Ibadan), Heather Harrington (University of Oxford), and Michael Stumpf (University of Melbourne).*

