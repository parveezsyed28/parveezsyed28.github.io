---
layout: single
title: "Parveez Banu Syed Azizuddin"
author_profile: true
permalink: /
classes: wide
---

## About Me

Welcome to my portfolio — a vibrant collection fueled by passion, creativity, and a relentless drive for robotics! Dive into projects that showcase how I bring sensors, control systems, and software together to build robots that sense, decide, and act with purpose. Each piece here reflects my excitement for hands-on learning and my unstoppable curiosity in the world of robotics, where every challenge sparks innovation and growth.

---

<style>
.project-card {
  display: flex;
  flex-wrap: wrap;
  margin-bottom: 3rem;
  background: #fff;
  box-shadow: 0 4px 12px rgba(0,0,0,0.12);
  border-radius: 10px;
  overflow: hidden;
}
.project-media {
  flex: 1 1 380px;
  max-width: 380px;
  object-fit: cover;
}
.project-details {
  flex: 1 1 500px;
  padding: 1.5rem 2rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.project-details h3 {
  margin-top: 0;
  color: #2c3e50;
}
.project-details ul {
  margin-top: 0.5rem;
  margin-bottom: 1rem;
}
.project-btn {
  margin-top: 1rem;
  align-self: flex-start;
  background: #007acc;
  color: #fff !important;
  padding: 0.5rem 1rem;
  border-radius: 6px;
  text-decoration: none;
  font-weight: 600;
  transition: background 0.3s ease;
}
.project-btn:hover {
  background: #005fa3;
}
</style>

---

## Featured Projects

<div class="project-card">
  <video class="project-media" controls poster="/assets/images/Wall_follower.mp4">
    <source src="/assets/images/Wall_follower.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <div class="project-details">
    <h3>Wall Following Robot (ROS 2 + Gazebo)</h3>
    <p>This robot autonomously follows walls using LiDAR data and ROS 2 nodes in a maze-like Gazebo simulation.</p>
    <ul>
      <li>Developed ROS 2 node to subscribe to LiDAR scan and control movement.</li>
      <li>Tuned control logic for stable wall following.</li>
      <li>Simulated in Gazebo environment.</li>
    </ul>

    <p><strong>Challenges faced:</strong><br>
    - Maintaining stable distance in tight corners and noisy sensor data.<br>
    - Filtering LiDAR data to avoid false positives.<br>
    - Balancing velocity for smooth and safe navigation.</p>

    <p><strong>Learning outcomes:</strong><br>
    - Developed skills in sensor processing and feedback control.<br>
    - Advanced ROS 2 node programming for navigation tasks.<br>
    - Improved Gazebo environment setup and simulation design.</p>

    <a href="https://github.com/parveezsyed28/wall_follower_bot" class="project-btn" target="_blank" rel="noopener">View Code</a>
  </div>
</div>

<div class="project-card">
  <video class="project-media" controls poster="/assets/images/Obstacle_Avoidance.mp4">
    <source src="/assets/images/Obstacle_Avoidance.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <div class="project-details">
    <h3>Obstacle Avoidance (ROS 2 + Gazebo)</h3>
    <p>Two-wheeled robot equipped with LiDAR for autonomous obstacle avoidance in a Gazebo simulated environment.</p>
    <ul>
      <li>Custom robot model with LiDAR sensor.</li>
      <li>Implemented obstacle detection and avoidance algorithms in Python.</li>
      <li>Configured Gazebo plugins for accurate simulation.</li>
    </ul>

    <p><strong>Challenges faced:</strong><br>
    - Ensuring accurate sensor data processing and filtering for reliable obstacle detection.<br>
    - Tuning velocity commands to achieve smooth and safe robot movements.<br>
    - Configuring Gazebo plugins and model files correctly.</p>

    <p><strong>Learning outcomes:</strong><br>
    - Mastered ROS 2 topics and message handling for real-time sensor data.<br>
    - Gained experience in Gazebo robot modeling and simulation environment.<br>
    - Enhanced understanding of LiDAR-based autonomous navigation.</p>

    <a href="https://github.com/parveezsyed28/obstacle_avoidance_lidar" class="project-btn" target="_blank" rel="noopener">View Code</a>
  </div>
</div>

<div class="project-card">
  <img src="/assets/images/obstacle_avoider.png" alt="Obstacle Avoider Robot" class="project-media" />
  <div class="project-details">
    <h3>Obstacle Avoider Robot (Embedded C)</h3>
    <p>Microcontroller-based robot using IR sensors and L293D motor driver programmed in Embedded C.</p>
    <ul>
      <li>Implemented obstacle detection logic with IR sensors.</li>
      <li>Motor control via embedded C on ATmega16.</li>
      <li>Optimized chassis design for sensor placement.</li>
    </ul>

    <p><strong>Challenges faced:</strong><br>
    - Ensuring sensor reliability under varying conditions.<br>
    - Timing motor control signals to avoid jerky motion.<br>
    - Managing power distribution effectively.</p>

    <p><strong>Learning outcomes:</strong><br>
    - Gained expertise in embedded C programming for real-time control.<br>
    - Practiced sensor integration on microcontrollers.<br>
    - Understood motor driver interfacing and control.</p>
  </div>
</div>

<div class="project-card">
  <video class="project-media" controls poster="/assets/images/Turtlesim.mp4">
    <source src="/assets/images/Turtlesim.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <div class="project-details">
    <h3>Geometric Shape Drawer using Turtlesim (ROS 2)</h3>
    <p>ROS 2 Python node to control turtlesim to draw shapes based on user input with reset service calls.</p>
    <ul>
      <li>Implemented publisher/subscriber nodes for turtle velocity.</li>
      <li>Handled CLI input and service calls.</li>
      <li>Modular code for easy extension.</li>
    </ul>

    <p><strong>Challenges faced:</strong><br>
    - Synchronizing service calls and velocity commands.<br>
    - Managing timing and velocity for precise shape drawing.</p>

    <p><strong>Learning outcomes:</strong><br>
    - Deepened understanding of ROS 2 communication patterns.<br>
    - Improved ability to build interactive robotic applications.<br>
    - Practiced Python scripting in ROS 2 nodes.</p>
  </div>
</div>

<div class="project-card">
  <img src="/assets/images/line_follower.png" alt="Line Follower Robot" class="project-media" />
  <div class="project-details">
    <h3>Line Follower Robot (Embedded C)</h3>
    <p>Robot follows black line using analog IR sensors on ATmega16 microcontroller.</p>
    <ul>
      <li>Implemented analog IR sensor interfacing.</li>
      <li>Developed control logic for path following.</li>
      <li>Designed compact hardware.</li>
    </ul>

    <p><strong>Challenges faced:</strong><br>
    - Filtering sensor noise for accurate line detection.<br>
    - Optimizing sensor placement and motor control.</p>

    <p><strong>Learning outcomes:</strong><br>
    - Applied embedded control techniques in constrained environments.<br>
    - Gained understanding of sensor-based navigation.</p>
  </div>
</div>

<div class="project-card">
  <img src="/assets/images/table_top.png" alt="Table Top Robot" class="project-media" />
  <div class="project-details">
    <h3>Table Top Robot (Embedded C)</h3>
    <p>Designed to detect table edges and avoid falling using IR sensors programmed on ATmega16.</p>
    <ul>
      <li>Used real-time IR sensor data for edge detection.</li>
      <li>Embedded control logic to adjust motion.</li>
    </ul>

    <p><strong>Challenges faced:</strong><br>
    - Achieving fast, reliable edge detection.<br>
    - Balancing sensor sensitivity to reduce false positives.</p>

    <p><strong>Learning outcomes:</strong><br>
    - Mastered IR sensor edge detection.<br>
    - Refined embedded safety control strategies.</p>
  </div>
</div>

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
- LinkedIn: [linkedin.com/in/parveez-banu-syed-azizuddin2807](https://www.linkedin.com/in/parveez-banu2807)
