# P Pranav

**`Robotics Software Engineer`**

---

### About
- I write software that lets robots perceive, plan, and act, from motion planning on real hardware to imitation-learned manipulation
- Focused on manipulation, state estimation, and motion planning
- Best at building, controlling, and programming real hardware: ROS 2, motion/control algorithms, embedded and PLC integration
- Currently building the **SO-101 Manipulation Stack** (ROS 2 Jazzy, ros2_control, MoveIt 2) and reimplementing core robotics algorithms from scratch in Python and C++

---

### Tech Stack

**Robotics**

![ROS 2](https://img.shields.io/badge/ROS_2-22314E?style=flat-square&logo=ros&logoColor=white)
![ros2_control](https://img.shields.io/badge/ros2__control-22314E?style=flat-square&logo=ros&logoColor=white)
![MoveIt](https://img.shields.io/badge/MoveIt_2-0A7E07?style=flat-square&logoColor=white)
![Gazebo](https://img.shields.io/badge/Gazebo-FF6600?style=flat-square&logo=gazebo&logoColor=white)
![RViz](https://img.shields.io/badge/RViz-22314E?style=flat-square&logo=ros&logoColor=white)

**Languages & Libraries**

![C++](https://img.shields.io/badge/C++17-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Eigen](https://img.shields.io/badge/Eigen-3C6EB4?style=flat-square&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=flat-square&logo=cmake&logoColor=white)

**ML / Learning**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![LeRobot](https://img.shields.io/badge/LeRobot-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![YOLOv8](https://img.shields.io/badge/YOLOv8-00FFFF?style=flat-square&logoColor=black)

**Tools**

![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Jetson](https://img.shields.io/badge/Jetson-76B900?style=flat-square&logo=nvidia&logoColor=white)
![CODESYS](https://img.shields.io/badge/CODESYS-0046AD?style=flat-square&logoColor=white)

**Foundations:** Kinematics & Dynamics · State Estimation (EKF, UKF) · Path Planning (A\*, Dijkstra, Visibility Graphs) · Inverse Kinematics (Damped Least Squares)

---

### Projects

**[SO-101 Manipulation Stack](https://github.com/ppranav04/so101_manipulation_stack)** - *active*\
A ROS 2 Jazzy software stack for the SO-101 arm (5-DOF + gripper): see an object on a table, pick it up, and place it. Building a custom **C++ `ros2_control` hardware interface** for the Feetech STS3215 servo bus, a **closed-form 5-DOF IK solver as a MoveIt 2 plugin** (benchmarked against KDL), camera intrinsics and **hand-eye calibration**, and **RGB pick-and-place** evaluated over 50+ trials. The same controllers run on mock hardware, Gazebo Harmonic, and the real arm, with gtest/pytest, Docker, and GitHub Actions CI.\
`ROS 2 Jazzy · C++ · ros2_control · MoveIt 2 · Gazebo Harmonic · OpenCV · Docker · CI`

**[Robotics Algorithms from Scratch](https://github.com/ppranav04/robotics-algorithms)** - *active*\
A study of state estimation, SLAM, planning, and control, implementing each algorithm in both **Python** and **C++17** (Eigen, CMake).\
Done: **EKF localization**\
In progress: **UKF**\
Roadmap: Particle Filter, Graph-Based SLAM, A\*, Hybrid A\*, RRT/RRT\*, Pure Pursuit/Stanley, LQR, MPC, Damped-Least-Squares IK\
`Python · C++17 · Eigen · CMake · State Estimation · SLAM · Planning · Control`

**[BT-101: SO-101 Teleoperation & Imitation Learning](https://github.com/ppranav04/BT-101)** - *weekend project*\
Leader-follower and joystick teleoperation on the SO-101 arm, built from scratch down to the servo serial protocol and validated against the Hugging Face LeRobot ecosystem. Feeds an imitation-learning pipeline: recording pick-and-place demonstrations to train an **Action Chunking Transformer (ACT)** policy that maps RGB + joint states to action chunks. Next: Diffusion Policy.\
`Python · PyTorch · LeRobot · ACT · Imitation Learning`

**SCARA Path Planner - B.Tech Thesis (IGCAR)** - *completed*\
Visibility-graph + A\* path planner for a 2-DOF SCARA among circular obstacles: builds a full visibility graph (start/goal tangents, inter-obstacle cross-tangents, arc-boundary edges) and searches it with **A\*** under an admissible Euclidean heuristic. Benchmarked against **Dijkstra** across 1–10 obstacles: identical optimal paths, with A\*'s compute-time advantage growing to 48% at 10 obstacles. Implemented in CODESYS Structured Text on a PLC motion controller and validated on a 1:1 SCARA test rig.\
`CODESYS · PLC · A* · Visibility Graphs · Python`

**[Autonomous Agricultural Harvester](https://github.com/ppranav04/agrirover)** - *completed*\
ROS 2 mobile manipulator with a 6-DOF arm for tomato harvesting. Real-time **YOLOv8** ripeness detection on a **Jetson Orin Nano** with a RealSense D435 for low-latency edge decisions, with **MoveIt** driving the arm for pick-and-place.\
`ROS 2 · YOLOv8 · Jetson · RealSense · MoveIt · Python · C++`
