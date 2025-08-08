---
layout: single
title: "Parveez Banu Syed Azizuddin"
author_profile: true
permalink: /
classes: wide
---

<style>
/* Header */
.header-container {
  text-align: center;
  margin: 40px auto 60px;
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

/* General text */
body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-color: #1a1a1a;
  color: #d1d9e6;
  line-height: 1.6;
}
h2, h3 {
  margin-top: 2em;
  margin-bottom: 0.5em;
  font-weight: 700;
}
h2 {
  font-size: 2.2rem;
  border-bottom: 3px solid #4a90e2;
  padding-bottom: 8px;
  color: #7db1f9;
}
h3 {
  font-size: 1.4rem;
  color: #a6c8ff;
}

/* Project section */
.project-title {
  font-size: 1.7rem;
  font-weight: 800;
  color: #4a90e2;
  margin-bottom: 10px;
}

.project-subsection {
  margin-bottom: 0.8rem;
  font-size: 1rem;
  color: #b0bec5;
}

.project-subsection strong {
  color: #7db1f9;
  font-weight: 700;
}

.project-subsection ul {
  list-style-type: disc;
  margin-left: 20px;
  margin-top: 6px;
  color: #c0cbdc;
}

/* Media */
.project-media {
  margin-top: 15px;
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
  margin-bottom: 12px;
}

/* Side by side images */
.side-by-side {
  display: flex;
  justify-content: center;
  gap: 18px;
  flex-wrap: wrap;
}
.side-by-side img {
  max-width: 48%;
  height: auto;
  border-radius: 6px;
  box-shadow: 0 3px 10px rgba(0,0,0,0.7);
  margin-bottom: 12px;
}

/* GitHub icon link */
.github-link {
  display: inline-flex;
  align-items: center;
  color: #4a90e2;
  text-decoration: none;
  font-weight: 600;
  margin-top: 4px;
  gap: 6px;
  font-size: 0.95rem;
}
.github-link svg {
  width: 18px;
  height: 18px;
  fill: #4a90e2;
  transition: fill 0.2s ease;
}
.github-link:hover svg {
  fill: #7db1f9;
}
.github-link:hover {
  text-decoration: underline;
}

/* Responsive adjustments */
@media (max-width: 600px) {
  .header-container h1 {
    font-size: 2.2rem;
  }
  .header-container p {
    font-size: 1rem;
  }
  h2 {
    font-size: 1.8rem;
  }
  .project-title {
    font-size: 1.3rem;
  }
  .side-by-side img {
    max-width: 100%;
  }
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
  <a class="github-link" href="https://github.com/parveezsyed28/Wall-Following-Robot-with-LiDAR" target="_blank" rel="noopener">
    <svg viewBox="0 0 16 16" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8a8 8 0 005.47 7.59c.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2 .37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.22 2.2.82a7.67 7.67 0 012-.27 7.65 7.65 0 012 .27c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.28.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8 8 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
    GitHub Repository
  </a>
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
  <a class="github-link" href="https://github.com/parveezsyed28/obstacle_avoidance_lidar" target="_blank" rel="noopener">
    <svg viewBox="0 0 16 16" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8a8 8 0 005.47 7.59c.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2 .37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.22 2.2.82a7.67 7.67 0 012-.27 7.65 7.65 0 012 .27c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.28.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8 8 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
    GitHub Repository
  </a>
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
  <a class="github-link" href="https://github.com/parveezsyed28/ros2_bot_description" target="_blank" rel="noopener">
    <svg viewBox="0 0 16 16" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8a8 8 0 005.47 7.59c.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2 .37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.22 2.2.82a7.67 7.67 0 012-.27 7.65 7.65 0 012 .27c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.28.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8 8 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
    GitHub Repository
  </a>
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
  <a class="github-link" href="https://github.com/parveezsyed28/user_input_turtle_shape" target="_blank" rel="noopener">
    <svg viewBox="0 0 16 16" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8a8 8 0 005.47 7.59c.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2 .37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.22 2.2.82a7.67 7.67 0 012-.27 7.65 7.65 0 012 .27c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.28.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8 8 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
    GitHub Repository
  </a>
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
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/ADC_based_speed_controlled_robot" target="_blank" rel="noopener">
    <svg viewBox="0 0 16 16" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8a8 8 0 005.47 7.59c.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2 .37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.22 2.2.82a7.67 7.67 0 012-.27 7.65 7.65 0 012 .27c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.28.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8 8 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
    GitHub Repository
  </a>
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
</div>
<a class="github-link" href="https://github.com/parveezsyed28/obstacle_avoider_robot" target="_blank" rel="noopener" style="display:block; text-align:center; margin-top:6px;">
  <svg viewBox="0 0 16 16" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8a8 8 0 005.47 7.59c.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2 .37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.22 2.2.82a7.67 7.67 0 012-.27 7.65 7.65 0 012 .27c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.28.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8 8 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
  GitHub Repository
</a>

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
  <a class="github-link" href="https://github.com/parveezsyed28/table_top_robot" target="_blank" rel="noopener">
    <svg viewBox="0 0 16 16" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8a8 8 0 005.47 7.59c.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2 .37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.22 2.2.82a7.67 7.67 0 012-.27 7.65 7.65 0 012 .27c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.28.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8 8 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
    GitHub Repository
  </a>
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
</div>
<a class="github-link" href="https://github.com/parveezsyed28/line_follower_robot" target="_blank" rel="noopener" style="display:block; text-align:center; margin-top:6px;">
  <svg viewBox="0 0 16 16" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8a8 8 0 005.47 7.59c.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2 .37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.22 2.2.82a7.67 7.67 0 012-.27 7.65 7.65 0 012 .27c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.28.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8 8 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
  GitHub Repository
</a>
