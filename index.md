---
layout: single
title: "Parveez Banu Syed Azizuddin"
author_profile: true
permalink: /
classes: wide
---

<style>
  .header-container {
    text-align: center;
    margin-top: 40px;
    margin-bottom: 60px;
  }
  .header-container h1 {
    font-size: 3rem;
    color: #4a90e2; /* pastel blue */
    margin: 0;
    font-weight: 900;
    letter-spacing: 1.2px;
  }
  .header-container p {
    margin: 8px 0 0;
    font-size: 1.25rem;
    color: #6fa8dc; /* lighter pastel blue */
    font-weight: 600;
  }
  .project-media {
    margin-top: 20px;
    max-width: 720px;
    margin-left: auto;
    margin-right: auto;
    text-align: center;
  }
  .project-media img,
  .project-media video {
    max-width: 100%;
    height: auto;
    border-radius: 6px;
    box-shadow: 0 3px 10px rgba(0,0,0,0.7);
    margin-bottom: 15px;
  }
  .side-by-side {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
  }
  .side-by-side img {
    max-width: 48%;
    height: auto;
    border-radius: 6px;
    box-shadow: 0 3px 10px rgba(0,0,0,0.7);
  }
  a.github-link {
    font-weight: 600;
    color: #4a90e2;
    text-decoration: none;
    display: inline-block;
    margin-top: 8px;
  }
  a.github-link:hover {
    text-decoration: underline;
  }
</style>

<div class="header-container">
  <h1>Parveez Banu Syed Azizuddin</h1>
  <p>Robotics Enthusiast | ROS2 Developer</p>
</div>

## About Me

Welcome to my robotics portfolio! I am passionate about creating intelligent autonomous systems by combining hardware and software. Here you will find my featured projects showcasing my skills in ROS 2, Gazebo, embedded systems, and CAD modeling.

---

## Featured Projects

### Wall Following Robot (ROS 2 + Gazebo)

This robot autonomously follows walls using LiDAR data and ROS 2 nodes, simulated within a maze-like Gazebo environment. The robot processes real-time sensor data to maintain a stable distance from the walls.

**Challenges faced:**

- Maintaining consistent distance during tight corners with noisy sensor input.
- Filtering LiDAR data to reduce false detections.
- Tuning velocity commands for smooth navigation.

**Learning outcomes:**

- Developed sensor processing and feedback control skills.
- Improved ROS 2 node programming for real-time navigation.
- Gained experience with Gazebo simulation environments.

**Skills & tools used:**

ROS 2 Humble, Gazebo Classic, Python, LiDAR sensor integration

<div class="project-media">
  <video controls>
    <source src="assets/images/Wall_follower.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/wall_follower_bot" target="_blank" rel="noopener">GitHub Repository</a>
</div>

---

### Obstacle Avoidance with LiDAR (ROS 2 + Gazebo)

A two-wheeled differential drive robot with LiDAR sensor to avoid obstacles autonomously in a Gazebo environment. Processes laser scan data and publishes velocity commands for smooth movement.

**Challenges faced:**

- Processing sensor data accurately for obstacle detection.
- Tuning smooth velocity commands.
- Configuring Gazebo plugins for sensor simulation.

**Learning outcomes:**

- Mastered ROS 2 message handling and sensor integration.
- Learned Gazebo robot modeling and environment design.
- Enhanced autonomous navigation understanding.

**Skills & tools used:**

ROS 2 Humble, Python, Gazebo Classic, URDF/Xacro

<div class="project-media">
  <video controls>
    <source src="assets/images/Obstacle_Avoidance.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/obstacle_avoidance_lidar" target="_blank" rel="noopener">GitHub Repository</a>
</div>

---

### Robot Description and Simulation (Fusion 360 + ROS 2 + Gazebo)

Custom two-wheeled robot designed in Fusion 360, described in URDF/Xacro with STL meshes, integrated with Gazebo plugins for realistic simulation.

**Challenges faced:**

- Managing mesh references and visualization.
- Configuring differential drive plugins.
- Syncing URDF with Gazebo extensions.

**Learning outcomes:**

