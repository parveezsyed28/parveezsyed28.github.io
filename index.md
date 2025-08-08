---
layout: single
title: "Parveez Banu Syed Azizuddin"
author_profile: true
permalink: /
classes: wide
---

<style>
  body {
    background: #1a1c22;
    color: #d0d7e0;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0 auto;
    max-width: 820px;
    padding: 40px 20px 60px;
    line-height: 1.5;
  }
  .header {
    text-align: center;
    margin-bottom: 30px;
  }
  .header h1 {
    color: #6fa8dc;
    font-size: 2.8rem;
    margin: 0;
  }
  .header p {
    color: #8db7f2;
    font-size: 1.1rem;
    margin-top: 8px;
    font-weight: 600;
  }
  .intro {
    text-align: center;
    margin-bottom: 50px;
    font-size: 1rem;
  }
  h2 {
    color: #8fbad3;
    font-size: 1.6rem;
    margin-top: 2.8em;
    margin-bottom: 0.6em;
    font-weight: 700;
  }
  .subheading {
    font-weight: 600;
    color: #a4c9e9;
    margin: 0.8em 0 0.3em;
  }
  .media {
    display: flex;
    justify-content: center;
    margin: 0.6em 0 1em;
  }
  .media img, .media video {
    max-height: 3.2em;
    border-radius: 5px;
    box-shadow: 0 2px 6px rgba(0,0,0,0.6);
  }
  .side-by-side {
    display: flex;
    gap: 12px;
    justify-content: center;
    margin-bottom: 0.8em;
  }
  .side-by-side img {
    max-height: 3.2em;
    border-radius: 5px;
    box-shadow: 0 2px 6px rgba(0,0,0,0.6);
  }
  .github-link {
    font-size: 0.95rem;
    font-weight: 600;
    color: #6fa8dc;
    text-decoration: none;
  }
  .github-link:hover {
    text-decoration: underline;
    color: #a4c9e9;
  }
</style>

<div class="header">
  <h1>Parveez Banu Syed Azizuddin</h1>
  <p>Robotics Enthusiast | ROS 2 Developer</p>
</div>

<p class="intro">
  Welcome to my robotics portfolio—showcasing hands-on projects in ROS 2, simulation, embedded systems, and CAD design.
</p>

## Featured Projects

### Wall Following Robot (ROS 2 + Gazebo)

This robot autonomously follows walls using LiDAR data and ROS 2 nodes, simulated within a maze-like Gazebo environment.

**Challenges faced:** Maintaining consistent distance during tight corners, filtering noisy LiDAR data, tuning velocity commands.

**Learning outcomes:** Sensor processing, ROS 2 real-time navigation, Gazebo simulation experience.

**Skills & tools used:** ROS 2 Humble, Gazebo Classic, Python, LiDAR integration.

<div class="media">
  <video controls>
    <source src="assets/images/Wall_follower.mp4" type="video/mp4" />
  </video>
</div>

