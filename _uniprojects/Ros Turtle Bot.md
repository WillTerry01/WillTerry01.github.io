---
name: BEng - ROS1, Turtle Bot
tools: [ROS1, Python, OpenCV]
image: ../Pictures/TurtleBot.jpg
description: Maze-navigating TurtleBot using ROS1 and computer vision with OpenCV.
---
# Turtle Bot and ROS1

The **TurtleBot** is a pre-built ROS1 robot designed for autonomous navigation and object detection.  

For this project, the robot had to **navigate a maze** and locate two doors — one marked with a green dot, the other with a red dot. Using **OpenCV (CV2)**, the robot identified the correct door based on color.

Once inside, it had to **search for a Cluedo character** displayed on the wall. To identify the character, the system leveraged **Harris Corner Detection**, allowing accurate recognition even in a small-scale, cluttered environment.

{% include elements/video.html id="aU5ADpcGbyY" %}

### 🔧 Approach & Implementation
- Developed ROS1 nodes in **Python** for navigation, sensor handling, and vision processing.  
- Implemented a **maze exploration algorithm**, combining sensor feedback with simple path planning.  
- Integrated **color detection** and corner-based feature recognition for object identification.  
- Debugged ROS1 topics, messages, and TF frames to ensure smooth communication between sensors and actuators.  

### 💡 Key Takeaways
- Gained hands-on experience with **ROS1 architecture**, including nodes, topics, and message passing.  
- Learned to integrate **computer vision with real-time robotics control**.  
- Improved debugging and problem-solving skills in a multi-component system.  
- Built confidence transitioning from ROS1 to ROS2 for more complex robotics projects later in my studies.

---
