---
layout: single
title: "Parveez Banu Syed Azizuddin"
author_profile: true
permalink: /
classes: wide
---

<link rel="stylesheet" href="{{ '/assets/css/main.css' | relative_url }}">

<div class="header-container">
  <h1>Parveez Banu Syed Azizuddin</h1>
  <p>Mechatronics Engineer | Robotics Enthusiast | ROS 2 Developer</p>
</div>


## About Me

Welcome to my portfolio, a space where curiosity and continuous learning drive my journey into robotics and autonomous systems. With a foundation in Electrical and Electronics Engineering and experience as a Mechatronics Engineer, I am actively expanding my skills in ROS 2, embedded systems, and simulation through hands-on projects and self-driven exploration. This collection highlights my growth as a robotics enthusiast and my commitment to mastering the integration of hardware and software to solve real-world challenges. Explore my work and join me as I build expertise and contribute to the exciting field of robotics.

---

## Featured Projects

### Wall Following Robot (ROS 2 + Gazebo)

This project focuses on creating a robot that maintains a steady distance alongside walls using LiDAR data. It leverages ROS 2 Humble and Gazebo Classic to simulate wall-following behavior by processing laser scan data and generating velocity commands to navigate corridors and turns smoothly. The robot’s custom URDF/Xacro model includes detailed sensor and actuator configurations optimized for precise wall tracking in maze-like environments.

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

ROS 2 Humble, Python  
Gazebo Classic Simulation  
URDF / Xacro Robot Description  
LiDAR sensor integration  
Ubuntu Linux, Visual Studio Code

<div class="project-media">
  <video controls>
    <source src="assets/images/Wall_follower.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/Wall-Following-Robot-with-LiDAR" target="_blank" rel="noopener">GitHub Repository</a>
</div>

---


### Obstacle Avoidance with LiDAR (ROS 2 + Gazebo)

This project simulates a differential drive robot designed to detect and avoid obstacles dynamically while navigating an open or cluttered environment. Using ROS 2 and Gazebo Classic, the robot processes laser scan data to identify obstacles in real time, adapting its velocity commands to steer clear of collisions. The simulation includes a custom URDF/Xacro robot model with integrated sensors, enabling reactive navigation in unpredictable scenarios.

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

ROS 2 Humble, Python  
Gazebo Classic Simulation  
URDF / Xacro Robot Description  
LiDAR sensor integration  
Ubuntu Linux, Visual Studio Code

<div class="media">
  <video controls>
    <source src="assets/images/Obstacle_Avoidance.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <br />
  <a href="https://github.com/parveezsyed28/obstacle_avoidance_lidar" target="_blank" class="github-link">GitHub Repository</a>
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

Email: <a href="mailto:parveezbanu.s@gmail.com">parveezbanu.s@gmail.com</a>  
GitHub: <a href="https://github.com/parveezsyed28" target="_blank">github.com/parveezsyed28</a>  
LinkedIn: <a href="https://linkedin.com/in/parveez-banu2807" target="_blank">linkedin.com/in/parveez-banu2807</a>