[View on GitHub](https://github.com/parveezsyed28/Wall-Following-Robot-with-LiDAR){: .github-link target="_blank" }

---

### Obstacle Avoidance with LiDAR (ROS 2 + Gazebo)

A differential drive robot with LiDAR to avoid obstacles in Gazebo.

**Challenges faced:** Accurate obstacle detection, smooth velocity tuning, Gazebo sensor plugin config.

**Learning outcomes:** ROS 2 messaging, sensor integration, Gazebo modeling.

**Skills & tools used:** ROS 2 Humble, Python, Gazebo Classic, URDF/Xacro.

<div class="media">
  <video controls>
    <source src="assets/images/Obstacle_Avoidance.mp4" type="video/mp4" />
  </video>
</div>

[View on GitHub](https://github.com/parveezsyed28/obstacle_avoidance_lidar){: .github-link target="_blank" }

---

### Robot Description and Simulation (Fusion 360 + ROS 2 + Gazebo)

Custom two-wheeled robot designed in Fusion 360 with URDF/Xacro and Gazebo plugins.

**Challenges faced:** Managing mesh references, configuring drive plugins, syncing URDF with Gazebo.

**Learning outcomes:** CAD to simulation pipeline, Gazebo plugin setup, hardware-software integration.

**Skills & tools used:** Fusion 360, ROS 2 Humble, Gazebo Classic, URDF/Xacro.

<div class="media side-by-side">
  <img src="assets/images/ros2_bot_description.png" alt="Robot Description" />
  <video controls>
    <source src="assets/images/robot_teleop.mp4" type="video/mp4" />
  </video>
</div>

[View on GitHub](https://github.com/parveezsyed28/ros2_bot_description){: .github-link target="_blank" }

---

### Geometric Shape Drawer using Turtlesim (ROS 2)

ROS 2 Python node controlling turtlesim to draw geometric shapes.

**Challenges faced:** Synchronizing services and velocity commands, precise timing.

**Learning outcomes:** ROS 2 communication, Python scripting, turtlesim visualization.

**Skills & tools used:** ROS 2 Humble, Python, Turtlesim.

<div class="media">
  <video controls>
    <source src="assets/images/Turtlesim.mp4" type="video/mp4" />
  </video>
</div>

[View on GitHub](https://github.com/parveezsyed28/user_input_turtle_shape){: .github-link target="_blank" }

---

### ADC-Based Speed-Controlled Robot

Robot with sensors and ADC potentiometer for speed control on ATmega16.

**Challenges faced:** Balancing sensor inputs, accurate ADC sampling, PWM control.

**Learning outcomes:** Embedded ADC usage, sensor integration, hardware-software co-design.

**Skills & tools used:** Embedded C, ATmega16, ADC, IR sensors.

<div class="media">
  <img src="assets/images/adc_robot_diagram.png" alt="ADC Robot Diagram" />
</div>

[View on GitHub](https://github.com/parveezsyed28/ADC_based_speed_controlled_robot){: .github-link target="_blank" }

---

### Obstacle Avoider Robot (Embedded C)

Microcontroller robot avoiding obstacles using IR sensors and L293D motor driver.

**Challenges faced:** Reliable sensor readings, motor timing, power management.

**Learning outcomes:** Embedded C control, sensor integration, motor interfacing.

**Skills & tools used:** Embedded C, ATmega16, IR sensors, L293D.

<div class="media side-by-side">
  <img src="assets/images/obstacle_avoider.png" alt="Obstacle Avoider Robot" />
  <img src="assets/images/Obstacle_avoider_connection.png" alt="Obstacle Avoider Circuit" />
</div>

[View on GitHub](https://github.com/parveezsyed28/obstacle_avoider_robot){: .github-link target="_blank" }

---

### Table Top Robot

Detects table edges to avoid falls using IR sensors on ATmega16.

**Challenges faced:** Fast edge detection, reducing false positives.

**Learning outcomes:** IR sensor mastery, embedded safety controls.

**Skills & tools used:** Embedded C, ATmega16, IR Sensors.

<div class="media">
  <img src="assets/images/table_top.png" alt="Table Top Robot" />
</div>

[View on GitHub](https://github.com/parveezsyed28/table_top_robot){: .github-link target="_blank" }

---

### Line Follower Robot

Follows black line using bottom IR sensors with embedded C programming.

**Challenges faced:** Sensor noise filtering, sensor placement, smooth control.

**Learning outcomes:** Sensor-based navigation, embedded control.

**Skills & tools used:** Embedded C, ATmega16, IR sensors, Motor driver.

<div class="media side-by-side">
  <img src="assets/images/line_follower.png" alt="Line Follower Robot" />
  <img src="assets/images/line_follower_connection.png" alt="Line Follower Circuit" />
</div>

[View on GitHub](https://github.com/parveezsyed28/line_follower_robot){: .github-link target="_blank" }

