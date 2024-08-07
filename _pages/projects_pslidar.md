---
layout: archive
title: "Object Detection using Pseudo-LiDAR"
permalink: /projects/pslidar/
author_profile: true
---

**Keywords:** Stereo Depth Estimation, Point Clouds, 3D Object Detection. 

**Source Code:** [Github](https://github.com/ieranik/ps_lidar)

In this project, we implement a novel pipeline for 3D object detection from stereo images using the [Pseudo-LiDAR](https://arxiv.org/abs/1812.07179) framework. The basic Pseudo-LiDAR pipeline takes as input a pair of images and uses a stereo depth estimation network to compute the depth map. Then the depths of the pixels are back-projected in the 3D space to create a point cloud, which is called Pseudo-LiDAR. Finally, a 3D object detection model is employed to identify the 3D objects in the Pseudo-LiDAR point cloud. The pipeline is illustrated in the following figure.

<p align="center">
  <img src="/images/psl_pipeline.png" width="1000"/>
</p> 

A key characteristic of both Pseudo-LiDAR is that any existing stereo depth estimation model and object detection model can be incorporated into the pipeline. In the original version, Pseudo-LiDAR used the state-of-the-art depth estimator, [PSM-Net](https://arxiv.org/abs/1803.08669), and the then best-performing object detectors, [AVOD](https://arxiv.org/abs/1712.02294), for object detection.

<p align="center">
  <img src="/images/psl_sample.png" width="700"/>
</p>


In this project, we integrate a more recent and efficient 3D object detector, called [SFA3D](https://github.com/maudzung/SFA3D), into the pseudo-LiDAR pipeline. We test the performance on the [KITTI dataset](https://ieeexplore.ieee.org/document/6248074). Our initial findings suggest that the integration of SFA3D reduces the number of false positives compared to the existing pseudo-LiDAR variants as can be seen in the above figure. The point clouds with and without depth correction are shown in the right and left columns, respectively, with the ground truth in the middle.




Papers
----

- *Md Ishat-E-Rabban*, Sumedh Koppula, Sparsh Bhogavilli, Venkata Sairam Polina, **3D Object Detection using Artificially Generated LiDAR Data**, [paper](https://ieranik.github.io/files/ps_lidar.pdf)
