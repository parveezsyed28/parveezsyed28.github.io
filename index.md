---
layout: default
title: Parveez Banu Syed Azizuddin | Robotics Portfolio
---

<style>
  body {
    background-color: #e6f0ff; /* light pastel blue */
    color: #334466; /* dark blue-gray */
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0 20px;
  }
  a {
    color: #3366cc; /* medium blue */
    text-decoration: none;
    font-weight: 600;
  }
  a:hover {
    color: #003399; /* dark blue */
    text-decoration: underline;
  }
  header {
    background-color: #4a69ad; /* calm blue */
    color: white;
    padding: 60px 20px 40px;
    text-align: center;
    box-shadow: 0 3px 10px rgba(0,0,80,0.4);
    margin-bottom: 40px;
    border-radius: 6px;
  }
  header h1 {
    margin: 0 0 8px;
    font-weight: 900;
    font-size: 3rem;
    letter-spacing: 1.5px;
    line-height: 1.1;
  }
  header p {
    font-weight: 500;
    font-size: 1.3rem;
    font-style: italic;
    max-width: 600px;
    margin: 0 auto;
    line-height: 1.4;
  }
  h2 {
    color: #3366cc; /* medium blue */
    border-bottom: 3px solid #4a69ad; /* calm blue */
    padding-bottom: 10px;
    margin-bottom: 32px;
    font-weight: 700;
  }
  .project {
    margin-bottom: 60px;
    padding-bottom: 30px;
    border-bottom: 1px solid #a3b1d1;
  }
  .project-title {
    font-size: 1.8rem;
    color: #003366; /* dark navy blue */
    font-weight: 700;
    margin-bottom: 15px;
  }
  .project-description,
  .project-challenges,
  .project-learning,
  .project-skills {
    max-width: 720px;
    margin-bottom: 16px;
    font-size: 1rem;
    color: #334466;
  }
  ul {
    padding-left: 20px;
    margin: 8px 0 0 0;
    list-style-type: disc;
  }
  .project-media {
    margin-top: 20px;
    max-width: 720px;
    text-align: center;
  }
  .project-media img,
  .project-media video {
    border-radius: 8px;
    box-shadow: 0 3px 10px rgba(51, 102, 204, 0.3);
    max-width: 100%;
    height: auto;
    margin: 10px 0;
  }
  .project-media video {
    max-height: 320px;
    width: 100%;
  }
  .images-container {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
  }
  .images-container img {
    max-width: 48%;
  }
  .github-link {
    color: #3366cc;
    font-weight: 600;
    display: inline-block;
    margin-top: 8px;
  }
  .github-link:hover {
    color: #003399;
  }
  footer {
    color: #607799;
    border-top: 1px solid #4a69ad;
    padding: 20px;
    text-align: center;
    margin-top: 80px;
  }
</style>

<header>
  <h1>Parveez Banu Syed Azizuddin</h1>
  <p>Robotics Enthusiast | ROS2 Developer</p>
</header>

## About Me

Hi, I’m **Parveez**, a passionate robotics enthusiast driven by curiosity and creativity.  
I love bringing robots to life by blending code, sensors, and hardware into intelligent systems that solve real-world problems.  
Whether it’s building autonomous bots or exploring new possibilities with ROS 2, every project is a journey of learning and innovation.  
This portfolio showcases my hands-on experience and dedication to making robotics accessible and exciting for everyone.

---

## Featured Projects

### Wall Follower Robot

**Description:**  
A robot designed to follow a black line using bottom-mounted IR sensors. The control system uses sensor feedback to maintain alignment on the path. Developed with embedded C on the ATmega16 microcontroller, utilizing analog sensor input for reliable line detection.

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

**Skills & tools:** Embedded C, ATmega16, IR Sensors, Analog Signal Processing, Motor Driver Control

<div class="project-media images-container">
  <img src="assets/images/line_follower.png" alt="Line Follower Robot" />
  <img src="assets/images/line_follower_connection.png" alt="Line Follower Circuit" />
</div>

---

### Obstacle Avoidance with LiDAR (ROS 2 + Gazebo)

**Description:**  
This project simulates a two-wheeled differential drive robot equipped with a LiDAR sensor that autonomously avoids obstacles within a Gazebo environment. Using ROS 2 Humble and Gazebo Classic, the robot processes real-time laser scan data and publishes velocity commands for smooth navigation.

- Developed custom robot model and integrated LiDAR sensor.  
- Implemented obstacle detection and avoidance algorithms in Python.  
- Designed simulation environment replicating real-world navigation challenges.

**Challenges faced:**  
- Ensuring accurate sensor data processing and filtering.  
- Tuning velocity commands for smooth robot movement.  
- Configuring Gazebo plugins and model files for proper simulation.

**Learning outcomes:**  
- Mastered ROS 2 topics and message handling.  
- Gained experience in Gazebo robot modeling and simulation.  
- Enhanced understanding of autonomous navigation using LiDAR.

**Skills & tools:** ROS 2 Humble, Python, Gazebo Classic, URDF/Xacro, LiDAR Integration

<div class="project-media">
  <video controls>
    <source src="assets/images/Obstacle_Avoidance.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/obstacle_avoidance_lidar" target="_blank">GitHub Repository</a>
