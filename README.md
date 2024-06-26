# Improving Localization Reliability with Path Planning
Perception-aware path planning metric design. Submission to IROS2024.
## Introduction
Just as even humans can get lost in the face of extremely monotonous or blurry observations from the eyes, not all scenarios are favorable for robot localization. To address this challenge, our objective is to identify areas that are favorable for robot localization. Existing assessment methods mainly focus on the richness of observed features, which results in potential failures when facing scenarios involving cluttered features and severe noise interference. In this paper, we propose a metric that considers these factors by introducing perturbations into the observations and analyzing how the intensity and direction of the perturbations affect pose estimation. We validate the effectiveness of our proposed metric through benchmark comparisons in various scenarios. Furthermore, we implement a planning framework that incorporates the proposed metric, enabling robots to make intelligent decisions by selecting localization-friendly topologies and sensor orientations.

<div align="center">
<img src="archieve/head.png" title="result image" width=75%/>
</div>

As the **above Figure** shows, the proposed metric is used to identify localization-friendly areas. Figure (c) illustrates the complete scene, while Figures (a) and (b) depict localized views within the scene. Figure (d) shows the result of evaluating this scenario using the proposed metric, where larger values indicate poorer observation quality and areas with a value of 0.0 indicate obstacles. The main sensor of the localization system is a rotating LiDAR, and the observation equation of the localization system is defined as the distance between the LiDAR point and the nearest plane.

## vedio
Click on the image below to watch the experimental video:

[![Watch the video](archieve/bilibili.png)](//player.bilibili.com/player.html?aid=916491163&bvid=BV1tu4y147L5&cid=1279018108&p=1)

## preprint paper
The paper is submitted to ICRA2024, which is under review now. Click [here](archieve/ICRA2024_Perception_Aware.pdf) to see the preprint version.


