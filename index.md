---
layout: default
title: Parveez Banu Syed Azizuddin | Robotics Portfolio
description: >
  Mechatronics Specialist with expertise in ROS 2, Gazebo, Embedded Systems, and Fusion 360 CAD modeling. Explore projects on wall following, obstacle avoidance, embedded robots, and more.
---

# Parveez Banu Syed Azizuddin

*Mechatronics Specialist | Robotics Enthusiast | ROS 2 Developer*

---

## About Me

I am a Mechatronics Specialist with a Bachelor’s degree in Electrical and Electronics Engineering and a Postgraduate Certificate in Industrial Automation. Passionate about robotics, I excel in integrating both hardware and software systems. My hands-on experience includes ROS 2, Gazebo simulation, Python programming, Fusion 360 CAD modeling, and embedded microcontroller development. I aspire to contribute as a versatile roboticist building intelligent autonomous systems.

---

## Featured Projects

### Wall Follower Robot (ROS 2 + Gazebo)

This robot autonomously follows walls using LiDAR data and ROS 2 nodes. The simulation runs in a maze-like Gazebo environment where the robot adjusts its path to maintain a stable distance from the wall.

**Highlights:**
- Created ROS 2 nodes subscribing to LiDAR data and publishing velocity commands.
- Tuned control logic for stable wall following in real-time.
- Simulated robot behavior in a complex maze environment using Gazebo.

**Challenges faced:**
- Maintaining stable distance through tight corners with noisy sensor data.
- Filtering LiDAR data to avoid false detections.
- Balancing speed and safety for smooth navigation.

**Learning outcomes:**
- Mastered real-time ROS 2 topic communication.
- Gained experience with sensor data filtering.
- Improved autonomous navigation logic.

<div class="project-media" style="text-align:center; margin-top:20px;">
  <video controls style="max-width:100%; height:auto; border-radius:8px; box-shadow: 0 3px 10px rgba(0,0,0,0.7);">
    <source src="/assets/images/Wall_follower.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
</div>

---

### Obstacle Avoidance with LiDAR (ROS 2 + Gazebo)

This project simulates a two-wheeled differential drive robot equipped with a LiDAR sensor that autonomously avoids obstacles within a Gazebo environment. Using ROS 2 Humble and Gazebo Classic, the robot processes real-time laser scan data and publishes velocity commands for smooth navigation.

**Highlights:**
- Developed custom robot model and integrated LiDAR sensor.
- Implemented obstacle detection and avoidance algorithms in Python.
- Designed simulation environment replicating real-world navigation challenges.

**Challenges faced:**
- Ensuring accurate sensor data processing and filtering.
- Tuning velocity commands for smooth movement.
- Configuring Gazebo plugins correctly.

**Learning outcomes:**
- Mastered ROS 2 message handling.
- Gained experience in Gazebo simulation setup.
- Enhanced understanding of LiDAR-based autonomous navigation.

<div class="project-media" style="text-align:center; margin-top:20px;">
  <video controls style="max-width:100%; height:auto; border-radius:8px; box-shadow: 0 3px 10px rgba(0,0,0,0.7);">
    <source src="/assets/images/Obstacle_Avoidance.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <br />
  <a href="https://github.com/parveezsyed28/obstacle_avoidance_lidar" target="_blank" rel="noopener" style="color:#4fc3f7; font-weight:600; text-decoration:none;">GitHub Repository</a>
</div>

---

### Robot Description and Simulation

This project features a custom-designed two-wheeled robot created in Fusion 360 and described with URDF/Xacro files. The model includes detailed STL meshes and integrates Gazebo plugins such as differential drive controllers.

**Highlights:**
- Designed mechanical components in Fusion 360.
- Created accurate URDF/Xacro descriptions with sensors and plugins.
- Simulated robot kinematics and sensor data in Gazebo.

**Challenges faced:**
- Managing mesh file references for visualization.
- Configuring differential drive plugin parameters.
- Synchronizing URDF with Gazebo extensions.

**Learning outcomes:**
- Robot modeling and simulation workflows.
- Integration of CAD designs with ROS 2.
- Gazebo plugin configuration skills.

<div class="project-media" style="text-align:center; margin-top:20px;">
  <img src="/assets/images/ros2_bot_description.png" alt="ROS 2 Bot Description" style="max-width:100%; border-radius:8px; box-shadow: 0 3px 10px rgba(0,0,0,0.7);" />
  <video controls style="max-width:100%; height:auto; margin-top: 10px; border-radius:8px; box-shadow: 0 3px 10px rgba(0,0,0,0.7);">
    <source src="/assets/images/robot_teleop.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <br />
  <a href="https://github.com/parveezsyed28/ros2_bot_description" target="_blank" rel="noopener" style="color:#4fc3f7; font-weight:600; text-decoration:none;">GitHub Repository</a>
