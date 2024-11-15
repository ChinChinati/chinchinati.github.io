---
layout: page
title: Wheeled-Humanoid Robot 
description: RL Controller
img: assets/img/centaur.jpg
importance: 2
category: <
related_publications: false
---

# Collaborative Control of Upper and Lower Body for Wheeled Humanoid Robots Using Multi-Agent Reinforcement Learning  

This project focuses on developing a robust collaborative control framework for wheeled humanoid robots using advanced Multi-Agent Reinforcement Learning (MARL) techniques. The objective was to enable effective coordination between the robot's upper and lower body to achieve complex tasks such as balancing, maneuvering, and manipulation in dynamic environments.  

## Key Highlights  
- **Environment Simulation:**  
  Developed and trained policies in the NVIDIA Isaac Gym environment, leveraging its high-fidelity physics simulation for rapid policy evaluation.  

- **Collaborative Policy Training:**  
  Designed specialized policies for the upper and lower body, employing algorithms like:  
  - MAPPO (Multi-Agent Proximal Policy Optimization)  
  - IPPO (Independent Proximal Policy Optimization)  
  - Dual-A2C (Actor-Critic)  

- **Task Coordination:**  
  - Lower body: Trained to maintain balance and execute precise maneuvers.  
  - Upper body: Optimized for manipulation tasks.  
  - Achieved seamless coordination for simultaneous locomotion and object interaction.  

- **Robust Performance:**  
  The trained policies demonstrated resilience to disturbances, allowing the robot to perform challenging tasks such as jumping and handling objects in unstructured scenarios.  

This work showcases the potential of MARL in enhancing the adaptability and efficiency of humanoid robots, paving the way for their deployment in real-world applications requiring advanced mobility and dexterity.  

<div class="row">
<div class="text-center mt-3 mt-md-0">
    <iframe 
        width="930" 
        height="550" 
        src="https://www.youtube.com/embed/h2RINaXp3i8?si=DZ8Dz7dfWSrPicfi" 
        title="YouTube video player" 
        frameborder="0" 
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
        referrerpolicy="strict-origin-when-cross-origin" 
        allowfullscreen>
    </iframe>
</div>

</div>
<div class="caption">
    Project Video
</div>
---