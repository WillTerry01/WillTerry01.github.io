---
name: MSc - Drone Robotics
tools: [Python, Aerostack2, Gazebo]
image: ../UniPictures/CrazyFlyDrone.jpeg
description: Two courseworks exploring autonomous flight and swarm navigation using Aerostack2 and Crazyflie drones, simulated in Gazebo.
---
# Drones

This module introduced **Crazyflie drones**, **Aerostack2**, and **Gazebo** for autonomous flight control and simulation. The *Crazyflie* is a small, lightweight drone with open-source firmware and detailed dynamics models — ideal for academic research and simulation. **Aerostack2** is a modular ROS2-based framework simplifying drone autonomy development, while **Gazebo** provided the physics-based simulation environment.

---

### 🧭 Coursework 1: Path Planning & Obstacle Avoidance

**Task:**  
Design a system for a drone to visit all given waypoints efficiently while avoiding obstacles defined in a YAML configuration file.

**Approach:**  
I explored several path-planning algorithms — **Breadth-First Search**, **Depth-First Search**, **Dijkstra**, and **A\*** — and selected **Dijkstra’s Algorithm** for its balance of accuracy and computational efficiency. Obstacle avoidance was implemented using a **buffered collision zone**: the drone checked for potential collisions and inserted temporary waypoints to detour around obstacles.

**Video Demonstration:**  
<div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;">
  <iframe
    src="https://www.youtube.com/embed/hos7udg7sPk"
    title="Path Planning Demo"
    allowfullscreen
    style="position:absolute;top:0;left:0;width:100%;height:100%;border:0;">
  </iframe>
</div>

---

### 🐝 Coursework 2: Swarm Coordination & Dynamic Navigation

**Task:**  
Control a swarm of 1–5 drones through a series of navigation challenges, including formation flying, obstacle courses, and dynamic environments.

**Stages:**
1. **Formation flight:** Circle, line, star, and orbiting patterns.  
2. **Window navigation:** Passing through multiple windows of varying sizes.  
3. **Forest traversal:** Navigating around fixed obstacles (tree structures).  
4. **Dynamic obstacles:** Real-time updates of moving objects via YAML input.

**Approach:**  
Two control architectures were explored:
- **Centralized control (my focus):** One drone acted as the master node computing trajectories for the entire swarm.  
- **Decentralized control (teammate’s focus):** Drones interacted through **potential fields**, attracting toward goals and repelling from obstacles and each other.

Both methods had trade-offs — centralized offered efficient coordination, while decentralized excelled in adaptability.

**Video Demonstration:**  
<div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;">
  <iframe
    src="https://www.youtube.com/embed/VsKYebtmU_g"
    title="Swarm Navigation Demo"
    allowfullscreen
    style="position:absolute;top:0;left:0;width:100%;height:100%;border:0;">
  </iframe>
</div>

---

### 🔧 Key Takeaways
- Designed and implemented **path planning** and **obstacle avoidance** algorithms.  
- Gained hands-on experience with **Aerostack2**, **ROS2 nodes**, and **Gazebo simulation**.  
- Compared **centralized vs decentralized** swarm architectures.  
- Strengthened skills in **Python**, **modular autonomy frameworks**, and **simulation debugging**.

---
