---
layout: archive
title: "Visibility Color Map Construction in Spatial Databases"
permalink: /projects/vcm/
author_profile: true
---

**Keywords:** Geometric Projections, Spatial Databases, R-Tree.


{% include youtubePlayer.html id="KJrx2J0N8ZA" %}

In this project, I worked on the Visibility Color Map (VCM) problem. I used tools from computational geometry, graph theory, and spatial databases to efficiently solve these queries. 

<p align="center">
  <img src="/images/vcm.png" width="450" />
</p> 

The VCM problem is to assign a color value to each point in the space denoting the visibility measure of a given extended target object from the point. In the existing solutions to the VCM problem, a viewpoint is simply discarded (i.e., considered as non-visible) if an obstacle even slightly blocks the view of the target from the viewpoint, which restricts its applicability for a wide range of scenarios. To alleviate this limitation, in this paper, we propose a scalable, efficient and comprehensive solution to construct a VCM for a fixed target that considers the partial visibility of the target. We index the obstacles in a spatial data structure called R-tree and use a projection-based idea to efficiently construct the VCM as outlined in the above figure. More importantly, our proposed data structures for the fixed target support incremental updates of the VCM if the target moves to nearby positions. Our experimental results show that our approach is orders of magnitude faster than the baseline technique.


{% include youtubePlayer.html id="7C0u7YufaqI" %}



Publications
----

- Arif Arman, Kaysar Abdullah, *Md Ishat-E-Rabban*, Mohammed Eunus Ali, **IndVizCMap: Visibility Color Map in an Indoor 3D Space**, Proceedings of the 24th ACM SIGSPATIAL, 2016.
[paper](https://ieranik.github.io/files/indvizcmap.pdf)

- *Md Ishat-E-Rabban*, Kaysar Abdullah, Mohammed Eunus Ali, Muhammad Aamir Cheema, **Visibility Color Map for a Fixed or Moving Target in Spatial Databases**, Proceedings of the 14th International Symposium on Spatial and Temporal Databases, 2015.
[paper](https://ieranik.github.io/files/mvcm.pdf)

- *Md Ishat-E-Rabban*, Kaysar Abdullah, Shibbir Ahmed, M Sohel Rahman, **An easier approach to visible edge determination from moving viewpoint**, International Conference on Electrical Engineering and Information & Communication Technology, 2014.

- Farhana Murtaza Choudhury, Mohammed Eunus Ali, Sarah Masud, Suman Nath, *Md Ishat-E-Rabban*, **Scalable Visibility Color Map Construction in Spatial Databases**, Information Systems Journal, volume 42, 2014.
[paper](https://ieranik.github.io/files/vcm.pdf)



