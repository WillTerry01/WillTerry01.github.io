---
name: ROS1 - Trutle Bot
tools: [ROS1, Python, CV2]
image: ../Pictures/TurtleBot.jpg
description: A Maze navigating Robot using ROS1 with CV2 Library
---

# Turtle Bot

The TurtleBot is a system pre-built with ROS1, designed for tasks like autonomous navigation and object detection. For this project, the robot's task was to navigate a small maze and locate two doors—one labeled with a green dot and the other with a red dot. Using the CV2 library for computer vision, the robot identified the correct door to pass through based on its color.

Once inside the room, the robot had to search for a Cluedo character pictured on the wall. To identify the character, the system utilized Harris Corner Detection, allowing the robot to correctly determine the character's identity.

{% include elements/video.html id="aU5ADpcGbyY" %}

This project was particularly challenging as it was my first time working with ROS1. However, it provided a solid foundation, and since then, I’ve gained significant experience with ROS2 and have undertaken other ROS2-based projects.
