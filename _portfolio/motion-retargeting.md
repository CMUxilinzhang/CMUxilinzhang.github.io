---
title: "Motion Retargeting & 3D Human Reconstruction"
excerpt: "A complete pipeline for 3D pose estimation and cross-skeleton motion retargeting.<img src='/images/motionretargeting.png'>"
collection: portfolio
---


This project builds a full pipeline that converts human video into animatable 3D motion sequences using pose estimation and motion retargeting. The social value lies in enabling **low-cost motion capture** for animation, VR/AR performance, teleoperation, and robot imitation learning—without requiring expensive hardware motion-capture systems.

## Objective
Develop a robust and accurate pipeline that extracts 3D human pose from video and retargets the motion across different skeleton structures while preserving physical realism.

## Method
We evaluated multiple pose-estimation baselines such as **OpenPose** and **MotionNet**, then adopted **ThreeDPoseTracker**, which significantly reduces temporal inconsistency and depth prediction errors.  
We reproduced the **Skeleton-Aware Network (SAN)** for motion retargeting, enabling cross-skeleton motion transfer.

Quantitative evaluation metrics included:
- limb-length variation  
- temporal consistency  
- global smoothness  
- BVH mesh penetration  

## Results
3DPoseTracker provided the most stable and clean 3D pose sequences. SAN produced smoother, physically plausible motion reconstructions with lower collision and penetration rates across multiple skeleton topologies.  
The pipeline demonstrates strong potential for generating training data for reinforcement learning and virtual avatar control.

<!-- ## My Role
I contributed to:
- pipeline integration and evaluation  
- SAN implementation  
- metric design and evaluation  
- visualization using Blender   -->
