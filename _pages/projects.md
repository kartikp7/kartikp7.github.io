---
layout: archive
title: ""
permalink: /projects/
author_profile: true
---

D-SLAM: Monocular Visual SLAM with Depth Prediction
====

* A RGB-D SLAM system that performs both **D**epth estimation and **SLAM** with monocular camera input. See project on github [here](https://github.com/zxcvbnmditto/D-SLAM).

* D-SLAM combines [monodepth2](https://github.com/nianticlabs/monodepth2), an open source project for deep learning-based depth estimation from monocular video input and [ORBSLAM2](https://github.com/raulmur/ORB_SLAM2) a popular open-source SLAM library. I benchmarked accuracy and runtime results on KITTI odometry dataset.

* D-SLAM system was deployed on workstation with NVIDIA GeForce GTX 1080Ti at 14FPS and embedded device NVIDIA Jetson TX2 RaceCar at 3.3 FPS. 

* Project won Outstanding Senior Design Project Award in UC Davis ECE Department.

<div style="display: flex; justify-content: space-between;">
  <div style="width: 48%;">
    <p>D-SLAM on KITTI dataset (GeForce GTX 1080Ti)</p>
    <video width="100%" controls>
      <source src="/vids/dslam_demo.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="width: 48%;">
    <p>D-SLAM in Kemper Hall, UC Davis (NVIDIA Jetson TX2)</p>
    <video width="100%" controls>
      <source src="/vids/tx2-demo.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

----

<!-- <div style="display: flex; justify-content: space-between;">
  <div style="width: 48%;">
    <p>D-SLAM on KITTI dataset (GeForce GTX 1080Ti)</p>
    <iframe src="https://drive.google.com/file/d/1Y53K2F81Wujuj8V1DhDYEtA_Srf-ca_S/view" width="100%" height="315" frameborder="0"></iframe>
  </div>

  <div style="width: 48%;">
    <p>D-SLAM in Kemper Hall, UC Davis (NVIDIA Jetson TX2)</p>
    <iframe src="https://drive.google.com/file/d/1v1yON3g1UNTW7SDlc7nQcAPV72MbT5ss/view" width="100%" height="315" frameborder="0"></iframe>
  </div>
</div> -->
