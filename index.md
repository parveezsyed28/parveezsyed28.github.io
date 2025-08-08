---
layout: single
title: "Parveez Banu Syed Azizuddin"
author_profile: true
permalink: /
classes: wide
---

<style>
  /* General Body */
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #121212;
    color: #d0d7ff;
    max-width: 900px;
    margin: 0 auto;
    padding: 20px 25px 50px;
    line-height: 1.45;
  }

  /* Remove underlines on headings */
  h1, h2, h3 {
    border-bottom: none !important;
    padding-bottom: 0 !important;
    margin-bottom: 0.6em;
  }

  /* Header Container */
  .header-container {
    text-align: center;
    margin: 60px 0 30px;
  }
  .header-container h1 {
    font-size: 2.8rem;
    font-weight: 900;
    color: #4a90e2;
    margin: 0;
    letter-spacing: 1.1px;
  }
  .header-container p {
    font-size: 1.2rem;
    font-weight: 600;
    color: #7f9ce5;
    margin-top: 8px;
    letter-spacing: 0.5px;
  }

  /* Section Titles */
  h2 {
    font-size: 1.7rem;
    font-weight: 700;
    color: #7aa7ff;
    margin-top: 3rem;
  }

  /* Subsection Titles */
  .subsection-title {
    font-weight: 600;
    color: #a0b6ff;
    margin-top: 1rem;
    margin-bottom: 0.3rem;
  }

  /* Paragraph and Lists */
  p, ul {
    font-size: 1rem;
    margin-top: 0.25rem;
    margin-bottom: 1rem;
  }
  ul {
    margin-left: 22px;
  }

  /* Media Containers */
  .media-container {
    margin: 12px 0 18px;
    max-width: 100%;
    display: flex;
    justify-content: center;
  }
  .media-container img,
  .media-container video {
    max-height: 2.5em; /* matches text line height nicely */
    width: auto;
    border-radius: 6px;
    box-shadow: 0 3px 10px rgba(0,0,0,0.7);
  }

  /* Side by Side media */
  .side-by-side {
    display: flex;
    gap: 15px;
    justify-content: center;
    margin-bottom: 12px;
  }
  .side-by-side img {
    max-height: 2.5em;
    width: auto;
    border-radius: 6px;
    box-shadow: 0 3px 10px rgba(0,0,0,0.7);
  }

  /* GitHub link styling (text-based) */
  .github-link {
    font-weight: 600;
    color: #4a90e2;
    text-decoration: none;
    font-size: 0.9rem;
    display: inline-block;
    margin-top: 8px;
    transition: color 0.3s ease;
  }
  .github-link:hover {
    color: #a0b6ff;
    text-decoration: underline;
  }
</style>

<div class="header-container">
  <h1>Parveez Banu Syed Azizuddin</h1>
  <p>Robotics Enthusiast | ROS2 Developer</p>
</div>

Welcome to my robotics portfolio — showcasing projects in ROS 2, Gazebo, embedded systems, and CAD modeling.

---

## Wall Following Robot (ROS 2 + Gazebo)

Autonomously follows walls using LiDAR and ROS 2 nodes in a maze-like Gazebo environment.

<div class="media-container">
  <video controls>
    <source src="assets/images/Wall_follower.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
</div>

[GitHub Repository](https://github.com/parveezsyed28/Wall-Following-Robot-with-LiDAR){: .github-link target="_blank" rel="noopener" }

---

## Obstacle Avoidance with LiDAR (ROS 2 + Gazebo)

Two-wheeled differential drive robot avoiding obstacles using LiDAR in Gazebo.

<div class="media-container">
  <video controls>
    <source src="assets/images/Obstacle_Avoidance.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
</div>

[GitHub Repository](https://github.com/parveezsyed28/obstacle_avoidance_lidar){: .github-link target="_blank" rel="noopener" }

---

## Robot Description and Simulation (Fusion 360 + ROS 2 + Gazebo)

Custom two-wheeled robot designed in Fusion 360 with URDF/Xacro and Gazebo simulation.

<div class="media-container" style="flex-direction: column; gap: 10px;">
  <img src="assets/images/ros2_bot_description.png" alt="Robot Description" />
  <video controls>
    <source src="assets/images/robot_teleop.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
</div>

[GitHub Repository](https://github.com/parveezsyed28/ros2_bot_description){: .github-link target="_blank" rel="noopener" }

---

## Geometric Shape Drawer using Turtlesim (ROS 2)

ROS 2 Python node controlling turtlesim to draw shapes.

<div class="media-container">
  <video controls>
    <source src="assets/images/Turtlesim.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
</div>

[GitHub Repository](https://github.com/parveezsyed28/user_input_turtle_shape){: .github-link target="_blank" rel="noopener" }

---

## ADC-Based Speed-Controlled Robot

Robot with sensors for obstacle avoidance and speed control via ADC on ATmega16.

[GitHub Repository](https://github.com/parveezsyed28/ADC_based_speed_controlled_robot){: .github-link target="_blank" rel="noopener" }

---

## Obstacle Avoider Robot

Microcontroller robot avoiding obstacles using IR sensors and L293D driver.

<div class="side-by-side">
  <img src="assets/images/obstacle_avoider.png" alt="Obstacle Avoider Robot" />
  <img src="assets/images/Obstacle_avoider_connection.png" alt="Obstacle Avoider Circuit" />
</div>

[GitHub Repository](https://github.com/parveezsyed28/obstacle_avoider_robot){: .github-link target="_blank" rel="noopener" }

---

## Table Top Robot

Designed to detect table edges and avoid falls using IR sensors on ATmega16 microcontroller.

<div class="media-container">
  <img src="assets/images/table_top.png" alt="Table Top Robot" />
</div>

[GitHub Repository](https://github.com/parveezsyed28/table_top_robot){: .github-link target="_blank" rel="noopener" }

---

## Line Follower Robot

Robot following black line with bottom IR sensors. Embedded C programming with analog sensor input.

<div class="side-by-side">
  <img src="assets/images/line_follower.png" alt="Line Follower Robot" />
  <img src="assets/images/line_follower_connection.png" alt="Line Follower Circuit" />
</div>

[GitHub Repository](https://github.com/parveezsyed28/line_follower_robot){: .github-link target="_blank" rel="noopener" }
