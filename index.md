---
layout: single
title: "Parveez Banu Syed Azizuddin"
author_profile: false
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

This project simulates a two-wheeled differential drive robot equipped with a LiDAR sensor that autonomously avoids obstacles within a Gazebo environment. Using ROS 2 Humble and Gazebo Classic, the robot processes real-time laser scan data from the `/scan` topic and publishes velocity commands to `/cmd_vel` for smooth navigation. The setup includes a custom URDF/Xacro model and a detailed Gazebo world representing a cluttered environment.

- Developed custom robot model and integrated LiDAR sensor.  
- Implemented obstacle detection and avoidance algorithms in Python.  
- Designed simulation environment replicating real-world navigation challenges.

**Challenges faced:**  
- Ensuring accurate sensor data processing and filtering for reliable obstacle detection.  
- Tuning velocity commands to achieve smooth and safe robot movements.  
- Configuring Gazebo plugins and model files for correct sensor simulation.

**Learning outcomes:**  
- Mastered ROS 2 topics and message handling for real-time sensor and control data.  
- Gained experience in Gazebo robot modeling and simulation environment setup.  
- Enhanced understanding of autonomous navigation using LiDAR-based perception.

**Skills & tools used:**  
- ROS 2 Humble, Python  
- Gazebo Classic Simulation  
- URDF / Xacro Robot Description  
- LiDAR sensor integration  
- Ubuntu Linux, Visual Studio Code

[GitHub Repository](https://github.com/parveezsyed28/obstacle_avoidance_lidar)

---

### Robot Description and Simulation (Fusion 360 + ROS 2 + Gazebo)

This project features a custom-designed two-wheeled robot created using Fusion 360 and described with URDF/Xacro files. The model includes detailed STL meshes and integrates Gazebo plugins such as the differential drive controller for realistic motion simulation. The robot is simulated within Gazebo to test movement and sensor plugins, providing a solid foundation for further ROS 2 robotic development.

- Designed mechanical components in Fusion 360 and exported STL meshes.  
- Created accurate URDF and Xacro descriptions with sensors and plugins.  
- Simulated robot kinematics and sensor data in Gazebo.

**Challenges faced:**  
- Managing mesh file references and ensuring proper visualization in Gazebo.  
- Configuring differential drive plugin parameters for smooth robot control.  
- Synchronizing URDF with Gazebo-specific XML extensions.

**Learning outcomes:**  
- Gained experience in robot modeling and simulation workflows.  
- Understood integration of hardware CAD designs with ROS 2 simulation environments.  
- Developed skills in robot plugin configuration for Gazebo.

**Skills & tools used:**  
- Fusion 360 CAD  
- ROS 2 Humble, Gazebo Classic  
- URDF / Xacro Robot Modeling  
- STL Meshes and Gazebo Plugins  
- Python, Linux

[GitHub Repository](https://github.com/parveezsyed28/ros2_bot_description)

---

### Geometric Shape Drawer using Turtlesim (ROS 2)

A ROS 2 Python node that controls the turtlesim to draw geometric shapes based on interactive user input. It includes service calls to reset the turtlesim, allowing repeated shape drawing. This project demonstrates ROS 2 communication concepts like publishers, subscribers, and service clients in a simple and visual way.

- Implemented publisher and subscriber nodes for turtle velocity commands.  
- Handled CLI input and reset services in ROS 2.  
- Designed code modularity for ease of extending shapes.

**Challenges faced:**  
- Synchronizing service calls and publisher commands for smooth turtle control.  
- Managing timing and velocity parameters for precise shape drawing.

**Learning outcomes:**  
- Deepened understanding of ROS 2 communication patterns.  
- Improved ability to build interactive robotic applications.  
- Practiced Python scripting in ROS 2 nodes.

**Skills & tools used:**  
- ROS 2 Humble, Python  
- Turtlesim Simulator  
- Publisher/Subscriber and Service Calls

<!-- Example video placeholder -->
<video width="600" controls>
  <source src="/assets/images/geometric_shape_drawer.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

---

### ADC-Based Speed-Controlled Robot

An advanced robot integrating multiple sensors for obstacle avoidance, cliff detection, and black line following, with dynamic speed control via ADC input. Developed using Embedded C on an ATmega16 microcontroller.

- Utilizes multiple IR sensors for environmental awareness.  
- Implements speed control using potentiometer input through ADC.  
- Embedded C programming for real-time sensor and motor control.

**Challenges faced:**  
- Balancing sensor input and motor speed for smooth navigation.  
- Implementing precise ADC sampling and PWM motor control.  
- Hardware-software integration of multiple sensors.

**Learning outcomes:**  
- Mastered ADC usage in microcontrollers.  
- Developed complex embedded systems integrating sensors and control logic.  
- Improved hardware-software co-design skills.

[Image or schematic placeholder](/assets/images/adc_robot_diagram.png)

---

### Obstacle Avoider Robot

A microcontroller-based robot that avoids obstacles using IR sensors and L293D motor driver, programmed in Embedded C for the ATmega16.

- Implemented IR sensor interfacing and obstacle detection logic.  
- Controlled motors via embedded C code.  
- Designed chassis optimized for sensor placement.

**Challenges faced:**  
- Ensuring sensor reliability under varying conditions.  
- Timing motor control signals to avoid jerky motion.  
- Managing power distribution effectively.

**Learning outcomes:**  
- Gained expertise in embedded C programming for real-time control.  
- Practiced sensor integration on microcontrollers.  
- Understood motor driver interfacing and control.

![Obstacle Avoider Robot](/assets/images/obstacle_avoider_robot.png)

---

### Table Top Robot

Designed to detect table edges and avoid falling using IR sensors programmed on ATmega16 microcontroller.

- Used real-time IR sensor data for edge detection.  
- Embedded control logic to adjust motion based on sensor feedback.

**Challenges faced:**  
- Achieving fast, reliable edge detection.  
- Balancing sensor sensitivity to reduce false positives.

**Learning outcomes:**  
- Mastered IR sensor edge detection.  
- Refined embedded safety control strategies.

![Table Top Robot](/assets/images/table_top_robot.png)

---

### Line Follower Robot

A robot following a black line using bottom-mounted IR sensors. Developed in Embedded C on the ATmega16, using analog sensor input for line detection.

- Implemented analog IR sensor interfacing.  
- Developed control logic for path following.  
- Designed compact hardware.

**Challenges faced:**  
- Filtering sensor noise for accurate line detection.  
- Optimizing sensor placement and motor control.

**Learning outcomes:**  
- Applied embedded control techniques in constrained environments.  
- Gained understanding of sensor-based navigation.

![Line Follower Robot](/assets/images/line_follower_robot.png)

---

## Skills & Tools

- ROS 2 Humble, Gazebo Classic Simulation  
- URDF / Xacro Robot Description  
- Python, Embedded C Programming  
- ATmega16 Microcontroller, L293D Motor Driver, IR Sensors  
- Fusion 360 CAD Modeling, KiCad PCB Design  
- Linux (Ubuntu), Git & GitHub  

---

## Contact

- Email: [parveezbanu.s@gmail.com](mailto:parveezbanu.s@gmail.com)  
- GitHub: [github.com/parveezsyed28](https://github.com/parveezsyed28)  
- LinkedIn: [linkedin.com/in/parveez-banu-syed-azizuddin2807](https://www.linkedin.com/in/parveez-banu-syed-azizuddin2807)  
