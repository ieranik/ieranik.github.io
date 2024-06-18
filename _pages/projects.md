---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---


Spatial Data Querying and Processing 
----

<table style="border-collapse: separate; border: none; border-spacing:25px 25px;" align="left">
	<tr>
		<td style="border: none;" align="left" width="400"> <p><img src="/images/mvfs.png" /></p>  </td>
		<td style="border: none;" align="left">
			<span style="color:black; font-size:16px"> 
			<b>Maximum Visibility Facility Selection (MVFS)</b><br>
			The MVFS query involves selecting *k* out of the *n* locations, that yield the maximum visibility coverage of the data space in the presence of a large obstacle set. I used tools from computational geometry, graph theory, spatial databases, and integer programming to develop an algorithm that was able to efficiently solve 2X larger instances of the MVFS problem compared to existing solutions. [<a href="https://ieranik.github.io/projects/vqsd/">Project Page</a>]
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
		<td style="border: none;" align="left" width="400"> <p><img src="/images/kafka.png" /></p>  </td>
		<td style="border: none;" align="left">
			<span style="color:black; font-size:16px"> 
			<b>Data Streaming with Spark and Kafka</b><br>
			This is a data streaming application developed using Apache Spark, Kafka, MySQL, and Scala. In this streaming service, the Kafka producer writes events to a Kafka topic, which are sent to a MySQL database. A web server is also created to view the dashboard. [<a href="https://github.com/ieranik/spark_kafka_stream">Project Page</a>]
			</span>
		</td>
	</tr>
</table>



Deep Learning for Robotics
----

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
		<td style="border: none;" align="left" width="400"> <p><img src="/images/hc.png" /></p>  </td>
		<td style="border: none;" align="left">
			<span style="color:black; font-size:16px"> 
			<b>Heterogeneous Coordination using Particle Filters and Reinforcement Learning</b><br>
			We investigate the performance of a heterogeneous multi-robot team consisting of one UAV and multiple UGVs in the context of the persistent monitoring task. We develop a particle filter based algorithm for UGV path planning and an actor-critic reinforcement learning architecture for UAV path planning resulting in reduced positional uncertainty and improved task performance. [<a href="https://ieranik.github.io/projects/hcrl/">Project Page</a>]
			</span>
		</td>
	</tr>
	<tr>
		<td style="border: none;" align="left" width="400"> <p><img src="/images/psl_sample.png" /></p>  </td>
		<td style="border: none;" align="left">
			<span style="color:black; font-size:16px"> 
			<b>Object Detection using Pseudo-LiDAR</b><br>
			Pseudo-LiDAR is a novel pipeline for 3D object detection from stereo images. The basic Pseudo-LiDAR pipeline takes as input a pair of images and uses a stereo depth estimation network to compute the depth map. Then the depths of the pixels are back-projected in the 3D space to create a point cloud, which is called Pseudo-LiDAR. Finally, a 3D object detection model is employed to identify the 3D objects in the Pseudo-LiDAR point cloud. [<a href="https://ieranik.github.io/projects/pslidar/">Project Page</a>]
			</span>
		</td>
	</tr>
</table>



Multi-Robot Systems
----

<table style="border-collapse: separate; border: none; border-spacing:25px 25px;" align="left">
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
		<td style="border: none;" align="left" width="400"> {% include youtubePlayer.html id="m8KrN-kRqSE" %} </td>
		<td style="border: none;" align="left">
			<span style="color:black; font-size:16px"> 
			<b>Resilient Multi-Robot Task Optimization</b><br>
			Resilient Task Optimization for multi-robot systems involves selecting trajectories for each robot such the task performance is maximized in the case of a worst-case failure of at most α robots. I have developed two algorithms for the resilient coverage maximization task based on greedy heuristic, and local search technique, which gives higher task performance compared to existing approaches. The proposed solution is also tested using a persistent monitoring case study. [<a href="https://ieranik.github.io/projects/rmrto/">Project Page</a>]
			</span>
		</td>
	</tr>
</table>