</div>

---

### ROS 2 Bot Description and Simulation

**Description:**  
Custom two-wheeled robot designed in Fusion 360 and described with URDF/Xacro files. Includes detailed STL meshes and Gazebo plugins for realistic motion simulation. Simulated within Gazebo to test movement and sensor plugins.

- Designed mechanical parts in Fusion 360.  
- Created accurate URDF and Xacro descriptions.  
- Simulated robot kinematics and sensors in Gazebo.

**Challenges faced:**  
- Managing mesh file references for visualization.  
- Configuring differential drive plugin parameters.  
- Synchronizing URDF with Gazebo XML extensions.

**Learning outcomes:**  
- Experience in robot modeling and simulation workflows.  
- Integration of CAD designs with ROS 2 simulation.  
- Skills in configuring robot plugins for Gazebo.

**Skills & tools:** Fusion 360, ROS 2 Humble, Gazebo Classic, URDF/Xacro, STL Meshes, Python

<div class="project-media">
  <img src="assets/images/ros2_bot_description.png" alt="ROS 2 Bot Description" />
  <video controls>
    <source src="assets/images/robot_teleop.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  <br />
  <a class="github-link" href="https://github.com/parveezsyed28/ros2_bot_description" target="_blank">GitHub Repository</a>
</div>

---

### Turtlesim Shape Drawer

**Description:**  
A ROS 2 Python node that controls turtlesim to draw geometric shapes based on user input. Includes service calls to reset turtlesim, demonstrating ROS 2 communication like publishers, subscribers, and service clients.

- Implemented publisher and subscriber nodes.  
- Managed CLI input and reset services.  
- Designed modular code for extensibility.

**Challenges faced:**  
- Synchronizing service calls with publisher commands.  
- Managing timing and velocity for precise shapes.

**Learning outcomes:**  
- Deepened understanding of ROS 2 communication.  
- Built interactive robotic applications.  
- Practiced Python scripting in ROS 2.

**Skills & tools:** ROS 2 Humble, Python, Turtlesim, Publisher/Subscriber, Service Calls

<div class="project-media">
  <video controls>
    <source src="assets/images/Turtlesim.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
</div>

---

### ADC-Based Speed Controlled Robot

**Description:**  
Robot integrating multiple IR sensors for obstacle avoidance, cliff detection, and black line following, with dynamic speed control via a potentiometer connected to the ATmega16 ADC.

- Utilizes front, top, left, and right IR sensors.  
- Speed control via ADC from trimpot.  
- Embedded C for real-time sensor processing.

**Challenges faced:**  
- Balancing sensor readings and motor control.  
- Accurate ADC sampling and PWM control.  
- Hardware integration of multiple sensors.

**Learning outcomes:**  
- Mastered ADC usage in microcontrollers.  
- Developed complex embedded systems.  
- Improved hardware-software co-design skills.

**Skills & tools:** Embedded C, ATmega16 ADC, IR Sensors, Potentiometer, L293D Motor Driver

<div class="project-media">
  <img src="assets/images/adc_robot_diagram.png" alt="ADC Robot Diagram" style="max-width: 80%; border-radius: 8px; box-shadow: 0 3px 10px rgba(51,102,204,0.3);" />
</div>

---

### Obstacle Avoider Robot (Embedded C)

**Description:**  
Microcontroller-based robot using IR sensors to avoid obstacles, programmed in Embedded C on the ATmega16. Controls motion via L293D motor driver with a focus on robust sensor integration.

- Implemented IR sensor interfacing and detection logic.  
- Controlled motors with embedded code.  
- Developed optimized chassis layout.

**Challenges faced:**  
- Ensuring reliable sensor readings in varied lighting.  
- Timing motor signals to avoid jerky movement.  
- Effective power distribution.

**Learning outcomes:**  
- Expertise in embedded C for real-time control.  
- Sensor integration on microcontrollers.  
- Motor driver interfacing.

**Skills & tools:** Embedded C, ATmega16, IR Sensors, L293D Motor Driver, PCB Design

<div class="project-media images-container">
  <img src="assets/images/obstacle_avoider.png" alt="Obstacle Avoider Robot" />
  <img src="assets/images/Obstacle_avoider_connection.png" alt="Obstacle Avoider Circuit" />
</div>

---

### Table Top Robot

**Description:**  
Robot designed to detect table edges and avoid falling using IR sensors with ATmega16 microcontroller. Continuously monitors edge proximity to maintain stability.

- Real-time IR sensor edge detection.  
- Embedded control adjusts motion based on feedback.

**Challenges faced:**  
- Fast, reliable edge detection.  
- Balancing sensor sensitivity and false positives.

**Learning outcomes:**  
- Mastered edge detection concepts.  
- Refined embedded safety control.

**Skills & tools:** Embedded C, ATmega16, IR Sensors, Real-time Embedded Control

<div class="project-media">
  <img src="assets/images/table_top.png" alt="Table Top Robot" />
</div>

---

<footer>
  &copy; {{ site.time | date: "%Y" }} Parveez Banu Syed Azizuddin — Robotics Portfolio
</footer>
