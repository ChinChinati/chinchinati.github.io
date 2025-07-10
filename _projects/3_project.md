---
layout: page
title: Autonomous Self-Balancing Robot
description: PID and LQR Controller
img: assets/img/sabar.jpg
importance: 5
category: <
related_publications: false
---

### <a href="https://github.com/ChinChinati/Self_balancing_bot">[code]</a>

# Two-Wheeled Self Balancing Robot

**Mentored by**: Prof. Arun Dayal Udai

This project focuses on the design, development, and control of a **Two-Wheeled Self Balancing Robot**. The robot was created from scratch, both in hardware and software, with a custom-built **cascaded PID controller** to ensure stability and accurate balancing. The robot was also simulated in both **Gazebo** and **Simulink** to validate and refine the controller performance under various conditions.

## Key Contributions

### 1. **Controller Development**

- Developed a **custom cascaded PID-based controller** that integrates **acceleration** values to improve the robot's stability and response time.
- The cascaded PID controller ensures better performance in balancing the robot by separating the control of tilt angle and angular velocity, allowing for smoother corrections.

### 2. **Simulation**

- **Gazebo Simulation**: Simulated the robot using the cascaded PID controller to test and visualize its behavior in a 3D environment. This simulation helped identify potential issues in the control loop before hardware implementation.
- **Simulink Simulation**: Implemented an **LQR (Linear Quadratic Regulator)** controller in Simulink to explore a different approach to balancing and compare its performance against the cascaded PID controller.

### 3. **Hardware Design**

- Designed and built the **two-wheeled robot hardware** from scratch, including the motor driver circuitry, sensor integration, and mechanical components. The robot's core functionality is based on precise control of the motors in response to sensor data (such as tilt and angular velocity).
- Integrated **gyroscope** and **accelerometer** sensors to monitor the robot’s tilt and acceleration, feeding the data into the controller to maintain balance.

## Challenges Overcome

- Fine-tuned the controller to deal with non-linearities in the robot’s dynamics.
- Addressed sensor noise and drift, ensuring that the robot could maintain stable balance in real-world conditions.
- Optimized the simulation-to-hardware transfer, ensuring that results from Gazebo and Simulink matched the real-world performance of the robot.

## Conclusion

This project demonstrates the integration of both hardware and advanced control techniques to build a **two-wheeled self-balancing robot**. The development of custom controllers and simulation in both **Gazebo** and **Simulink** has provided invaluable insights into robotic control systems and stability management. The project provides a solid foundation for further exploration of dynamic balancing and robotic control systems.

<div class="row">
<div class="text-center mt-3 mt-md-0">
<iframe width="930" height="550" src="https://www.youtube.com/embed/h7SCwEhvALs?si=izTCJtqIv10d9OkU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

</div>
<div class="caption">
    Project Video
</div>
---
