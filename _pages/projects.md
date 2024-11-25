---
permalink: /projects/
title: "Projects"
---
### Robotic Arm Teleoperation Using a Skin Sensor

<video width="640" height="360" controls>
  <source src="{{ '/assets/videos/hebi.mp4' | relative_url }}" type="video/mp4">
  Your browser does not support the video tag.
</video>

I developed ROS-based software to teleoperate two **HEBI robotic arms** using **[skin sensors](https://intouch-robotics.com/)** designed to detect human touch.

Key features:
- An **LSTM Neural Network** processes sensor data to classify various types of human touch.
- The classification results are combined with an **inverse kinematics algorithm** to compute precise low-level joint commands, enabling smooth and responsive arm movements.

### Visual SLAM

<video width="640" height="360" controls>
  <source src="{{ '/assets/videos/visual_slam.mp4' | relative_url }}" type="video/mp4">
  Your browser does not support the video tag.
</video>

I implemented stereo SLAM (Simultaneous Localization and Mapping) C++ software capable of:
- Tracking the camera trajectory.
- Building a sparse map of the environment.

The software is inspired by the **[ORB-SLAM2 paper](https://arxiv.org/abs/1610.06475)**.

The computed trajectory is displayed in **red**, while the ground truth trajectory is shown in **yellow**.

The software operates on two separate threads:
1. **Trajectory computation:** Continuously tracks the camera's movement.
2. **Global optimization:** Minimizes the reprojection error to reduce cumulative errors.

---

### Drone Controller based on Reinforcement Learning

