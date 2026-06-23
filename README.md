<p align="center">
  <img src="https://github.com/user-attachments/assets/d4b526d6-0c41-4894-aeb3-39c7176adf91" width="480" alt="banner gif">
</p>

# 🛠️ P Pranav 

**`Robotics Software Engineer`**

---

### About
- I build software for robots to think: assistive prosthetics, food-production automation, and precision systems for scientific infrastructure
- Focused on perception, motion planning, and learning-based manipulation
- Best at building, controlling, and programming real hardware: ROS 2, motion/control algorithms, CODESYS/PLC integration
- Currently building **Project Tvastr**: teleoperation + ACT policies on an SO-101 arm

---


### Tech Stack

**Robotics**

![ROS 2](https://img.shields.io/badge/ROS_2-22314E?style=flat-square&logo=ros&logoColor=white)
![MoveIt](https://img.shields.io/badge/MoveIt-0A7E07?style=flat-square&logoColor=white)
![Gazebo](https://img.shields.io/badge/Gazebo-FF6600?style=flat-square&logo=gazebo&logoColor=white)
![RViz](https://img.shields.io/badge/RViz-22314E?style=flat-square&logo=ros&logoColor=white)

**Languages**

![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)

**ML / Learning**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![LeRobot](https://img.shields.io/badge/LeRobot-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![YOLOv8](https://img.shields.io/badge/YOLOv8-00FFFF?style=flat-square&logoColor=black)

**Control &amp; Planning**

![CODESYS](https://img.shields.io/badge/CODESYS-0046AD?style=flat-square&logoColor=white)
![PLC](https://img.shields.io/badge/PLC-0046AD?style=flat-square&logoColor=white)

**Tools**

![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitLab](https://img.shields.io/badge/GitLab-FC6D26?style=flat-square&logo=gitlab&logoColor=white)
![Jetson](https://img.shields.io/badge/Jetson-76B900?style=flat-square&logo=nvidia&logoColor=white)
![SolidWorks](https://img.shields.io/badge/SolidWorks-E2231A?style=flat-square&logo=dassaultsystemes&logoColor=white)

**Foundations:** Kinematics &amp; Dynamics · Path Planning (A\*, Dijkstra, Visibility Graphs) · Trajectory Optimization · Sim-to-Real

---

### Projects

**[SO-101 Teleoperation &amp; Imitation Learning (Project Tvastr)](https://github.com/<USERNAME>/tvastr)** - *active*
Complete leader-follower teleoperation and imitation-learning pipeline on a 6-DOF SO-101 arm in the Hugging Face LeRobot ecosystem. Recorded pick-and-place demonstrations, trained an **Action Chunking Transformer (ACT)** policy mapping RGB + joint states to action chunks, and deployed it for closed-loop autonomous execution.\
`Python · PyTorch · LeRobot · ACT · Imitation Learning`

**SCARA Path Planner - B.Tech Thesis (IGCAR)**\
Visibility-graph + A\* path planner for a 2-DOF SCARA among circular obstacles: builds a full visibility graph (start/goal tangents, inter-obstacle cross-tangents, arc-boundary edges) and searches it with **A\*** under an admissible Euclidean heuristic, benchmarked against **Dijkstra** (identical optimal paths, fewer node expansions). Implemented in CODESYS Structured Text on a PLC motion controller and validated on a 1:1 SCARA test rig.\
`CODESYS · PLC · A* · Visibility Graphs · Python`

**[Autonomous Agricultural Harvester](https://github.com/ppranav04/agrirover)**
Autonomous mobile manipulator with a 6-DOF arm for precision crop harvesting. Real-time **YOLOv8** crop detection running on **Jetson Nano** for low-latency edge decisions, with **MoveIt** driving the arm for pick-and-place.\
`ROS 2 · YOLOv8 · Jetson · MoveIt · Python · C++`

**[EMG-Controlled Biomimetic Hand](https://github.com/ppranav04/biomimetic_hand)**
Tendon-driven InMoov humanoid hand that grasps and releases from live EMG muscle signals. Acquired and filtered raw EMG via Arduino, mapped activation thresholds to servo commands, and 3D-printed the hand with fishing-line tendon actuation - biosignal processing applied to assistive/prosthetic robotics.\
`Arduino · EMG · Servos · 3D Printing · SolidWorks · C++`




