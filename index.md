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
body {
  font-family: 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  background: linear-gradient(135deg, #f5f9ff, #e0f0ff);
  color: #1a1a1a;
  margin: 0 20px;
  text-align: center;
  line-height: 1.6;
}

/* ============================
   Header Styles
=============================== */
.header-container {
  margin-top: 50px;
  margin-bottom: 50px;
}

.header-container h1 {
  font-size: 3rem;
  font-weight: 900;
  background: linear-gradient(270deg, #357edd, #ff6ec7, #ffba3c);
  background-size: 600% 600%;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: gradientMove 8s ease infinite, fadeInDown 1s ease forwards;
  letter-spacing: 1.2px;
}

.header-container p {
  font-size: 1.4rem;
  font-weight: 600;
  color: #357edd;
  margin-top: 10px;
  animation: fadeInUp 1s ease forwards;
  animation-delay: 0.3s;
}

/* ============================
   Section Headers
=============================== */
h2 {
  font-size: 2.2rem;
  color: #2a4d8f;
  margin-top: 60px;
  margin-bottom: 30px;
  font-weight: 700;
  text-align: center;
  position: relative;
  animation: fadeIn 1s ease forwards;
}

h2::after {
  content: "";
  display: block;
  width: 100px;
  height: 4px;
  margin: 8px auto 0;
  background: linear-gradient(90deg, #ff6ec7, #357edd, #ffba3c);
  border-radius: 2px;
  animation: fadeIn 1.5s ease forwards;
}

h3 {
  font-size: 1.6rem;
  color: #ff6ec7;
  margin-top: 40px;
  margin-bottom: 15px;
  animation: fadeIn 1s ease forwards;
}

/* ============================
   Paragraph & List Styles
=============================== */
p {
  max-width: 720px;
  margin-left: auto;
  margin-right: auto;
  text-align: justify;
}

ul, ol {
  max-width: 720px;
  margin-left: auto;
  margin-right: auto;
  text-align: left;
  padding-left: 1.2em;
  margin-bottom: 1em;
}

ul li, ol li {
  margin-bottom: 0.4em;
}

/* ============================
   Project Card Styles
=============================== */
.project-card {
  background: #ffffffcc;
  border-radius: 12px;
  padding: 20px;
  margin: 30px auto;
  max-width: 750px;
  box-shadow: 0 8px 20px rgba(0,0,0,0.15);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-card:hover {
  transform: translateY(-5px) scale(1.02);
  box-shadow: 0 12px 25px rgba(0,0,0,0.25);
}

.project-card h3 {
  margin-bottom: 12px;
}

/* ============================
   Media Styles
=============================== */
.media, .project-media {
  margin: 15px auto 30px auto;
  max-width: 720px;
  text-align: center;
}

.media img, .project-media img,
.media video, .project-media video {
  max-width: 100%;
  max-height: 400px;
  border-radius: 8px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.15);
}

/* Side-by-side */
.side-by-side {
  display: flex;
  gap: 20px;
  justify-content: center;
  flex-wrap: wrap;
}

.side-by-side img,
.side-by-side video {
  max-width: 48%;
  max-height: 350px;
}

/* ============================
   GitHub Links
=============================== */
.github-link {
  display: inline-block;
  margin-top: 8px;
  color: #fff;
  font-weight: 600;
  font-size: 0.95rem;
  text-decoration: none;
  padding: 6px 12px;
  border-radius: 8px;
  background: linear-gradient(90deg, #357edd, #ff6ec7, #ffba3c);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.github-link:hover {
  transform: scale(1.05);
  box-shadow: 0 4px 15px rgba(0,0,0,0.3);
}

/* ============================
   Skills Tags
=============================== */
.skill-tag {
  display: inline-block;
  margin: 5px 6px;
  padding: 6px 12px;
  border-radius: 20px;
  background: linear-gradient(90deg, #ff6ec7, #357edd, #ffba3c);
  color: #fff;
  font-weight: 600;
  font-size: 0.9rem;
  transition: transform 0.3s ease;
}

.skill-tag:hover {
  transform: scale(1.1);
}

/* ============================
   Contact Links
=============================== */
.contact-info a {
  display: inline-block;
  margin: 0 15px;
  color: #fff;
  text-decoration: none;
  font-weight: 600;
  font-size: 1.1rem;
  padding: 6px 12px;
  border-radius: 8px;
  background: linear-gradient(90deg, #357edd, #ff6ec7, #ffba3c);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.contact-info a:hover {
  transform: scale(1.1);
  box-shadow: 0 4px 15px rgba(0,0,0,0.3);
}

/* ============================
   Animations
=============================== */
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

@keyframes fadeInDown {
  from { opacity: 0; transform: translateY(-20px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes fadeInUp {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes gradientMove {
  0%{background-position:0% 50%;}
  50%{background-position:100% 50%;}
  100%{background-position:0% 50%;}
}

/* ============================
   Responsive
=============================== */
@media (max-width: 768px){
  .side-by-side {
    flex-direction: column;
  }

  .side-by-side img, .side-by-side video {
    max-width: 100%;
  }

  .header-container h1 {
    font-size: 2.2rem;
  }
  .header-container p {
    font-size: 1.2rem;
  }
}
</style>

<div class="header-container">
  <h1>Parveez Banu Syed Azizuddin</h1>
  <p>Mechatronics Engineer | Robotics Enthusiast | ROS 2 Developer</p>
</div>

## About Me

Welcome to my portfolio, a space where curiosity and continuous learning drive my journey into robotics and autonomous systems. With a foundation in Electrical and Electronics Engineering and experience as a Mechatronics Engineer, I am actively expanding my skills in ROS 2, embedded systems, and simulation through hands-on projects and self-driven exploration. This collection highlights my growth as a robotics enthusiast and my commitment to mastering the integration of hardware and software to solve real-world challenges. Explore my work and join me as I build expertise and contribute to the exciting field of robotics.

---

## Featured Projects

<div class="project-card">
### Wall Following Robot (ROS 2 + Gazebo)
This project focuses on creating a robot that maintains a steady distance alongside walls using LiDAR data. It leverages ROS 2 Humble and Gazebo Classic to simulate wall-following behavior by processing laser scan data and generating velocity commands to navigate corridors and turns smoothly.  

**Skills & tools used:** ROS 2 Humble, Python, Gazebo Classic, URDF/Xacro, LiDAR, Ubuntu Linux

<div class="project-media">
  <video controls>
    <source src="assets/images/Wall_follower.mp4" type="video/mp4" />
  </video>
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/Wall-Following-Robot-with-LiDAR" target="_blank">GitHub Repository</a>
</div>
</div>

<div class="project-card">
### Obstacle Avoidance with LiDAR (ROS 2 + Gazebo)
This project simulates a differential drive robot designed to detect and avoid obstacles dynamically while navigating an open or cluttered environment.  

**Skills & tools used:** ROS 2 Humble, Python, Gazebo Classic, URDF/Xacro, LiDAR, Ubuntu Linux

<div class="media">
  <video controls>
    <source src="assets/images/Obstacle_Avoidance.mp4" type="video/mp4" />
  </video>
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/obstacle_avoidance_lidar" target="_blank">GitHub Repository</a>
</div>
</div>

<!-- Repeat the same project-card structure for all other projects -->

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
</div>

---

## Contact

<div class="contact-info">
  <a href="mailto:parveezbanu.s@gmail.com">Email</a>
  <a href="https://github.com/parveezsyed28" target="_blank">GitHub</a>
  <a href="https://linkedin.com/in/parveez-banu2807" target="_blank">LinkedIn</a>
</div>


---


### Robot Description and Simulation using ROS2

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

Fusion 360 CAD  
ROS 2 Humble, Gazebo Classic  
URDF / Xacro Robot Modeling  
STL Meshes and Gazebo Plugins  
Python, Linux

<div class="media side-by-side">
  <video controls>
    <source src="assets/images/robot_teleop.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
</div>
<a href="https://github.com/parveezsyed28/ros2_bot_description" target="_blank" class="github-link">GitHub Repository</a>

---

### Geometric Shape Drawer using Turtlesim

A ROS 2 Python node that controls the turtlesim to draw geometric shapes based on interactive user input. It includes service calls to reset the turtlesim, allowing repeated shape drawing. This project helps demonstrate ROS 2 communication concepts like publishers, subscribers, and service clients in a simple and visual way.

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

ROS 2 Humble, Python  
Turtlesim Simulator  
Publisher/Subscriber and Service Calls

<div class="media">
  <video controls>
    <source src="assets/images/Turtlesim.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
</div>
<a href="https://github.com/parveezsyed28/user_input_turtle_shape" target="_blank" class="github-link">GitHub Repository</a>

---

### ADC-Based Robot (Analog to Digital Conversion)

This advanced robot integrates multiple sensors for obstacle avoidance, cliff detection, and black line following. It also includes dynamic speed control using a potentiometer connected to the ATmega16 microcontroller's ADC module. The robot uses analog sensor inputs to adapt motor speed and navigate various environments.

- Utilizes front, top, left, and right IR sensors for comprehensive environment awareness.
- Speed control implemented via ADC reading from a trimpot.
- Embedded C programming for real-time sensor processing and motor control.

**Challenges faced:**

- Balancing sensor readings and motor control for smooth navigation.
- Implementing accurate ADC sampling and PWM motor speed control.
- Hardware integration of multiple sensors with the microcontroller.

**Learning outcomes:**

- Mastered ADC usage in microcontrollers for analog sensor data.
- Developed complex embedded systems integrating multiple sensors.
- Improved skills in hardware-software co-design.

**Skills & tools used:**

Embedded C, ATmega16 ADC module  
IR Sensors, Potentiometer for Speed Control  
L293D Motor Driver  
Real-time Embedded Systems

<a href="https://github.com/parveezsyed28/adc_speed_controlled_robot" target="_blank" class="github-link">GitHub Repository</a>

---

### Obstacle Avoider Robot

This microcontroller-based robot avoids obstacles using IR sensors programmed with Embedded C on the ATmega16. The robot detects obstacles using front-facing IR sensors and controls motion via an L293D motor driver. The design emphasizes robust sensor integration and real-time control logic on limited hardware.

- Implemented IR sensor interfacing and obstacle detection logic.
- Controlled motor driver signals with embedded C code.
- Developed chassis and hardware layout optimized for sensor placement.

**Challenges faced:**

- Ensuring sensor readings were reliable under different lighting conditions.
- Timing motor control signals to avoid jerky movement.
- Managing power distribution to motors and sensors effectively.

**Learning outcomes:**

- Built expertise in embedded C programming for real-time control.
- Gained practical experience in sensor integration on microcontrollers.
- Understood motor driver interfacing and motion control.

**Skills & tools used:**

Embedded C, ATmega16  
IR Sensors, L293D Motor Driver  
PCB Design & Hardware Integration

<div class="media side-by-side">
  <img src="assets/images/obstacle_avoider.png" alt="Obstacle Avoider Robot" />
  <img src="assets/images/Obstacle_avoider_connection.png" alt="Obstacle Avoider Circuit" />
</div>
<a href="https://github.com/parveezsyed28/obstacle_avoider_robot" target="_blank" class="github-link">GitHub Repository</a>

---

### Table Top Robot

This robot is designed to detect table edges and avoid falling by using IR sensors programmed on the ATmega16 microcontroller. It continuously monitors edge proximity and maneuvers accordingly to maintain stability on the table surface.

- Used real-time IR sensor data for edge detection.
- Embedded control logic to adjust robot motion based on sensor feedback.

**Challenges faced:**

- Achieving fast and reliable edge detection for safe operation.
- Balancing sensor sensitivity and false positive reduction.

**Learning outcomes:**

- Mastered edge detection concepts with IR sensors.
- Refined embedded control strategies for safety features.

**Skills & tools used:**

Embedded C, ATmega16  
IR Sensors for Edge Detection  
Real-time Embedded Control

<div class="media">
  <img src="assets/images/table_top.png" alt="Table Top Robot" />
</div>
<a href="https://github.com/parveezsyed28/table_top_robot" target="_blank" class="github-link">GitHub Repository</a>

---

### Line Follower Robot

A robot designed to follow a black line using bottom-mounted IR sensors. The control system uses sensor feedback to maintain alignment on the path. The robot was developed with embedded C programming on the ATmega16 microcontroller, utilizing analog sensor input for reliable line detection.

- Implemented analog IR sensor interfacing for line detection.
- Developed control logic for real-time path following.
- Compact and efficient hardware design.

**Challenges faced:**

- Ensuring accurate sensor readings without noise filtering.
- Fine-tuning sensor placement for reliable line detection.
- Implementing smooth motor control to follow curves.

**Learning outcomes:**

- Gained understanding of sensor-based path following.
- Applied embedded control techniques in constrained environments.

**Skills & tools used:**

Embedded C, ATmega16  
IR Sensors, Analog Signal Processing  
Motor Driver Control

<div class="media side-by-side">
  <img src="assets/images/line_follower.png" alt="Line Follower Robot" />
  <img src="assets/images/line_follower_connection.png" alt="Line Follower Circuit" />
</div>
<a href="https://github.com/parveezsyed28/line_follower_robot" target="_blank" class="github-link">GitHub Repository</a>

---

## Skills & Tools

- ROS 2 Humble, Gazebo Classic Simulation  
- URDF / Xacro Robot Description  
- Python, Embedded C Programming  
- ATmega16 Microcontroller, L293D Motor Driver, IR Sensors  
- Fusion 360, CAD Modeling, KiCad PCB Design  
- Linux (Ubuntu), Git & GitHub


---

## Industrial Automation & Robotics Projects

### ABB RobotStudio + Teach Pendant Projects

#### Pick & Place / Sorting Simulation
**Objective:** Simulate and program ABB robot for pick & place and color sorting tasks with precise motion.  
**Tools & Environment:** ABB RobotStudio, ABB Teach Pendant, Tool Center Point (TCP) configuration  
**Key Learnings:** Understanding TCP, trajectory planning, and precise robotic motion control  
**Highlights:** Successfully implemented object manipulation and sorting sequences, demonstrating accuracy and repeatability  

#### Drawing / Pattern Simulation
**Objective:** Program ABB robot to draw geometric patterns or designs.  
**Tools & Environment:** ABB RobotStudio, ABB Teach Pendant, Tool Center Point (TCP)  
**Key Learnings:** Trajectory programming, smooth motion control, TCP adjustments for precise tool path  
**Highlights:** Executed multiple pattern-drawing sequences with minimal error, showcasing motion precision  

---

### Nachi Robot Teach Pendant Projects

#### Pick & Place
**Objective:** Control Nachi robot using teach pendant for basic pick & place tasks  
**Tools & Environment:** Nachi Teach Pendant, TCP configuration  
**Key Learnings:** Accurate tool manipulation, motion control using teach pendant  
**Highlights:** Completed object handling tasks with reliable accuracy  

#### Color Sorting
**Objective:** Program Nachi robot to sort objects based on color using teach pendant  
**Tools & Environment:** Nachi Teach Pendant, TCP configuration  
**Key Learnings:** Integration of sensor feedback with robotic motion, TCP calibration  
**Highlights:** Achieved reliable color sorting with minimal errors  

#### Drawing / Pattern Making
**Objective:** Create geometric drawings with Nachi robot using teach pendant  
**Tools & Environment:** Nachi Teach Pendant, TCP configuration  
**Key Learnings:** Trajectory planning, precise TCP adjustments, creative motion sequences  
**Highlights:** Successfully executed multiple drawing sequences with repeatable accuracy  

---

### PLC Projects

#### Water Treatment Plant Backwash Automation
**Objective:** Automate backwash sequence of pumps and valves with interlocks and fail-safes  
**Tools & Environment:** RSLogix 500 / Studio 5000, Ladder Logic, PLC sensors and actuators  
**Key Learnings:** Process automation, sequence programming, interlock implementation  
**Highlights:** Developed a reliable automated sequence ensuring safe and efficient operation  

#### Small Foundry Energy Efficiency & QA Control
**Objective:** Monitor energy usage and ensure quality control in a small foundry setup  
**Tools & Environment:** RSLogix 500 / Studio 5000, Ladder / Structured Text, PLC integration  
**Key Learnings:** Energy monitoring logic, sensor integration, process control optimization  
**Highlights:** Implemented energy-efficient control logic with basic QA monitoring  

---

## Contact

<div class="contact-info">
  <a href="mailto:parveezbanu.s@gmail.com">Email</a>
  <a href="https://github.com/parveezsyed28" target="_blank">GitHub</a>
  <a href="https://linkedin.com/in/parveez-banu2807" target="_blank">LinkedIn</a>
</div>
GitHub: <a href="https://github.com/parveezsyed28" target="_blank">github.com/parveezsyed28</a>  
LinkedIn: <a href="https://linkedin.com/in/parveez-banu2807" target="_blank">linkedin.com/in/parveez-banu2807</a>
