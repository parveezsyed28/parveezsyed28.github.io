---
layout: home
title: "Parveez Banu Syed Azizuddin"
subtitle: "Robotics Enthusiast | ROS 2 Developer"
author_profile: true
permalink: /
classes: wide
---

## About Me

Welcome to my portfolio — a vibrant collection fueled by passion, creativity, and a relentless drive for robotics! Dive into projects that showcase how I bring sensors, control systems, and software together to build robots that sense, decide, and act with purpose. Each piece here reflects my excitement for hands-on learning and my unstoppable curiosity in the world of robotics, where every challenge sparks innovation and growth.

---

## Featured Projects

### Wall Following Robot (ROS 2 + Gazebo)

This robot autonomously follows the wall using LiDAR data and ROS 2 nodes. The simulation is set in a maze-like Gazebo world, and the robot uses real-time perception to adjust its path and maintain proximity to the wall.

- Created a ROS 2 node to subscribe to LiDAR scan data and control robot movement.
- Tuned control logic to maintain a constant distance from the wall.
- Simulated robot behavior in a maze environment using Gazebo.

**Challenges faced:**  
- Maintaining stable distance in tight corners and noisy sensor data.  
- Filtering LiDAR data to avoid false positives.  
- Balancing velocity for smooth, safe navigation.

**Learning outcomes:**  
- Developed skills in sensor processing and feedback control.  
- Advanced ROS 2 node programming for navigation tasks.  
- Improved Gazebo environment setup and simulation design.

**Project Video:**  
<video width="600" controls>
  <source src="/assets/images/Wall_follower.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

[GitHub Repository](https://github.com/parveezsyed28/wall_follower_bot)

---

### Obstacle Avoidance with LiDAR (ROS 2 + Gazebo)

Simulates a differential drive robot equipped with a LiDAR sensor that autonomously avoids obstacles in a cluttered Gazebo world.

- Developed custom robot model and integrated LiDAR sensor.  
- Implemented obstacle detection and avoidance algorithms in Python.  
- Designed simulation environment replicating real-world challenges.

**Challenges faced:**  
- Accurate filtering of LiDAR data for reliable detection.  
- Smooth and safe robot velocity tuning.  
- Correct setup of Gazebo plugins and sensor simulation.

**Learning outcomes:**  
- Mastered ROS 2 topic/message handling.  
- Gained experience with URDF/Xacro and simulation setup.  
- Improved navigation logic using real-time perception.

[GitHub Repository](https://github.com/parveezsyed28/obstacle_avoidance_lidar)

---

### Robot Description and Simulation (Fusion 360 + ROS 2 + Gazebo)

A custom-designed two-wheeled robot modeled in Fusion 360 and described with URDF/Xacro, simulated in Gazebo.

- Designed mechanical components in Fusion 360 and exported STL meshes.  
- Created accurate URDF and Xacro files.  
- Simulated movement and sensors using Gazebo plugins.

**Challenges faced:**  
- Ensuring correct mesh rendering in Gazebo.  
- Tuning differential drive plugin.  
- Integrating sensor and motion plugins with URDF.

**Learning outcomes:**  
- Integration of CAD models with ROS 2 simulation.  
- Practice with URDF/Xacro and Gazebo configuration.  
- Improved understanding of simulation workflows.

[GitHub Repository](https://github.com/parveezsyed28/ros2_bot_description)

---

### Geometric Shape Drawer using Turtlesim (ROS 2)

Draws user-defined geometric shapes in turtlesim using ROS 2 Python nodes and services.

- Implemented publisher/subscriber logic.  
- Reset turtlesim via service calls.  
- Allowed user input for interactive experience.

**Challenges faced:**  
- Synchronizing service and command timing.  
- Handling velocity for precise shape creation.

**Learning outcomes:**  
- ROS 2 communication concepts (topics, services).  
- Modular code structuring for robotics.  
- Python scripting in ROS 2.

<video width="600" controls>
  <source src="/assets/images/geometric_shape_drawer.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

---

### ADC-Based Speed-Controlled Robot (Embedded C + ATmega16)

An embedded robot using IR sensors and ADC-based potentiometer input for dynamic speed control.

- Multi-sensor obstacle, cliff, and line detection.  
- ADC input from potentiometer for speed regulation.  
- Programmed in Embedded C on ATmega16.

**Challenges faced:**  
- Precise ADC sampling and PWM control.  
- Balancing motor speed with sensor feedback.  
- Integrating analog and digital signals effectively.

**Learning outcomes:**  
- Mastered ADC and real-time sensor control.  
- Developed advanced embedded motor control logic.  
- Strengthened hardware-software integration skills.

---

### Obstacle Avoider Robot (Embedded C + ATmega16)

An IR-sensor-based robot that avoids obstacles using motor control logic and L293D driver.

- Programmed using Embedded C on ATmega16.  
- IR sensor integration for detection.  
- Compact chassis for mobility.

**Challenges faced:**  
- IR accuracy under environmental noise.  
- Motor timing and power balancing.

**Learning outcomes:**  
- Embedded C in robotics.  
- Sensor-based autonomous control.  
- Real-time microcontroller programming.

![Obstacle Avoider Robot](/assets/images/obstacle_avoider_robot.png)

---

### Table Top Robot

A safety robot that detects table edges to prevent falls using IR sensors and embedded logic.

- Programmed on ATmega16.  
- Edge detection and feedback motion control.

**Challenges faced:**  
- Accurate edge detection without false triggers.  
- Fast reaction to avoid fall-off.

**Learning outcomes:**  
- Embedded IR sensor control.  
- Safety logic in embedded systems.

![Table Top Robot](/assets/images/table_top_robot.png)

---

### Line Follower Robot

Follows a black line using analog IR sensors and motor control on ATmega16.

- IR sensor placement for accuracy.  
- Embedded path following algorithm.  
- Analog signal processing and filtering.

**Challenges faced:**  
- Noise filtering in analog signals.  
- Responsive motor control for sharp curves.

**Learning outcomes:**  
- Sensor-based embedded navigation.  
- Microcontroller-level motor and sensor control.

![Line Follower Robot](/assets/images/line_follower_robot.png)

---

## Skills & Tools

- ROS 2 Humble, Gazebo Classic Simulation  
- URDF / Xacro Robot Description  
- Python, Embedded C Programming  
- ATmega16, L293D, IR Sensors  
- Fusion 360 CAD, KiCad PCB Design  
- Linux (Ubuntu), Git & GitHub  

---

## Contact

- 📧 [parveezbanu.s@gmail.com](mailto:parveezbanu.s@gmail.com)  
- 🧠 [GitHub](https://github.com/parveezsyed28)  
- 💼 [LinkedIn](https://www.linkedin.com/in/parveez-banu2807)
- 