- Experience in CAD to ROS simulation pipeline.
- Robot plugin configuration in Gazebo.
- Integration of hardware models into software simulation.

**Skills & tools used:**

Fusion 360, ROS 2 Humble, Gazebo Classic, URDF/Xacro

<div class="project-media">
  <img src="assets/images/ros2_bot_description.png" alt="Robot Description" />
  <video controls>
    <source src="assets/images/robot_teleop.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/ros2_bot_description" target="_blank" rel="noopener">GitHub Repository</a>
</div>

---

### Geometric Shape Drawer using Turtlesim (ROS 2)

A ROS 2 Python node that controls turtlesim to draw geometric shapes interactively. Demonstrates ROS 2 communication (publishers, subscribers, services).

**Challenges faced:**

- Synchronizing service calls and velocity commands.
- Timing and velocity tuning for precise shapes.

**Learning outcomes:**

- Improved ROS 2 communication skills.
- Python scripting for interactive robotics.
- Visualization with Turtlesim.

**Skills & tools used:**

ROS 2 Humble, Python, Turtlesim

<div class="project-media">
  <video controls>
    <source src="assets/images/Turtlesim.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/turtlesim_shape_drawer" target="_blank" rel="noopener">GitHub Repository</a>
</div>

---

### ADC-Based Speed-Controlled Robot

Robot with multiple sensors for obstacle avoidance, cliff detection, and line following. Speed control through ADC potentiometer on ATmega16.

**Challenges faced:**

- Balancing sensor input and motor speed.
- Accurate ADC sampling and PWM control.
- Integrating multiple sensors with microcontroller.

**Learning outcomes:**

- Mastered ADC use in microcontrollers.
- Developed embedded sensor integration.
- Hardware-software co-design.

**Skills & tools used:**

Embedded C, ATmega16, ADC, IR sensors

<div class="project-media">
  <img src="assets/images/adc_robot_diagram.png" alt="ADC Robot Diagram" />
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/adc_speed_controlled_robot" target="_blank" rel="noopener">GitHub Repository</a>
</div>

---

### Obstacle Avoider Robot

Microcontroller robot avoiding obstacles using IR sensors and L293D motor driver, programmed in Embedded C.

**Challenges faced:**

- Reliable IR sensor readings under various conditions.
- Smooth motor control timing.
- Effective power management.

**Learning outcomes:**

- Embedded C for real-time control.
- Sensor integration on microcontrollers.
- Motor driver interfacing.

**Skills & tools used:**

Embedded C, ATmega16, IR sensors, L293D

<div class="project-media side-by-side">
  <img src="assets/images/obstacle_avoider.png" alt="Obstacle Avoider Robot" />
  <img src="assets/images/Obstacle_avoider_connection.png" alt="Obstacle Avoider Circuit" />
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/obstacle_avoider_robot" target="_blank" rel="noopener">GitHub Repository</a>
</div>

---

### Table Top Robot

Designed to detect table edges and avoid falls using IR sensors on ATmega16 microcontroller.

**Challenges faced:**

- Fast, reliable edge detection.
- Reducing false positives.

**Learning outcomes:**

- Mastered IR edge detection.
- Embedded safety control design.

**Skills & tools used:**

Embedded C, ATmega16, IR Sensors

<div class="project-media">
  <img src="assets/images/table_top.png" alt="Table Top Robot" />
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/table_top_robot" target="_blank" rel="noopener">GitHub Repository</a>
</div>

---

### Line Follower Robot

Robot following black line with bottom IR sensors. Embedded C programming with analog sensor input.

**Challenges faced:**

- Filtering sensor noise.
- Sensor placement optimization.
- Smooth motor control on curves.

**Learning outcomes:**

- Sensor-based path following.
- Embedded control techniques.

**Skills & tools used:**

Embedded C, ATmega16, IR sensors, Motor driver

<div class="project-media side-by-side">
  <img src="assets/images/line_follower.png" alt="Line Follower Robot" />
  <img src="assets/images/line_follower_connection.png" alt="Line Follower Circuit" />
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/line_follower_robot" target="_blank" rel="noopener">GitHub Repository</a>
</div>
