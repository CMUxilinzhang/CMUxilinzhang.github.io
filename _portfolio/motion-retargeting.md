---
title: "Pose Estimation and Motion Retargeting for Virtual Reconstruction"
excerpt: >
  A hybrid system combining TDPT pose estimation and SAN-based motion retargeting for realistic virtual reconstruction.<br/>
  <img src="/images/motionretargeting.png">
collection: portfolio
---


## Introduction  
Accurate motion reconstruction is essential for **robot imitation learning, animation, and human–robot interaction**. Existing pipelines struggle with occlusion, motion jitter, and cross-skeleton retargeting errors.  
**Objective:** build an end-to-end system that converts raw RGB videos into clean, retargeted 3D motions suitable for robotics and virtual avatars.

## Methods  
Following the pipeline in :contentReference[oaicite:5]{index=5}:
- **ThreeDPoseTracker (TDPT)** for robust 3D joint rotations (BVH output).  
- **Skeleton-Aware Network (SAN)** trained on Mixamo for motion retargeting across different skeletons.  
- **Blender-based quantitative evaluation** for penetration, smoothness, and positional error.

## Results  
- TDPT achieves **0.0468 temporal inconsistency** and **5.71% limb-length variation**, outperforming OpenPose+MotioNet.  
- SAN achieves **147 FPS** and low positional error (0.87% intra-structure, 2.54% cross-structure).  
- Our pipeline significantly reduces mesh penetration compared to AutoRigPro (50.24% → 28.85%).

## Discussion  
By combining reliable pose estimation with structure-aware retargeting, the system offers more realistic and physically consistent motion. Remaining challenges include handling extreme poses, domain shifts, and skeleton mismatch.

## My Contribution  
I implemented the retargeting pipeline, established evaluation metrics, generated Blender visualizations, and co-authored the full analysis.  
