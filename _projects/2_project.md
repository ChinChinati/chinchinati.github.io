---
layout: page
title: Quadrupedal Robot 
description: 12DOF Legged Robot Development
img: assets/img/shiro.png
importance: 4
category: <
related_publications: false
---

### <a href="https://github.com/ChinChinati/Shiro">[code]</a>
### <a href="https://github.com/ChinChinati/shiro_description">[ROS Package]</a> with trained RL Policy
# Locomotion Control Framework for Quadrupedal Robots  

This project focused on the end-to-end design and implementation of a robust locomotion control framework for quadrupedal robots. The aim was to develop a system capable of executing diverse gaits while adapting to varying environmental conditions, such as unstructured terrains. By integrating traditional control techniques with advanced reinforcement learning, the project successfully demonstrated versatility, adaptability, and efficient performance for real-world applications.  

## Key Features and Contributions  

### 1. **Diverse Gait Execution**  
- Trained a single policy capable of executing four distinct gaits, providing the robot with the ability to walk, trot, canter, and gallop.  
- Enabled dynamic control over gait parameters such as foot swing trajectory, body posture, and movement speed, allowing the robot to adapt its motion to specific tasks and environmental requirements.  

### 2. **Curriculum Learning for Policy Robustness**  
- Utilized a teacher-student curriculum learning framework to progressively train the robot's control policy.  
- The teacher provided optimal guidance during the initial training phases, enabling the student model to gradually acquire robust and generalizable behaviors.  

### 3. **Multi-Version Locomotion Controller Design**  
- **Version 1 (Traditional Control):**  
  Developed a locomotion controller based on **Zero Moment Point (ZMP) stabilization**, ensuring static and dynamic balance during gait execution. This version served as a foundation for stable walking and maneuvering.  
- **Version 2 (Reinforcement Learning):**  
  Advanced the framework by designing a reinforcement learning-based control policy that allowed the robot to adapt to complex and dynamic environments. The policy provided greater flexibility and enhanced task performance compared to traditional approaches.  

### 4. **Simulation Environment Development**  
- Built a robust simulation environment using ROS and Gazebo to test and refine the control framework.  
- Derived precise kinematic and dynamic models for the robot, ensuring accurate simulation of real-world behaviors.  
- Successfully transferred the trained RL policy from simulation to the ROS-based control system for real-world deployment.  

### 5. **Hardware Integration and Testing**  
- Implemented the complete control framework on a quadrupedal robot platform.  
- Conducted extensive hardware testing, verifying the robot's ability to execute various gaits, maintain stability, and adapt to physical disturbances in real-world conditions.  

## Key Achievements  
- Demonstrated seamless integration of traditional control methods and reinforcement learning for adaptive locomotion.  
- Achieved robust and diverse gait execution, showcasing the potential for quadrupedal robots in challenging applications, such as exploration and navigation in unstructured environments.  
- Built a modular and scalable framework, paving the way for further advancements in quadrupedal robot control and deployment.  

<div class="row">
<div class="text-center mt-3 mt-md-0">
<iframe width="930" height="550" src="https://www.youtube.com/embed/RTfxgl5l3NM?si=I3ojspaZbAXg7j6E" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

</div>
<div class="caption">
    Project Video
</div>
---