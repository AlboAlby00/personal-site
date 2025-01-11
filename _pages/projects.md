---
permalink: /projects/
title: "Projects"
---

### Visual SLAM

<div style="display: flex; justify-content: center; align-items: center; margin: 20px 0;">
  <img 
    src="{{ '/assets/gif/visual_slam.gif' | relative_url }}" 
    alt="Visual SLAM GIF" 
    style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); width: 1000px; height: auto;"
  />
</div>

I implemented stereo SLAM (Simultaneous Localization and Mapping) C++ software capable of:
- Tracking the camera trajectory.
- Building a sparse map of the environment.

The software is inspired by the **[ORB-SLAM2 paper](https://arxiv.org/abs/1610.06475)**.

The computed trajectory is displayed in **red**, while the ground truth trajectory is shown in **yellow**.

The software operates on two separate threads:
1. **Trajectory computation:** Continuously tracks the camera's movement.
2. **Global optimization:** Minimizes the reprojection error to reduce cumulative errors.

**Download the full report:**
[Visual SLAM Report]({{ '/assets/pdf/slam_report.pdf' | relative_url }})

### Robotic Arm Teleoperation Using a Skin Sensor

<div style="display: flex; justify-content: center; align-items: center; margin: 20px 0;">
  <img 
    src="{{ '/assets/gif/hebi.gif' | relative_url }}" 
    alt="Animated GIF" 
    style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); max-height: 640px; height: auto; width: auto;"
  />
</div>

I developed ROS-based software to teleoperate two **HEBI robotic arms** using **[skin sensors](https://intouch-robotics.com/)** designed to detect human touch.

Key features:
- An **LSTM Neural Network** processes sensor data to classify various types of human touch.
- The classification results are combined with an **inverse kinematics algorithm** to compute precise low-level joint commands, enabling smooth and responsive arm movements.

### Connect 4 Robotic Player

<div style="display: flex; justify-content: center; align-items: center; gap: 20px; margin: 20px 0;">
  <img src="{{ '/assets/images/connect-4-1.jpg' | relative_url }}" alt="Connect 4 Image 1" style="height: 400px; width: auto; object-fit: cover; border-radius: 8px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);">
  <img src="{{ '/assets/images/connect-4-2.jpg' | relative_url }}" alt="Connect 4 Image 2" style="height: 400px; width: auto; object-fit: cover; border-radius: 8px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);">
</div>

I collaborated with a team to program a Franka Emika robotic arm to play Connect 4.

The robot uses an RGB-D camera to estimate the current state of the game board. This information is processed by a machine learning algorithm inspired by AlphaZero to plan the next move.

Our project competed in a robotics challenge, where we showcased the system's capabilities and achieved first place.

### Drone Controller using Reinforcement Learning
I collaborated with a team of four to develop a robust software stack for an autonomous drone using ROS2. My primary focus was on the control system that was implemented using Reinforcement Learning, specifically using Proximal Policy Optimization (PPO) algorithm. 
**Download the full report:**
[Drone Report]({{ '/assets/pdf/drone_report.pdf' | relative_url }})

---
