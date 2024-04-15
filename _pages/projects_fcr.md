---
layout: archive
title: "Fast Connectivity Restoration"
permalink: /projects/fcr/
author_profile: true
---

**Keywords:** Graph Theory, Quadratic Optimization, Multi-Robot Systems. 

In this project, we investigate the problem of making a network *k*-connected while minimizing robot movements. The input to this problem is a set of robot positions and the integer value *k*. Here, we assume a disk communication model with communication radius h. The goal is to find new positions of the robots which form a k-connected topology while minimizing the maximum distance between the previous and new positions of the robots, i.e., the minmax distance. We call this problem the Fast k-connectivity Restoration (FCR) problem. An example of
the FCR problem instance is shown in the following video. In the examples shown in the video, the robots moves towards higher degree of connectivity while minimizing the length of the path travelled be the robots. 

{% include youtubePlayer.html id="ehlxi9v4qxw" %}

We have developed a Quadratically Constrained Program (QCP) formulation of the FCR problem, which is based on the idea of multi-commodity network flow. The QCP formulation enables us to solve the FCR problem optimally using a QCP solver. However, the QCP formulation can be used to solve only small instances of the FCR problem due to high computational overhead.

We therefore propose a scalable algorithm, EA-SCR, to solve the FCR problem which requires less computational time than the optimal QCP-based algorithm. The EA-SCR algorithm solves the FCR problem by dividing it into two phases. In the first phase, we find a set of edges that, if augmented to the input network, make the network *k*-connected, and the maximum cost of the augmented edges is minimized. Here the cost of an edge is proportional to the Fast k-connectivity Restoration distance between the two corresponding robots. We call this Graph Topology Optimization (GTO) problem. We solve the GTO problem by first sorting the non-existent edges of the communication graph in increasing order of weight, and then keep adding the edges in order until the graph becomes k-connected. In the second phase, we move the robots in such a way that the edges obtained from the first phase is established, and the maximum distance traveled by a robot is minimized. We call this Movement Minimization (MM) problem. To solve the MM problem, we propose a Breadth First Search (BFS) based idea called cascaded relocation, which establishes the edges obtained from the first phase without removing any existing edges.

We conduct extensive experimentation to evaluate the performance of our proposed algorithm. The empirical results show that the EA-SCR algorithm generates solutions which are within 10% of the optimal solution and gives 30% lower minmax distance than all existing FCR algorithms as listed below. 

* [Movement control algorithms for realization of fault-tolerant ad hoc robot networks](https://ieeexplore.ieee.org/document/1316760)
* [Movement-Assisted Connectivity Restoration in Wireless Sensor and Actor Networks](https://ieeexplore.ieee.org/document/4689552)
* [Establishing Fault-Tolerant Connectivity of Mobile Robot Networks](https://ieeexplore.ieee.org/document/9454397)


{% include youtubePlayer.html id="AYcu3Itwqc4" %}

We also test the EA-SCR algorithm in action by performing a hardware experiment using 6 drones. A video of the hardware experiment in given above. The source code for this project can be found in this [github repository](https://github.com/ieranik/fbr).



Tools Used
----

* [Gurobi](https://www.gurobi.com/solutions/gurobi-optimizer)
* [OpenGL](https://open.gl/)
* [CrazyFlie](https://www.bitcraze.io/products/crazyflie-2-1/)



Publications
----

- *Md Ishat-E-Rabban*, Guangyao Shi, Griffin Bonner, Pratap Tokekar, **Fast k-connectivity Restoration in Multi-Robot Systems for Robust Communication Maintenance**, arXiv preprint arXiv:2404.03834, 2024.
[paper](https://ieranik.github.io/files/fcr.pdf)


- *Md Ishat-E-Rabban* , Guangyao Shi, Pratap Tokekar, **Fast Biconnectivity Restoration in Multi-Robot Systems for Robust Communication Maintenance**, arXiv preprint arXiv:2011.00685, 2023.
[paper](https://ieranik.github.io/files/fbr.pdf)


- Guangyao Shi, *Md Ishat-E-Rabban*, Lifeng Zhou, Pratap Tokekar, **Communication-Aware Multi-robot Coordination with Submodular Maximization**, IEEE International Conference on Robotics and Automation, Pages 8955-8961, 2021.
[paper](https://ieranik.github.io/files/csm.pdf)