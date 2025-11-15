---
layout: default
title: "Portfolio – Parveez Banu Syed Azizuddin"
---

<!-- ========================= -->
<!--       TOP NAV MENU        -->
<!-- ========================= -->

<nav class="top-nav">
  <ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#ros2-projects">ROS2 Projects</a></li>
    <li><a href="#embedded-projects">Embedded Projects</a></li>
    <li><a href="#automation-projects">Industrial Automation</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<style>
/* --------------------------- */
/*       BASIC NAV STYLE       */
/* --------------------------- */
.top-nav ul {
  list-style: none;
  padding: 0;
  display: flex;
  gap: 25px;
  background: #111;
  padding: 12px 20px;
  border-radius: 8px;
  position: sticky;
  top: 0;
  z-index: 999;
}

.top-nav ul li a {
  color: #fff;
  font-weight: bold;
  text-decoration: none;
  position: relative;
  padding: 5px 0;
}

.section-title {
  font-size: 2rem;
  margin-top: 60px;
  margin-bottom: 20px;
  color: #0a7cff;
  font-weight: 800;
  padding: 10px 15px;
  background: rgba(0, 123, 255, 0.08);
  border-left: 5px solid #0a7cff;
  border-radius: 6px;
}


/* Hover underline animation */
.top-nav ul li a::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -2px;
  width: 0;
  height: 2px;
  background: #1e90ff;
  transition: width 0.3s ease;
}

.top-nav ul li a:hover::after {
  width: 100%;
}

/* --------------------------- */
/*    PROJECT CARD + EFFECTS   */
/* --------------------------- */

.project-card {
  border: 1px solid #ddd;
  border-radius: 12px;
  padding: 15px;
  margin-bottom: 25px;
  background: #f9f9f9;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  opacity: 0;
  animation: fadeIn 1s forwards;
}

.project-card:hover {
  transform: translateY(-6px) scale(1.02);
  box-shadow: 0 8px 20px rgba(0,0,0,0.15);
}

.project-img, .project-media video {
  width: 600px;       /* fixed width */
  height: 340px;      /* fixed height */
  border-radius: 12px;
  transition: transform 0.3s ease;
  object-fit: cover;  /* ensures images/videos don’t stretch */
}

.project-card:hover .project-img,
.project-card:hover .project-media video {
  transform: scale(1.03); /* subtle zoom on hover */
}

.media.side-by-side {
  display: flex;              /* horizontal layout */
  flex-wrap: wrap;            /* allows wrapping on smaller screens */
  gap: 20px;                  /* space between images */
  justify-content: flex-start; /* align left instead of center */
}

.media.side-by-side img {
  flex: 1 1 calc(50% - 10px); /* each image takes roughly half the width minus gap */
  max-width: 100%;             /* prevents overflow */
  height: auto;
  border-radius: 12px;
  object-fit: cover;
}


/* --------------------------- */
/*      SECTION ANIMATION      */
/* --------------------------- */

.section-title {
  font-size: 2rem;
  margin-top: 60px;
  margin-bottom: 20px;
  color: #1e90ff;
  opacity: 0;
  animation: fadeSlideUp 0.8s forwards;
}

