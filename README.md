✅ README.md for robot197 (ROS2 URDF Humanoid Robot Project)

# 🤖 robot197 — ROS2 URDF Humanoid Robot Project

This repository contains the **robot197 humanoid robot** built completely from scratch using **Fusion 360**, **URDF**, and **Xacro**.  
All meshes are custom-made (.stl) and assembled together using proper revolute & fixed joints.

This is the **first full robotics project** developed by Ranzan Tamang as part of learning ROS2, URDF/Xacro, and robot modeling.

---

## 📌 Features

### ✔ Custom-designed robot
- Torso  
- Head  
- Arms  
- Fingers  
- Hips  
- Legs  

All meshes are uniquely created by the author.

### ✔ Full URDF/Xacro Robot Description
Includes:
- Multiple links  
- Revolute joints (with limits & dynamics)  
- Fixed joints  
- Materials & colors  
- Origin & RPY configuration  
- 100% mesh-based robot

### ✔ Works with ROS2
Tested on:
- **ROS2 Humble**
- Ubuntu **22.04**
- Rviz2

Launch and visualize with:
```bash
ros2 launch urdf_tutorial display.launch.py model:=/path/to/robot197.xacro

📁 Project Structure

my_robot_description/
│── meshes/
│    ├── torso197.stl
│    ├── head197.stl
│    ├── right_arm197.stl
│    ├── left_arm197.stl
│    ├── right_fingure197.stl
│    ├── left_fingure197.stl
│    ├── hips197.stl
│    ├── left_leg197.stl
│    ├── right_leg197.stl
│
│── urdf/
│    ├── robot197.xacro
│
└── CMakeLists.txt

🦾 Robot Description

The robot contains:

Part	Joint Type	Parent → Child
Head	Revolute	base_link → head_link
Right Arm	Revolute	base_link → right_arm
Left Arm	Revolute	base_link → left_arm
Right Finger	Revolute	right_arm → right_fingure
Left Finger	Revolute	left_arm → left_fingure
Hips	Fixed	base_link → hips197
Left Leg	Revolute	hips197 → left_leg
Right Leg	Revolute	hips197 → right_leg

All joints have:

Position limits

Axis definition

Dynamics (damping + friction)

🖥 How to Visualize in Rviz2

Build your ROS2 workspace:
colcon build --symlink-install
source install/setup.bash
ros2 launch urdf_tutorial display.launch.py model:=/path/to/robot197.xacro

🔧 Tools Used

Fusion 360 → 3D modeling & STL export

ROS2 Humble → Robot framework

URDF / Xacro → Robot structure

Rviz2 → Visualization

Git & GitHub → Version control

🎯 Purpose of This Project

This project is part of my personal journey to become a Robotics Engineer, focusing on:

Mastering URDF & Xacro

Learning robot kinematics

Practicing ROS2

Building a portfolio for future Master's (RA) applications

Understanding real robot assembly structure

🚀 Future Improvements

Add joints for head yaw/pitch

Add elbow joints

Add knee joints

Add textures/materials

Add controllers for movement

Gazebo simulation support

👨‍💻 Author

Ranzan Tamang (ranzant197)
Aspiring Robotics Engineer
Currently working on ROS2, URDF, Gazebo & Fusion 360 projects.