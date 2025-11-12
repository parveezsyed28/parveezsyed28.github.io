---
layout: single
title: "Parveez Banu Syed Azizuddin"
author_profile: true
permalink: /
classes: wide
---

<style>
/* ============================
   Overall Page Styles
=============================== */
body { font-family: 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif; background: linear-gradient(135deg, #f5f9ff, #e0f0ff); color: #1a1a1a; margin: 0 20px; text-align: center; line-height: 1.6; }
.header-container { margin-top: 50px; margin-bottom: 50px; }
.header-container h1 { font-size: 3rem; font-weight: 900; background: linear-gradient(270deg, #357edd, #ff6ec7, #ffba3c); background-size: 600% 600%; -webkit-background-clip: text; -webkit-text-fill-color: transparent; animation: gradientMove 8s ease infinite, fadeInDown 1s ease forwards; letter-spacing: 1.2px; }
.header-container p { font-size: 1.4rem; font-weight: 600; color: #357edd; margin-top: 10px; animation: fadeInUp 1s ease forwards; animation-delay: 0.3s; }
h2 { font-size: 2.2rem; color: #2a4d8f; margin-top: 60px; margin-bottom: 30px; font-weight: 700; text-align: center; position: relative; animation: fadeIn 1s ease forwards; }
h2::after { content: ""; display: block; width: 100px; height: 4px; margin: 8px auto 0; background: linear-gradient(90deg, #ff6ec7, #357edd, #ffba3c); border-radius: 2px; animation: fadeIn 1.5s ease forwards; }
h3 { font-size: 1.6rem; color: #ff6ec7; margin-top: 40px; margin-bottom: 15px; animation: fadeIn 1s ease forwards; }
p { max-width: 720px; margin-left: auto; margin-right: auto; text-align: justify; }
ul, ol { max-width: 720px; margin-left: auto; margin-right: auto; text-align: left; padding-left: 1.2em; margin-bottom: 1em; }
ul li, ol li { margin-bottom: 0.4em; }
.project-card { background: #ffffffcc; border-radius: 12px; padding: 20px; margin: 30px auto; max-width: 750px; box-shadow: 0 8px 20px rgba(0,0,0,0.15); transition: transform 0.3s ease, box-shadow 0.3s ease; }
.project-card:hover { transform: translateY(-5px) scale(1.02); box-shadow: 0 12px 25px rgba(0,0,0,0.25); }
.project-card h3 { margin-bottom: 12px; }
.media, .project-media { margin: 15px auto 30px auto; max-width: 720px; text-align: center; }
.media img, .project-media img, .media video, .project-media video { max-width: 100%; max-height: 400px; border-radius: 8px; box-shadow: 0 5px 15px rgba(0,0,0,0.15); }
.side-by-side { display: flex; gap: 20px; justify-content: center; flex-wrap: wrap; }
.side-by-side img, .side-by-side video { max-width: 48%; max-height: 350px; }
.github-link { display: inline-block; margin-top: 8px; color: #fff; font-weight: 600; font-size: 0.95rem; text-decoration: none; padding: 6px 12px; border-radius: 8px; background: linear-gradient(90deg, #357edd, #ff6ec7, #ffba3c); transition: transform 0.3s ease, box-shadow 0.3s ease; }
.github-link:hover { transform: scale(1.05); box-shadow: 0 4px 15px rgba(0,0,0,0.3); }
.skill-tag { display: inline-block; margin: 5px 6px; padding: 6px 12px; border-radius: 20px; background: linear-gradient(90deg, #ff6ec7, #357edd, #ffba3c); color: #fff; font-weight: 600; font-size: 0.9rem; transition: transform 0.3s ease; }
.skill-tag:hover { transform: scale(1.1); }
.contact-info a { display: inline-block; margin: 0 15px; color: #fff; text-decoration: none; font-weight: 600; font-size: 1.1rem; padding: 6px 12px; border-radius: 8px; background: linear-gradient(90deg, #357edd, #ff6ec7, #ffba3c); transition: transform 0.3s ease, box-shadow 0.3s ease; }
.contact-info a:hover { transform: scale(1.1); box-shadow: 0 4px 15px rgba(0,0,0,0.3); }
@keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
@keyframes fadeInDown { from { opacity: 0; transform: translateY(-20px); } to { opacity: 1; transform: translateY(0); } }
@keyframes fadeInUp { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } }
@keyframes gradientMove { 0%{background-position:0% 50%;} 50%{background-position:100% 50%;} 100%{background-position:0% 50%;} }
@media (max-width: 768px){ .side-by-side { flex-direction: column; } .side-by-side img, .side-by-side video { max-width: 100%; } .header-container h1 { font-size: 2.2rem; } .header-container p { font-size: 1.2rem; } }
</style>

<div class="header-container">
  <h1>Parveez Banu Syed Azizuddin</h1>
  <p>Mechatronics Engineer | Robotics & Embedded Systems | Automation Enthusiast</p>
</div>

## About Me

Welcome to my portfolio, a space where curiosity and continuous learning drive my journey into robotics and autonomous systems. With a foundation in Electrical and Electronics Engineering and experience as a Mechatronics Engineer, I am actively expanding my skills in ROS 2, embedded systems, and simulation through hands-on projects and self-driven exploration. This collection highlights my growth as a robotics enthusiast and my commitment to mastering the integration of hardware and software to solve real-world challenges. Explore my work and join me as I build expertise and contribute to the exciting field of robotics.

---

## ROS2 Projects

<div class="project-card">
   
<h3>Wall Following Robot (ROS 2 + Gazebo)</h3>

<p>This project focuses on creating a robot that maintains a steady distance alongside walls using LiDAR data. It leverages ROS 2 Humble and Gazebo Classic to simulate wall-following behavior by processing laser scan data and generating velocity commands to navigate corridors and turns smoothly. The robot’s custom URDF/Xacro model includes detailed sensor and actuator configurations optimized for precise wall tracking in maze-like environments.</p>

<p>
- Developed custom robot model and integrated LiDAR sensor.  
- Implemented obstacle detection and avoidance algorithms in Python.  
- Designed simulation environment replicating real-world navigation challenges.
</p>

<p><strong>Challenges faced:</strong>

   - Ensuring accurate sensor data processing and filtering for reliable obstacle detection.  
   - Tuning velocity commands to achieve smooth and safe robot movements.  
   - Configuring Gazebo plugins and model files for correct sensor simulation.
</p>

<p><strong>Learning outcomes:</strong>

- Mastered ROS 2 topics and message handling for real-time sensor and control data.  
- Gained experience in Gazebo robot modeling and simulation environment setup.  
- Enhanced understanding of autonomous navigation using LiDAR-based perception.
</p>

<p><strong>Skills & Tools:</strong>

ROS 2 Humble, Python  
Gazebo Classic Simulation  
.</p>


<div class="project-media">
  <video controls><source src="assets/images/Wall_follower.mp4" type="video/mp4" /></video>
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/Wall-Following-Robot-with-LiDAR" target="_blank">GitHub</a>
</div>

---
   
<h3>Obstacle Avoidance Robot (ROS 2 + Gazebo)</h3>

<p>This project simulates a differential drive robot designed to detect and avoid obstacles dynamically while navigating an open or cluttered environment. Using ROS 2 and Gazebo Classic, the robot processes laser scan data to identify obstacles in real time, adapting its velocity commands to steer clear of collisions. The simulation includes a custom URDF/Xacro robot model with integrated sensors, enabling reactive navigation in unpredictable scenarios.</p>

<p>
Developed custom robot model and integrated LiDAR sensor.
- Implemented obstacle detection and avoidance algorithms in Python.
- Designed simulation environment replicating real-world navigation challenges.
</p>

<p><strong>Challenges faced:</strong>

  - Ensuring accurate sensor data processing and filtering for reliable obstacle detection.
- Tuning velocity commands to achieve smooth and safe robot movements.
- Configuring Gazebo plugins and model files for correct sensor simulation.

</p>

<p><strong>Learning outcomes:</strong>

- Mastered ROS 2 topics and message handling for real-time sensor and control data.
- Gained experience in Gazebo robot modeling and simulation environment setup.
- Enhanced understanding of autonomous navigation using LiDAR-based perception.

</p>

<p><strong>Skills & Tools:</strong>
ROS 2 Humble, Python  
Gazebo Classic Simulation  
URDF / Xacro Robot Description  
LiDAR sensor integration  
Ubuntu Linux, Visual Studio Code
  
</p>


<div class="project-media">
  <video controls><source src="assets/images/Obstacle_Avoidance.mp4" type="video/mp4" /></video>
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/obstacle_avoidance_lidar" target="_blank">GitHub</a>
</div>

---

<h3>Robot Description & Simulation (ROS2 + Fusion 360)</h3>

<p>Custom two-wheeled robot modeled in Fusion 360 and simulated in Gazebo with URDF/Xacro.</p>

<p><strong>Skills & Tools:</strong> Fusion 360, ROS 2 Humble, Gazebo, URDF/Xacro</p>

<div class="media">
  <video controls><source src="assets/images/robot_teleop.mp4" type="video/mp4" /></video>
</div>
<a class="github-link" href="https://github.com/parveezsyed28/ros2_bot_description" target="_blank">GitHub</a>
</div>

---
   
<h3>Turtlesim Geometric Shape Drawer</h3>

<p>ROS 2 Python node draws shapes in Turtlesim based on user input.</p>

<p><strong>Skills & Tools:</strong> ROS 2 Humble, Python, Turtlesim</p>

<div class="media">
  <video controls><source src="assets/images/Turtlesim.mp4" type="video/mp4" /></video>
</div>
<a class="github-link" href="https://github.com/parveezsyed28/user_input_turtle_shape" target="_blank">GitHub</a>
</div>

---

## Embedded Projects

<div class="project-card">
   
<h3>ADC-Based Robot</h3>

<p>Obstacle avoidance, cliff detection, line following, and potentiometer-based speed control using ATmega16 ADC.</p>

<p><strong>Skills & Tools:</strong> Embedded C, ATmega16, IR Sensors, L293D, Potentiometer</p>

<a class="github-link" href="https://github.com/parveezsyed28/adc_speed_controlled_robot" target="_blank">GitHub</a>
</div>

---

<div class="project-card">
<h3>Obstacle Avoider Robot</h3>

<p>IR sensor-based obstacle detection and motor control with ATmega16 microcontroller.</p>

<p><strong>Skills & Tools:</strong> Embedded C, ATmega16, IR Sensors, L293D</p>

<div class="media side-by-side">
  <img src="assets/images/obstacle_avoider.png" alt="Obstacle Avoider Robot" />
  <img src="assets/images/Obstacle_avoider_connection.png" alt="Obstacle Avoider Circuit" />
</div>
<a class="github-link" href="https://github.com/parveezsyed28/obstacle_avoider_robot" target="_blank">GitHub</a>
</div>

---

<div class="project-card">
<h3>Table Top Robot</h3>

<p>Edge-detection robot preventing falls, using IR sensors on ATmega16.</p>

<p><strong>Skills & Tools:</strong> Embedded C, ATmega16, IR Sensors</p>

<div class="media">
  <img src="assets/images/table_top.png" alt="Table Top Robot" />
</div>
<a class="github-link" href="https://github.com/parveezsyed28/table_top_robot" target="_blank">GitHub</a>
</div>


---

<div class="project-card">
<h3>Line Follower Robot</h3>

<p>Black line following using bottom IR sensors, motor control via ATmega16 and L293D.</p>

<p><strong>Skills & Tools:</strong> Embedded C, ATmega16, IR Sensors, L293D</p>

<div class="media side-by-side">
  <img src="assets/images/line_follower.png" alt="Line Follower Robot" />
  <img src="assets/images/line_follower_connection.png" alt="Line Follower Circuit" />
</div>
<a class="github-link" href="https://github.com/parveezsyed28/line_follower_robot" target="_blank">GitHub</a>
</div>

---

<div class="project-card">
## Industrial Automation Projects

<h3>ABB RobotStudio + Teach Pendant</h3>

- **Pick & Place / Sorting Simulation**  
- **Drawing / Pattern Simulation**  
<p><strong>Tools:</strong> ABB RobotStudio, ABB Teach Pendant, TCP</p> 
<p><strong>Skills Learned:</strong> Trajectory planning, TCP configuration, precise motion control</p>

<h3>Nachi Robot Teach Pendant</h3>

- **Pick & Place & Color Sorting**  
- **Drawing / Pattern Making**  
<p><strong>Tools:</strong> Nachi Teach Pendant, TCP</p>
<p><strong>Skills Learned:</strong> Motion sequences, sensor integration, TCP adjustments</p>

### PLC Projects

<h3>Water Treatment Plant Backwash Automation</h3> 
<h3>Small Foundry Energy Efficiency & QA Control</h3>  
<p><strong>Tools:</strong> RSLogix 5000, Ladder/Structured Text, PLCs</p> 
<p><strong>Skills Learned:</strong> Sequence programming, interlock logic, process optimization</p>

---

## Skills & Tools

<div>
<span class="skill-tag">ROS 2 Humble</span>
<span class="skill-tag">Gazebo Classic</span>
<span class="skill-tag">URDF / Xacro</span>
<span class="skill-tag">Python</span>
<span class="skill-tag">Embedded C</span>
<span class="skill-tag">ATmega16</span>
<span class="skill-tag">L293D Motor Driver</span>
<span class="skill-tag">IR Sensors</span>
<span class="skill-tag">Fusion 360</span>
<span class="skill-tag">CAD Modeling</span>
<span class="skill-tag">KiCad PCB Design</span>
<span class="skill-tag">Linux (Ubuntu)</span>
<span class="skill-tag">Git & GitHub</span>
<span class="skill-tag">ABB RobotStudio</span>
<span class="skill-tag">Nachi Teach Pendant</span>
<span class="skill-tag">PLC Ladder Logic</span>
</div>

---

## Contact

<div class="contact-info">
<a href="mailto:parveezbanu.s@gmail.com">Email</a>
<a href="https://github.com/parveezsyed28" target="_blank">GitHub</a>
<a href="https://linkedin.com/in/parveez-banu2807" target="_blank">LinkedIn</a>
</div>
