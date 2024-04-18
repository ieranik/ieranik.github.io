---
layout: archive
title: "Visibility Queries in Spatial Databases"
permalink: /projects/vqsd/
author_profile: true
---

**Keywords:** Computational Geometry, Spatial Databases, R-Tree, Graph Partitioning.


In this project, I studied several visibility queries in the presence of a city-scale large set of obstacles indexed in a spatial data structure. I worked extensively on the Maximum Visibility Facility Selection (MVFS) and the Visibility Color Map (VCM) problem. I used tools from computational geometry, graph theory, and spatial databases to efficiently solve these queries. 

<p align="center">
  <img src="/images/mvfs.png" width="500"/>
</p> 

In the MVFS problem, we are given a large set of obstacles in 2D or 3D space, a set of *n* candidate locations where facilities can be established. The MVFS query finds *k* out of the *n* locations, that yield the maximum visibility coverage of the data space. A sample instance of the MVFS problem with *n*=5 and *k*=3 is shown in the figure above. 

Though the MVFS problem has been extensively studied in visual sensor networks, computational geometry, and computer vision in the form of the optimal camera placement problem, existing solutions are designed for discretized space and only work for MVFS instances having a few hundred facilities. To this end, we introduce the concept of equivisibility triangulation to devise the first approach to accurately determine the visibility coverage of continuous data space from a subset of the facility locations, which avoids the limitations of discretizing the data space. Then, we propose an efficient graph-theoretic approach that exploits the idea of vertex separators for an efficient exact in-memory solution to the MVFS problem. Finally, we propose the first external-memory approximation algorithm that is scalable for a large number of obstacles and facility locations. We conduct an extensive experimental study to show the effectiveness and efficiency of our proposed algorithms. The source code for this project can be found in this [Github repository](https://github.com/ieranik/mvfs).

<p align="center">
  <img src="/images/vcm.png" width="450" />
</p> 

The VCM problem is to assign a color value to each point in the space denoting the visibility measure of a given extended target object from the point. In the existing solutions to the VCM problem, a viewpoint is simply discarded (i.e., considered as non-visible) if an obstacle even slightly blocks the view of the target from the viewpoint, which restricts its applicability for a wide range of scenarios. To alleviate this limitation, in this paper, we propose a scalable, efficient and comprehensive solution to construct a VCM for a fixed target that considers the partial visibility of the target. We index the obstacles in a spatial data structure called R-tree and use a projection-based idea to efficiently construct the VCM as outlined in the above figure. More importantly, our proposed data structures for the fixed target support incremental updates of the VCM if the target moves to nearby positions. Our experimental results show that our approach is orders of magnitude faster than the baseline technique.



Publications
----

- *Md Ishat-E-Rabban*, Mohammed Eunus Ali, Muhammad Aamir Cheema, Tanzima Hashem, **The Maximum Visibility Facility Selection Query in Spatial Databases**, Proceedings of the 27th ACM SIGSPATIAL, 2019.
[paper](https://ieranik.github.io/files/mvfs.pdf)

- Arif Arman, Kaysar Abdullah, *Md Ishat-E-Rabban*, Mohammed Eunus Ali, **IndVizCMap: Visibility Color Map in an Indoor 3D Space**, Proceedings of the 24th ACM SIGSPATIAL, 2016.
[paper](https://ieranik.github.io/files/indvizcmap.pdf)

- *Md Ishat-E-Rabban*, Kaysar Abdullah, Mohammed Eunus Ali, Muhammad Aamir Cheema, **Visibility Color Map for a Fixed or Moving Target in Spatial Databases**, Proceedings of the 14th International Symposium on Spatial and Temporal Databases, 2015.
[paper](https://ieranik.github.io/files/mvcm.pdf)

- *Md Ishat-E-Rabban*, Kaysar Abdullah, Shibbir Ahmed, M Sohel Rahman, **An easier approach to visible edge determination from moving viewpoint**, International Conference on Electrical Engineering and Information & Communication Technology, 2014.

- Farhana Murtaza Choudhury, Mohammed Eunus Ali, Sarah Masud, Suman Nath, *Md Ishat-E-Rabban*, **Scalable Visibility Color Map Construction in Spatial Databases**, Information Systems Journal, volume 42, 2014.
[paper](https://ieranik.github.io/files/vcm.pdf)