</div>

---

### Geometric Shape Drawer (Turtlesim)

A ROS 2 Python node controlling turtlesim to draw geometric shapes based on user input, demonstrating ROS 2 publishers, subscribers, and service clients.

**Highlights:**
- Implemented publisher and subscriber nodes.
- Handled CLI input and reset services.
- Modular design for extending shapes.

**Challenges faced:**
- Synchronizing service calls and commands.
- Managing timing for precise drawing.

**Learning outcomes:**
- ROS 2 communication patterns.
- Interactive robotic applications.
- Python scripting in ROS 2.

<div class="project-media" style="text-align:center; margin-top:20px;">
  <video controls style="max-width:100%; height:auto; border-radius:8px; box-shadow: 0 3px 10px rgba(0,0,0,0.7);">
    <source src="/assets/images/Turtlesim.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
</div>

---

### ADC-Based Speed Controlled Robot

An advanced robot integrating multiple IR sensors and dynamic speed control using the ADC module on the ATmega16 microcontroller.

**Highlights:**
- Uses front, top, left, right IR sensors.
- Speed controlled via ADC reading from potentiometer.
- Real-time sensor processing and motor control.

**Challenges faced:**
- Balancing sensor readings with motor control.
- Accurate ADC sampling and PWM motor speed control.
- Hardware integration of multiple sensors.

**Learning outcomes:**
- Mastered ADC in microcontrollers.
- Developed complex embedded systems.
- Hardware-software co-design.

<div class="project-media" style="text-align:center; margin-top:20px;">
  <img src="/assets/images/adc_robot_diagram.png" alt="ADC Robot Diagram" style="max-width:80%; border-radius:8px; box-shadow: 0 3px 10px rgba(0,0,0,0.7);" />
</div>

---

### Obstacle Avoider Robot

Microcontroller-based robot avoids obstacles using IR sensors programmed with Embedded C on ATmega16. Controls motion via L293D motor driver.

**Highlights:**
- IR sensor interfacing and obstacle detection.
- Motor control with embedded C.
- Hardware optimized for sensor placement.

**Challenges faced:**
- Reliable sensor readings under varying light.
- Smooth motor control to avoid jerks.
- Power distribution management.

**Learning outcomes:**
- Embedded C for real-time control.
- Sensor integration on microcontrollers.
- Motor driver interfacing.

<div class="project-media images-container" style="margin-top:20px;">
  <img src="/assets/images/obstacle_avoider.png" alt="Obstacle Avoider Robot" />
  <img src="/assets/images/Obstacle_avoider_connection.png" alt="Obstacle Avoider Circuit" />
</div>

---

### Table Top Robot

Designed to detect table edges and avoid falling using IR sensors on ATmega16 microcontroller.

**Highlights:**
- Real-time IR sensor data for edge detection.
- Embedded control logic for stability.

**Challenges faced:**
- Fast and reliable edge detection.
- Balancing sensitivity and false positives.

**Learning outcomes:**
- Edge detection with IR sensors.
- Embedded control strategies.

<div class="project-media" style="text-align:center; margin-top:20px;">
  <img src="/assets/images/table_top.png" alt="Table Top Robot" style="max-width:100%; border-radius:8px; box-shadow: 0 3px 10px rgba(0,0,0,0.7);" />
</div>

---

### Line Follower Robot

A robot following a black line using bottom-mounted IR sensors and embedded C on ATmega16.

**Highlights:**
- Analog IR sensor interfacing.
- Real-time control logic for path following.
- Compact hardware design.

**Challenges faced:**
- Accurate sensor readings without noise filtering.
- Fine sensor placement for reliability.
- Smooth motor control on curves.

**Learning outcomes:**
- Sensor-based path following.
- Embedded control techniques.

<div class="project-media images-container" style="margin-top:20px;">
  <img src="/assets/images/line_follower.png" alt="Line Follower Robot" />
  <img src="/assets/images/line_follower_connection.png" alt="Line Follower Circuit" />
</div>

---

## Skills

- ROS 2 Humble and Python programming  
- Embedded C on ATmega16 microcontroller  
- Fusion 360 CAD modeling  
- Gazebo Classic simulation and URDF/Xacro robot modeling  
- Linux and Visual Studio Code

---

## Contact

Feel free to reach out:

- Email: <a href="mailto:your.email@example.com">your.email@example.com</a>  
- GitHub: <a href="https://github.com/parveezsyed28" target="_blank" rel="noopener">github.com/parveezsyed28</a>

---

<footer style="text-align:center; padding:20px; color:#607d8b; border-top:1px solid #37474f; margin-top:60px;">
  © 2025 Parveez Banu Syed Azizuddin. All rights reserved.
</footer>
