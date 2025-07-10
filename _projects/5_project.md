---
layout: page
title: Multi-Drone Coordination
description: Autonomous navigation
img: assets/img/pluto.jpg
importance: 3
category: <
---

# Autonomous Drone Control Using ArUco Tags

This project involved designing and implementing an autonomous control framework for drones to achieve accurate pose estimation and coordinated flight. The work focused on leveraging ArUco markers for precise localization and enabling advanced functionalities like hovering, trajectory following, and multi-drone coordination.

## Key Features and Contributions

### 1. **Accurate Pose Estimation with ArUco Tags**

- Used a single monocular camera for real-time pose estimation of drones by detecting and interpreting ArUco tags.
- Achieved high accuracy in determining the drone’s position and orientation relative to the marker, forming the basis for precise control.

### 2. **Autonomous Hovering and Trajectory Execution**

- Designed and implemented a control system for a drone to:
  - Hover at a specified height using real-time pose feedback.
  - Move autonomously in a rectangular trajectory (1 x 2 meters) while maintaining stability.

### 3. **Multi-Drone Coordination**

- Developed a leader-follower framework, where a second drone autonomously followed the trajectory of the first drone in real time.
- Ensured seamless coordination between drones using continuous pose estimation and control adjustments.

## Key Achievements

- Demonstrated autonomous hovering and precise trajectory following in dynamic scenarios.
- Successfully implemented multi-drone coordination, paving the way for scalable swarm robotics applications.
- Highlighted the effectiveness of using monocular vision and ArUco tags for low-cost, accurate drone localization and control.

<iframe width="930" height="500" src="https://www.youtube.com/embed/PdnE_47Gra4?si=VHnNhFGGLldkTy8q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
