---
layout: archive
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

About Me
====

Hi. I am Ishat, a CS masters student at [the University of Maryland College Park](https://www.cs.umd.edu/) (UMD) working with Dr. Pratap Tokekar. I conduct research on multi-robot systems with a focus on developing learning-based planners and ensuring resilience of robot teams performing optimization tasks. Before joining UMD, I spent 5 years at [Bangladesh University of Engineering and Technology](https://cse.buet.ac.bd/) (BUET) as a faculty member and IT consultant. During my time at BUET, I also performed research on efficient processing of visibility queries on spatial databases. 

My academic explorations span diverse fields of computer science including deep learning, robotics, spatial/graph data processing and visualization, etc. I have significant experience with deep learning architectures for single and multi-agent path planning and perception, which include graph neural networks, transformers, actor-critic networks, objection detectors, depth estimators, etc. In my body of research, I have extensively applied and developed techniques from graph theory (e.g., partitioning, maximum flow, matching, etc.) and computational geometry (e.g., triangulation, projective transforms, visible-surface determination) on large datasets. I am also skilled at creating cool demos using 3D visualization tools and renderers. 

My hobbies include poetry, cricket, and puzzles. I love working with people, both as a mentor and mentee. I am graduating from UMD in spring 2024, and I am excitedly looking forward to starting the next phase of my life as a software engineer. 
  



Projects
======

<table style="border-collapse: separate; border: none; border-spacing:25px 25px;" align="left">
	<tr>
		<td style="border: none;" align="left" width="400"> {% include youtubePlayer.html id="BvKpqHFJBXo" %} </td>
		<td style="border: none;" align="left">
			<span style="color:black; font-size:16px"> 
			<b>Deep Mapping and Path Planning</b><br>
			We propose a memory-enabled deep neural architecture for multi-robot navigation in a structured environment. The architecture uses value iteration networks to solve the path planning task, and graph neural networks to facilitate inter-robot communication by exchanging environment embeddings. Our proposed model outperforms the state-of-the-art in both simple and complex occupancy maps, resulting in 5% and 30% increase in action selection accuracy respectively. [<a href="https://ieranik.github.io/projects/dmpp/">Project Page</a>]
			</span>
		</td>
	</tr>
	<tr>
		<td style="border: none;" align="left" width="400"> {% include youtubePlayer.html id="ehlxi9v4qxw" %} </td>
		<td style="border: none;" align="left">
			<span style="color:black; font-size:16px"> 
			<b>Fast Connectivity Restoration</b><br>
			The Fast Connectivity Restoration (FCR) problem involves relocating a team of robots such that their underlying network becomes <i>k</i>-connected and the maximum robot movement is minimized. I have developed a Quadratically Constrained Program (QCP) formulation to optimally solve the FCR problem, and also a scalable heuristic graph-theoretic algorithm that gives lower running time. Experiments show that our proposed solution outperforms all existing algorithms. [<a href="https://ieranik.github.io/projects/fcr/">Project Page</a>]
			</span>
		</td>
	</tr>
	<tr>
		<td style="border: none;" align="left" width="400"> {% include youtubePlayer.html id="KJrx2J0N8ZA" %}  </td>
		<td style="border: none;" align="left">
			<span style="color:black; font-size:16px"> 
			<b>Visibility Color Map (VCM) Construction</b><br>
			The VCM is a color map that assigns a value to each point in the 3D space denoting the visibility measure of a given extended target object from the point in the presence of a city-scale large set of obstacles indexed in a spatial data structure. I developed algorithmic tools to address limitations of existing works on VCM construction and accelerated VCM query processing by two orders of magnitude. [<a href="https://ieranik.github.io/projects/vcm/">Project Page</a>]
			</span>
		</td>
	</tr>
	<tr>
		<td style="border: none;" align="left" width="400"> <p><img src="/images/hc.png" /></p>  </td>
		<td style="border: none;" align="left">
			<span style="color:black; font-size:16px"> 
			<b>Heterogeneous Coordination using Particle Filters and Reinforcement Learning</b><br>
			We investigate the performance of a heterogeneous multi-robot team consisting of one UAV and multiple UGVs in the context of the persistent monitoring task. We develop a particle filter based algorithm for UGV path planning and an actor-critic reinforcement learning architecture for UAV path planning resulting in reduced positional uncertainty and improved task performance. [<a href="https://ieranik.github.io/projects/hcrl/">Project Page</a>]
			</span>
		</td>
	</tr>
	<tr>
		<td style="border: none;" align="left" width="400"> {% include youtubePlayer.html id="m8KrN-kRqSE" %} </td>
		<td style="border: none;" align="left">
			<span style="color:black; font-size:16px"> 
			<b>Resilient Multi-Robot Task Optimization</b><br>
			Resilient Task Optimization for multi-robot systems involves selecting trajectories for each robot such the task performance is maximized in the case of a worst-case failure of at most α robots. I have developed two algorithms for the resilient coverage maximization task based on greedy heuristic, and local search technique, which gives higher task performance compared to existing approaches. The proposed solution is also tested using a persistent monitoring case study. [<a href="https://ieranik.github.io/projects/rmrto/">Project Page</a>]
			</span>
		</td>
	</tr>
</table>


[See all projects >>](https://ieranik.github.io/projects/)


Publications
======

- *Md Ishat-E-Rabban*, Guangyao Shi, Griffin Bonner, Pratap Tokekar, **Fast k-connectivity Restoration in Multi-Robot Systems for Robust Communication Maintenance**, arXiv preprint arXiv:2404.03834, 2024.
[paper](https://ieranik.github.io/files/fcr.pdf)
[code](https://github.com/ieranik/fbr)

- *Md Ishat-E-Rabban*, Pratap Tokekar, **D2M2N: Decentralized Differentiable Memory-Enabled Mapping and Navigation for Multiple Robots**, arXiv preprint arXiv:2310.07070, 2023.
[paper](https://ieranik.github.io/files/D2M2N.pdf)
[code](https://github.com/ieranik/d2m2n)

- *Md Ishat-E-Rabban*, Pratap Tokekar, **Failure-Resilient Coverage Maximization With Multiple Robots**, IEEE Robotics and Automation Letters, volume 6, Issue 2, 2021.
[paper](https://ieranik.github.io/files/rcm.pdf)
[code](https://github.com/ieranik/rcm)

- Guangyao Shi, *Md Ishat-E-Rabban*, Lifeng Zhou, Pratap Tokekar, **Communication-Aware Multi-robot Coordination with Submodular Maximization**, IEEE International Conference on Robotics and Automation, Pages 8955-8961, 2021.
[paper](https://ieranik.github.io/files/csm.pdf)

- *Md Ishat-E-Rabban*, Mohammed Eunus Ali, Muhammad Aamir Cheema, Tanzima Hashem, **The Maximum Visibility Facility Selection Query in Spatial Databases**, Proceedings of the 27th ACM SIGSPATIAL, 2019.
[paper](https://ieranik.github.io/files/mvfs.pdf)
[code](https://github.com/ieranik/mvfs)

- *Md Ishat-E-Rabban*, Kaysar Abdullah, Mohammed Eunus Ali, Muhammad Aamir Cheema, **Visibility Color Map for a Fixed or Moving Target in Spatial Databases**, Proceedings of the 14th International Symposium on Spatial and Temporal Databases, 2015.
[paper](https://ieranik.github.io/files/mvcm.pdf)


[See all publications >>](https://ieranik.github.io/publications/)