/* Fade + Slide Animations */
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(15px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes fadeSlideUp {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

/* --------------------------- */
/*       SMOOTH SCROLL         */
/* --------------------------- */
html {
  scroll-behavior: smooth;
}
</style>

---

<h1 id="home" class="section-title">👋 Welcome</h1>

Hi! I'm **Parveez Banu Syed Azizuddin**. Welcome to my portfolio, a space where curiosity and continuous learning drive my journey into robotics and autonomous systems. With a foundation in Electrical and Electronics Engineering and experience as a Mechatronics Engineer, I am actively expanding my skills in ROS 2, embedded systems, and simulation through hands-on projects and self-driven exploration. This collection highlights my growth as a robotics enthusiast and my commitment to mastering the integration of hardware and software to solve real-world challenges. Explore my work and join me as I build expertise and contribute to the exciting field of robotics.

---

<h1 id="ros2-projects" class="section-title">🤖 ROS2 Projects</h1>

## 🟦 **Wall Following Robot (ROS 2 + Gazebo)**

<div class="project-card">

  <p>
    This project focuses on creating a robot that maintains a steady distance alongside walls using LiDAR data. 
    It leverages ROS 2 Humble and Gazebo Classic to simulate wall-following behavior by processing laser scan data 
    and generating velocity commands to navigate corridors and turns smoothly. The robot’s custom URDF/Xacro model 
    includes detailed sensor and actuator configurations optimized for precise wall tracking in maze-like environments.
  </p>

  <p>
    <strong>Key Tasks:</strong><br>
    - Developed custom robot model and integrated LiDAR sensor.<br>
    - Implemented obstacle detection and avoidance algorithms in Python.<br>
    - Designed simulation environment replicating real-world navigation challenges.
  </p>

  <p>
    <strong>Challenges faced:</strong><br>
    - Ensuring accurate sensor data processing and filtering for reliable obstacle detection.<br>
    - Tuning velocity commands to achieve smooth and safe robot movements.<br>
    - Configuring Gazebo plugins and model files for correct sensor simulation.
  </p>

  <p>
    <strong>Learning outcomes:</strong><br>
    - Mastered ROS 2 topics and message handling for real-time sensor and control data.<br>
    - Gained experience in Gazebo robot modeling and simulation environment setup.<br>
    - Enhanced understanding of autonomous navigation using LiDAR-based perception.
  </p>

  <p>
    <strong>Skills & Tools:</strong><br>
    ROS 2 Humble, Python, Gazebo Classic Simulation, URDF/Xacro, RViz
  </p>

  <div class="project-media">
    <video controls>
      <source src="assets/images/Wall_follower.mp4" type="video/mp4" />
    </video>
    <br />
    <a class="github-link" href="https://github.com/parveezsyed28/Wall-Following-Robot-with-LiDAR" target="_blank">GitHub</a>
  </div>
</div>

---


## 🟦 **Obstacle Avoidance Robot (ROS 2 + Gazebo)**

<div class="project-card">
  
  <p>
    This project simulates a differential-drive robot designed to detect and avoid obstacles dynamically while navigating an open or cluttered environment. 
    Using ROS 2 Humble and Gazebo Classic, the robot processes laser scan data in real time to adjust velocity commands and steer clear of collisions. 
    The simulation uses a custom URDF/Xacro model with integrated sensors for reactive navigation in unpredictable scenarios.
  </p>

  <p>
    <strong>Key Tasks:</strong><br>
    - Developed a custom robot model and integrated LiDAR sensors.<br>
    - Implemented obstacle detection and avoidance algorithms in Python.<br>
    - Designed simulation environment replicating real-world navigation challenges.
  </p>

  <p>
    <strong>Challenges faced:</strong><br>
    - Ensuring accurate sensor data processing and filtering for reliable obstacle detection.<br>
    - Tuning velocity commands to achieve smooth and safe robot movements.<br>
    - Configuring Gazebo plugins and model files for correct sensor simulation.
  </p>

  <p>
    <strong>Learning outcomes:</strong><br>
    - Mastered ROS 2 topics and message handling for real-time sensor and control data.<br>
    - Gained experience in Gazebo robot modeling and simulation environment setup.<br>
    - Enhanced understanding of autonomous navigation using LiDAR-based perception.
  </p>

  <p>
    <strong>Skills & Tools:</strong><br>
    ROS 2 Humble, Python, Gazebo Classic Simulation, URDF/Xacro Robot Description, LiDAR sensor integration, Ubuntu Linux
  </p>

  <div class="project-media">
    <video controls>
      <source src="assets/images/Obstacle_Avoidance.mp4" type="video/mp4" />
    </video>
    <br />
    <a class="github-link" href="https://github.com/parveezsyed28/obstacle_avoidance_lidar" target="_blank">GitHub</a>
  </div>
</div>

---


## 🟦 **Robot Description & Simulation (ROS2 + Fusion 360)**

<div class="project-card">

  <p>
    This project features a custom-designed two-wheeled robot created in Fusion 360 and described with URDF/Xacro files. 
    The model includes detailed STL meshes and integrates Gazebo plugins such as the differential drive controller for realistic motion simulation. 
    The robot is tested in Gazebo to validate movement and sensor functionality, providing a foundation for further ROS 2 robotic development.
  </p>

  <p>
    <strong>Key Tasks:</strong><br>
    - Designed mechanical components in Fusion 360 and exported STL meshes.<br>
    - Created accurate URDF/Xacro descriptions with sensors and plugins.<br>
    - Simulated robot kinematics and sensor data in Gazebo.
  </p>

  <p>
    <strong>Challenges faced:</strong><br>
    - Managing mesh file references and ensuring proper visualization in Gazebo.<br>
    - Configuring differential drive plugin parameters for smooth robot control.<br>
    - Synchronizing URDF with Gazebo-specific XML extensions.
  </p>

  <p>
    <strong>Learning outcomes:</strong><br>
    - Gained experience in robot modeling and simulation workflows.<br>
    - Understood integration of hardware CAD designs with ROS 2 simulation environments.<br>
    - Developed skills in robot plugin configuration for Gazebo.
  </p>

  <p>
    <strong>Skills & Tools:</strong><br>
    Fusion 360 CAD, ROS 2 Humble, Gazebo Classic, URDF/Xacro, STL Meshes, Python, Linux
  </p>

  <div class="project-media">
    <video controls>
      <source src="assets/images/robot_teleop.mp4" type="video/mp4" />
    </video>
    <br />
    <a class="github-link" href="https://github.com/parveezsyed28/ros2_bot_description" target="_blank">GitHub</a>
  </div>
</div>

---

## 🟦 **Turtlesim Geometric Shape Drawer (ROS 2 Python)**

<div class="project-card">

  <p>
    A ROS 2 Python node that controls the Turtlesim to draw geometric shapes based on interactive user input. 
    The project includes service calls to reset the Turtlesim for repeated shape drawing and demonstrates ROS 2 communication concepts like publishers, subscribers, and service clients.
  </p>

  <p>
    <strong>Key Tasks:</strong><br>
    - Implemented publisher and subscriber nodes for turtle velocity commands.<br>
    - Handled CLI input and reset services in ROS 2.<br>
    - Designed code modularity for ease of extending shapes.
  </p>

  <p>
    <strong>Challenges faced:</strong><br>
    - Synchronizing service calls and publisher commands for smooth turtle control.<br>
    - Managing timing and velocity parameters for precise shape drawing.
  </p>

  <p>
    <strong>Learning outcomes:</strong><br>
    - Deepened understanding of ROS 2 communication patterns.<br>
    - Improved ability to build interactive robotic applications.<br>
    - Practiced Python scripting in ROS 2 nodes.
  </p>

  <p>
    <strong>Skills & Tools:</strong><br>
    ROS 2 Humble, Python, Turtlesim Simulator, Publisher/Subscriber and Service Calls
  </p>

  <div class="project-media">
    <video controls>
      <source src="assets/images/Turtlesim.mp4" type="video/mp4" />
    </video>
    <br />
    <a class="github-link" href="https://github.com/parveezsyed28/user_input_turtle_shape" target="_blank">GitHub</a>
  </div>
</div>

---


<h1 id="embedded-projects" class="section-title">🔧 Embedded Projects</h1>

## 🟦 **ADC-Based Robot**

<div class="project-card">

  <p>
    Advanced microcontroller-based robot integrating multiple sensors for obstacle avoidance, cliff detection, and black line following. Includes dynamic speed control via a potentiometer connected to the ATmega16 ADC module. Analog sensor inputs allow adaptive motor speed control for various environments.
  </p>

  <p>
    <strong>Key Tasks:</strong><br>
    - Utilized front, top, left, and right IR sensors for environment awareness.<br>
    - Implemented speed control via ADC reading from a trimpot.<br>
    - Developed embedded C code for real-time sensor processing and motor control.
  </p>

  <p>
    <strong>Challenges faced:</strong><br>
    - Balancing sensor readings and motor control for smooth navigation.<br>
    - Implementing accurate ADC sampling and PWM motor speed control.<br>
    - Integrating multiple sensors with microcontroller hardware.
  </p>

  <p>
    <strong>Learning outcomes:</strong><br>
    - Mastered ADC usage in microcontrollers.<br>
    - Built complex embedded systems integrating multiple sensors.<br>
    - Enhanced hardware-software co-design skills.
  </p>

  <p>
    <strong>Skills & Tools:</strong><br>
    Embedded C, ATmega16 ADC module, IR Sensors, Potentiometer, L293D Motor Driver, Real-time Embedded Systems
  </p>

  <a class="github-link" href="https://github.com/parveezsyed28/adc_speed_controlled_robot" target="_blank">GitHub</a>
</div>

---

## 🟦 **Obstacle Avoider Robot**

<div class="project-card">

  <p>
    Microcontroller-based robot that avoids obstacles using IR sensors programmed in Embedded C on the ATmega16. Motion is controlled via an L293D motor driver. Emphasis on robust sensor integration and real-time control logic on limited hardware.
  </p>

  <p>
    <strong>Key Tasks:</strong><br>
    - Implemented IR sensor interfacing and obstacle detection logic.<br>
    - Controlled motor driver signals using embedded C.<br>
    - Developed chassis and hardware layout optimized for sensor placement.
  </p>

  <p>
    <strong>Challenges faced:</strong><br>
    - Ensuring reliable sensor readings under varying lighting conditions.<br>
    - Timing motor control signals to avoid jerky movement.<br>
    - Managing power distribution to motors and sensors effectively.
  </p>

  <p>
    <strong>Learning outcomes:</strong><br>
    - Built expertise in embedded C for real-time control.<br>
    - Gained practical experience in sensor integration on microcontrollers.<br>
    - Learned motor driver interfacing and motion control.
  </p>

  <p>
    <strong>Skills & Tools:</strong><br>
    Embedded C, ATmega16, IR Sensors, L293D Motor Driver, PCB Design & Hardware Integration
  </p>

   <!-- Side-by-side images -->
  <div class="media side-by-side">
    <img src="assets/images/obstacle_avoider.png" alt="Obstacle Avoider Robot" />
    <img src="assets/images/Obstacle_avoider_connection.png" alt="Obstacle Avoider Circuit" />
  </div>
  <a class="github-link" href="https://github.com/parveezsyed28/obstacle_avoider_robot" target="_blank">GitHub</a>
</div>
---

## 🟦 **Table Top Robot**

<div class="project-card">

  <p>
    Designed to detect table edges and prevent falls using IR sensors on ATmega16. Continuously monitors edge proximity and adjusts motion to maintain stability.
  </p>

  <p>
    <strong>Key Tasks:</strong><br>
    - Monitored real-time IR sensor data for edge detection.<br>
    - Developed embedded control logic to adjust robot motion based on sensor feedback.
  </p>

  <p>
    <strong>Challenges faced:</strong><br>
    - Achieving fast and reliable edge detection.<br>
    - Balancing sensor sensitivity and reducing false positives.
  </p>

  <p>
    <strong>Learning outcomes:</strong><br>
    - Mastered edge detection concepts with IR sensors.<br>
    - Refined embedded control strategies for safety.
  </p>

  <p>
    <strong>Skills & Tools:</strong><br>
    Embedded C, ATmega16, IR Sensors, Real-time Embedded Control
  </p>

  <div class="project-media">
    <img class="project-img" src="assets/images/table_top.png" alt="Table Top Robot" />
  </div>

  <a class="github-link" href="https://github.com/parveezsyed28/table_top_robot" target="_blank">GitHub</a>
</div>

---

## 🟦 **Line Follower Robot**

<div class="project-card">

  <p>
    Robot designed to follow a black line using bottom-mounted IR sensors. Embedded C control on ATmega16 ensures alignment on the path using analog sensor feedback.
  </p>

  <p>
    <strong>Key Tasks:</strong><br>
    - Implemented analog IR sensor interfacing for line detection.<br>
    - Developed control logic for real-time path following.<br>
    - Designed compact and efficient hardware layout.
  </p>

  <p>
    <strong>Challenges faced:</strong><br>
    - Ensuring accurate sensor readings.<br>
    - Fine-tuning sensor placement for reliable line detection.<br>
    - Implementing smooth motor control to follow curves.
  </p>

  <p>
    <strong>Learning outcomes:</strong><br>
    - Gained understanding of sensor-based path following.<br>
    - Applied embedded control techniques in constrained environments.
  </p>

  <p>
    <strong>Skills & Tools:</strong><br>
    Embedded C, ATmega16, IR Sensors, Analog Signal Processing, Motor Driver Control
  </p>

 <div class="project-media side-by-side">
    <img class="project-img" src="assets/images/line_follower.png" alt="Line Follower Robot" />
    <img class="project-img" src="assets/images/line_follower_connection.png" alt="Line Follower Circuit" />
  </div>
  <a class="github-link" href="https://github.com/parveezsyed28/line_follower_robot" target="_blank">GitHub</a>
</div>


<h1 id="automation-projects" class="section-title">🏭 Industrial Automation</h1>

### 🔹 Industrial Robotics

#### ABB RobotStudio + Teach Pendant Projects

<div class="project-card">
<h3>Pick & Place / Sorting Simulation</h3>
<p><strong>Objective:</strong> Simulate and program ABB robot for pick & place and color sorting tasks with precise motion.</p>  
<p><strong>Tools & Environment:</strong> ABB RobotStudio, ABB Teach Pendant, Tool Center Point (TCP) configuration</p>  
<p><strong>Challenges faced:</strong>
- Programming accurate pick & place sequences while handling varying object sizes.  
- Ensuring precise motion without collisions.  
- Configuring TCP parameters for exact tool positioning.</p>
<p><strong>Learning outcomes:</strong>
- Mastered trajectory planning and tool positioning.  
- Understood ABB RobotStudio simulation and teach pendant integration.  
- Developed precise motion control sequences for industrial tasks.</p>
<p><strong>Skills & Tools:</strong> ABB RobotStudio, Teach Pendant, TCP, Motion Control</p>
</div>

<div class="project-card">
<h3>Drawing / Pattern Simulation</h3>
<p><strong>Objective:</strong> Program ABB robot to draw geometric patterns or designs with precision.</p>  
<p><strong>Tools & Environment:</strong> ABB RobotStudio, ABB Teach Pendant, TCP configuration</p>
<p><strong>Challenges faced:</strong>
- Ensuring smooth motion along curves and corners.  
- Synchronizing speed and position to minimize error.  
- Adapting TCP to different tool orientations for accuracy.</p>
<p><strong>Learning outcomes:</strong>
- Gained experience in trajectory programming for complex patterns.  
- Learned fine-tuning of TCP parameters for consistent precision.  
- Developed repeatable drawing sequences with minimal deviation.</p>
<p><strong>Skills & Tools:</strong> ABB RobotStudio, Teach Pendant, TCP, Trajectory Programming</p>
</div>

#### Nachi Robot Teach Pendant Projects

<div class="project-card">
<h3>Pick & Place</h3>
<p><strong>Objective:</strong> Control Nachi robot using teach pendant for basic pick & place tasks.</p>
<p><strong>Tools & Environment:</strong> Nachi Teach Pendant, TCP configuration</p>
<p><strong>Challenges faced:</strong>
- Learning Nachi-specific teach pendant commands.  
- Ensuring smooth motion without jerks or collisions.  
- Adapting sequences to different object sizes and positions.</p>
<p><strong>Learning outcomes:</strong>
- Mastered basic robot motion programming using teach pendant.  
- Developed skills in accurate tool manipulation.  
- Implemented reliable pick & place sequences for industrial tasks.</p>
<p><strong>Skills & Tools:</strong> Nachi Teach Pendant, TCP, Motion Control</p>
</div>

<div class="project-card">
<h3>Color Sorting</h3>
<p><strong>Objective:</strong> Program Nachi robot to sort objects based on color using teach pendant.</p>
<p><strong>Tools & Environment:</strong> Nachi Teach Pendant, TCP configuration</p>
<p><strong>Challenges faced:</strong>
- Integrating sensor feedback with robotic motion.  
- Calibrating TCP and motion sequences to align with color detection.  
- Minimizing sorting errors and misplacements.</p>
<p><strong>Learning outcomes:</strong>
- Gained experience integrating perception with motion control.  
- Developed reliable color sorting sequences.  
- Learned precise TCP adjustment for repeatable performance.</p>
<p><strong>Skills & Tools:</strong> Nachi Teach Pendant, TCP, Sensor Integration, Motion Control</p>
</div>

<div class="project-card">
<h3>Drawing / Pattern Making</h3>
<p><strong>Objective:</strong> Create geometric drawings with Nachi robot using teach pendant.</p>
<p><strong>Tools & Environment:</strong> Nachi Teach Pendant, TCP configuration</p>
<p><strong>Challenges faced:</strong>
- Achieving smooth trajectory along curves.  
- Synchronizing tool speed and orientation for precise patterns.  
- Minimizing errors over multiple repetitions.</p>
<p><strong>Learning outcomes:</strong>
- Mastered trajectory planning for creative tasks.  
- Learned fine control of TCP for precision.  
- Built repeatable pattern-making sequences using the teach pendant.</p>
<p><strong>Skills & Tools:</strong> Nachi Teach Pendant, TCP, Trajectory Programming, Motion Control</p>
</div>

### 🔹 PLC Projects

<div class="project-card">
<h3>Water Treatment Plant Backwash Automation</h3>
<p><strong>Objective:</strong> Automate backwash sequence of pumps and valves with interlocks and fail-safes.</p>  
<p><strong>Tools & Environment:</strong> RSLogix 500 / Studio 5000, Ladder Logic, PLC sensors and actuators</p>
<p><strong>Challenges faced:</strong>
- Designing safe automated sequences with interlocks.  
- Handling fail-safes to prevent system damage.  
- Integrating sensors and actuators reliably in the PLC logic.</p>
<p><strong>Learning outcomes:</strong>
- Learned process automation and sequence programming.  
- Gained experience implementing interlocks and safety features.  
- Built robust automation sequences for industrial systems.</p>
<p><strong>Skills & Tools:</strong> RSLogix 500 / Studio 5000, Ladder Logic, PLC Integration, Sensors & Actuators</p>
</div>

<div class="project-card">
<h3>Small Foundry Energy Efficiency & QA Control</h3>
<p><strong>Objective:</strong> Monitor energy usage and ensure quality control in a small foundry setup.</p>  
<p><strong>Tools & Environment:</strong> RSLogix 500 / Studio 5000, Ladder / Structured Text, PLC integration</p>
<p><strong>Challenges faced:</strong>
- Implementing energy monitoring logic.  
- Integrating sensors for quality control.  
- Optimizing process control with limited PLC resources.</p>
<p><strong>Learning outcomes:</strong>
- Gained knowledge in energy-efficient control logic.  
- Practiced sensor integration and process optimization.  
- Learned basic QA monitoring via PLC automation.</p>
<p><strong>Skills & Tools:</strong> RSLogix 500 / Studio 5000, Ladder & Structured Text, PLC Integration, Sensors</p>
</div>

---

<h1 id="skills" class="section-title">🧠 Skills</h1>

- ROS2, Gazebo, RViz  
- Python for robotics  
- Fusion 360 modeling  
- Embedded C, Arduino  
- Industrial Robotics: ABB RobotStudio & Teach Pendant, Nachi Teach Pendant  
- PLC: Allen-Bradley (RSLogix 500, Studio 5000), Delta PLC basics  
- Electromechanical troubleshooting
  

---

## 📬 Contact

<div class="contact-info">
  <p>📧 <a href="mailto:parveezbanu.s@gmail.com">parveezbanu.s@gmail.com</a></p>
  <p>🌐 <a href="https://parveezsyed28.github.io" target="_blank">Portfolio</a></p>
  <p>🔗 <a href="https://github.com/parveezsyed28" target="_blank">GitHub</a></p>
  <p>💼 <a href="https://linkedin.com/in/parveez-banu2807" target="_blank">LinkedIn</a></p>
  <p>📍 Toronto, Canada</p>
</div>

---

<!-- ========================= -->
<!--  FLOATING RETURN TO TOP   -->
<!-- ========================= -->

<button id="topBtn" title="Go to top">▲</button>

<style>
#topBtn {
  position: fixed;
  bottom: 30px;
  right: 30px;
  z-index: 9999;
  background: #1e90ff;
  color: #fff;
  border: none;
  border-radius: 50%;
  width: 45px;
  height: 45px;
  font-size: 20px;
  cursor: pointer;
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
  opacity: 0;
  pointer-events: none;
  transition: opacity 0.3s ease, transform 0.3s ease;
}

#topBtn:hover {
  transform: scale(1.1);
}
</style>

<script>
// Show button when scrolled down
window.onscroll = function() {
  const btn = document.getElementById("topBtn");
  if (document.body.scrollTop > 200 || document.documentElement.scrollTop > 200) {
    btn.style.opacity = "1";
    btn.style.pointerEvents = "auto";
  } else {
    btn.style.opacity = "0";
    btn.style.pointerEvents = "none";
  }
};

// Smooth scroll to top
document.getElementById("topBtn").onclick = function() {
  window.scrollTo({ top: 0, behavior: 'smooth' });
};
</script>

