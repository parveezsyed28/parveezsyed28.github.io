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

 .project-media {
  margin-top: 20px; /* adds space above video */
}

.project-card:hover .project-img,
.project-card:hover .project-media video {
  transform: scale(1.03); /* subtle zoom on hover */
}

.ros-card      { border-top: 4px solid #7eb8f7; }
.embedded-card { border-top: 4px solid #f7c97e; }
.plc-card      { border-top: 4px solid #7ef7b8; }
.robotics-card { border-top: 4px solid #f7a7e0; }

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

.skills {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 12px;
}

.skill-tag {
  display: inline-block;
  background-color: #007BFF;
  color: white;
  padding: 6px 12px;
  border-radius: 8px;
  font-size: 14px;
  transition: transform 0.3s, background-color 0.3s;
  cursor: default;
}

.skill-tag:hover {
  transform: translateY(-3px) scale(1.05);
  background-color: #0056b3;
}

.project-skills {
  margin-top: 12px;
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.skill-item {
  display: inline-block;
  padding: 5px 10px;
  border-radius: 6px;
  font-size: 13px;
  border: 1px solid #ccc;
  color: #333;
  background-color: #f0f0f0;
}

/* Robotics / Simulation Skills */
.skill-ros { background-color: #d0f0f5; }
.skill-gazebo { background-color: #e8e0ff; }
.skill-rviz { background-color: #cce5ff; }
.skill-urdf { background-color: #f0f0f0; }
.skill-turtlesim { background-color: #d1f7c4; }
.skill-python { background-color: #ffe0b2; }

/* CAD / Modeling Skills */
.skill-cad { background-color: #d4edda; }
.skill-fusion360 { background-color: #c8e6c9; }
.skill-stl { background-color: #f1f8e9; }

/* Embedded / Microcontroller Skills */
.skill-embedded { background-color: #fff3e0; }
.skill-atmega16 { background-color: #ffe0b2; }
.skill-ir { background-color: #ffecb3; }
.skill-l293d { background-color: #ffe6cc; }
.skill-pwm { background-color: #fff0e0; }
.skill-adc { background-color: #fff4e0; }
.skill-hardware { background-color: #f5f5dc; }
.skill-555 { background-color: #fce4ec; }
.skill-7805 { background-color: #ffe6f0; }
.skill-voltreg { background-color: #fff0f5; }

/* PLC / Industrial Automation Skills */
.skill-plc { background-color: #e0f7fa; }
.skill-allenbradley { background-color: #b2ebf2; }
.skill-delta { background-color: #b2dfdb; }
.skill-rslogix { background-color: #cceeee; }
.skill-studio5000 { background-color: #d0f0f0; }
.skill-ladder { background-color: #f0f4c3; }
.skill-structuredtext { background-color: #fff9c4; }
.skill-fbd { background-color: #e6f7ff; }

/* Robotics Industrial Skills */
.skill-abb { background-color: #e3f2fd; }
.skill-nachi { background-color: #bbdefb; }
.skill-tcp { background-color: #c8e6c9; }
.skill-motion { background-color: #dcedc8; }
.skill-trajectory { background-color: #f0f4c3; }

/* General / Tools */
.skill-linux { background-color: #f0f0f0; color: #333; }
.skill-git { background-color: #f1f1f1; color: #333; }
.skill-vscode { background-color: #e8eaf6; }


.ladder-gallery {
  display: flex;
  flex-wrap: wrap;
  gap: 15px;
  margin-top: 10px;
}

.ladder-gallery img {
  width: 100%;
  max-width: 900px;
  border-radius: 8px;
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

Hi! I'm **Parveez Banu Syed Azizuddin**. Welcome to my portfolio — a collection of projects I’ve been working on while exploring industrial automation and control systems. With a background in Electrical and Electronics Engineering and experience as a Mechatronics Engineer, I’ve been drawn to how systems behave in real-world conditions — especially how sensors, control logic, and timing come together to make something work reliably. I’ve been building projects across PLCs, embedded systems, and ROS 2, trying to understand not just how to make things work, but how to make them stable and predictable.

---

<h1 id="ros2-projects" class="section-title">🤖 ROS2 Projects</h1>

## 🟦 **Wall Following Robot (ROS 2 + Gazebo)**

<div class="project-card ros-card">

  <p>
    A mobile robot that uses LiDAR data to maintain a consistent distance from walls while navigating corridors and turns without human input. The challenge was handling unstable readings at corners and openings, where simple control logic caused oscillations and drift. I found that stabilizing distance control and prioritizing side-wall feedback produced significantly smoother and more reliable motion.
  </p>

 <p>
    <strong>Skills & Tools:</strong>
  </p>
  <div class="project-skills">
    <span class="skill-item skill-ros">ROS2</span>
    <span class="skill-item skill-python">Python</span>
    <span class="skill-item skill-gazebo">Gazebo Classic</span>
    <span class="skill-item skill-urdf">URDF/Xacro</span>
    <span class="skill-item skill-cad">Fusion 360</span>
  </div>

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

<div class="project-card ros-card">
  
  <p>
    A differential-drive robot that detects and avoids obstacles in real time using LiDAR data in a simulated environment. The challenge was translating noisy sensor input into smooth motion without abrupt stops or erratic behavior. I found that filtering scan data and tuning control loop timing had a greater impact on stability than the avoidance logic itself.
  </p>

 <p><strong>Skills & Tools:</strong></p>
<div class="project-skills">
  <span class="skill-item skill-ros">ROS 2 Humble</span>
  <span class="skill-item skill-python">Python</span>
  <span class="skill-item skill-gazebo">Gazebo Classic</span>
  <span class="skill-item skill-urdf">URDF/Xacro</span>
  <span class="skill-item skill-lidar">LiDAR </span>
  <span class="skill-item skill-linux">Ubuntu</span>
</div>

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

<div class="project-card ros-card">

  <p>
     A custom-designed two-wheeled robot modeled in CAD and simulated in Gazebo using URDF/Xacro with integrated plugins. The challenge was aligning mechanical design, URDF structure, and simulation parameters so the robot behaved realistically. I learned that correct plugin configuration and consistent frame definitions are critical for stable motion and accurate simulation.
  </p>

 
 <p><strong>Skills & Tools:</strong></p>
<div class="project-skills">
   <span class="skill-item skill-ros">ROS2 Humble</span>
  <span class="skill-item skill-python">Python</span>
  <span class="skill-item skill-gazebo">Gazebo Classic</span>
  <span class="skill-item skill-urdf">URDF/Xacro</span>
  <span class="skill-item skill-cad">Fusion 360</span>
  <span class="skill-item skill-stl">STL Meshes</span>
  <span class="skill-item skill-linux">Ubuntu</span>
</div>

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

<div class="project-card ros-card">

  <p>
    A ROS 2 Python node that controls a simulated robot to draw geometric shapes based on user input. The challenge was coordinating service calls and velocity commands to maintain precise motion without timing conflicts. I learned how synchronization between communication patterns directly affects motion accuracy, even in simple systems.
  </p>

  <p><strong>Skills & Tools:</strong></p>
<div class="project-skills">
  <span class="skill-item skill-ros">ROS2 Humble</span>
  <span class="skill-item skill-python">Python</span>
   <span class="skill-item skill-turtlesim">Turtlesim</span>
  <span class="skill-item">Publisher/Subscriber</span>
  <span class="skill-item">Service Calls</span>
</div>

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

## 🟦 **ADC-Based Multi-Behaviour Robot**

<div class="project-card embedded-card">

  <p>
    A microcontroller-based robot that combines obstacle avoidance, edge detection, and line following with dynamic speed control using ADC input. The challenge was balancing multiple sensor inputs and control behaviors on limited hardware without causing conflicts or unstable motion. I found that prioritizing behaviors and tuning response timing was key to achieving consistent performance.
  </p>

<p><strong>Skills & Tools:</strong></p>
 <div class="project-skills">
   <span class="skill-item skill-embedded">Embedded C</span>
  <span class="skill-item skill-atmega16">ATmega16</span>
  <span class="skill-item skill-ir">IR Sensors</span>
  <span class="skill-item skill-l293d">L293D Motor Driver</span>
  <span class="skill-item">Potentiometer</span>
  <span class="skill-item skill-7805">7805 Voltage Regulator</span>
  <span class="skill-item skill-555">IC555 Timer</span>
  <span class="skill-item skill-pwm">PWM Control</span>
  <span class="skill-item skill-adc">ADC</span>
</div>

  <a class="github-link" href="https://github.com/parveezsyed28/ADC_speed_controlled_robot" target="_blank">GitHub</a>
</div>

---

## 🟦 **Obstacle Avoider Robot**

<div class="project-card embedded-card">

  <p>
    A real-time obstacle-avoiding robot built on a microcontroller using IR sensors and direct motor control. The challenge was ensuring reliable sensor detection under varying conditions while maintaining smooth movement. I learned that simple, well-timed control logic is more effective than complex decision-making on constrained systems.
  </p>

<p><strong>Skills & Tools:</strong></p>
 <div class="project-skills">
  <span class="skill-item skill-embedded">Embedded C</span>
  <span class="skill-item skill-atmega16">ATmega16</span>
  <span class="skill-item skill-ir">IR Sensors</span>
  <span class="skill-item skill-l293d">L293D Motor Driver</span>
  <span class="skill-item">PCB Design</span>
  <span class="skill-item skill-hardware">Hardware Integration</span>
  <span class="skill-item skill-7805">7805 Voltage Regulator</span>
  <span class="skill-item skill-555">IC555 Timer</span>
</div>

   <!-- Side-by-side images -->
  <div class="media side-by-side">
    <img src="assets/images/obstacle_avoider.png" alt="Obstacle Avoider Robot" />
    <img src="assets/images/Obstacle_avoider_connection.png" alt="Obstacle Avoider Circuit" />
  </div>
  <a class="github-link" href="https://github.com/parveezsyed28/obstacle_avoider_robot" target="_blank">GitHub</a>
</div>
---

## 🟦 **Table Top Robot**

<div class="project-card embedded-card">

  <p>
   A robot that detects table edges and prevents falls by continuously monitoring IR sensor feedback. The challenge was achieving fast and reliable detection without false     triggers that could interrupt motion. I found that tuning sensor thresholds and response timing was critical for stable and safe operation.
  </p>


<p><strong>Skills & Tools:</strong></p>
 <div class="project-skills">
   <span class="skill-item skill-embedded">Embedded C</span>
  <span class="skill-item skill-atmega16">ATmega16</span>
  <span class="skill-item skill-ir">IR Sensors</span>
  <span class="skill-item">Real-time Embedded Control</span>
</div>
>

  <div class="project-media">
    <img class="project-img" src="assets/images/table_top.png" alt="Table Top Robot" />
  </div>

  <a class="github-link" href="https://github.com/parveezsyed28/table_top_robot" target="_blank">GitHub</a>
</div>

---

## 🟦 **Line Follower Robot**

<div class="project-card embedded-card">

  <p>
   A robot that follows a path using IR sensors to continuously correct its trajectory. The challenge was maintaining stability through turns and recovering quickly from deviations without overshooting. I learned that balancing correction speed and control response is key to smooth and accurate tracking.
  </p>

  <p><strong>Skills & Tools:</strong></p>
    <div class="project-skills">
  <span class="skill-item skill-embedded">Embedded C</span>
  <span class="skill-item skill-atmega16">ATmega16</span>
  <span class="skill-item skill-ir">IR Sensors</span>
  <span class="skill-item skill-l293d">L293D Motor Driver</span>
</div>


 <div class="project-media side-by-side">
    <img class="project-img" src="assets/images/line_follower.png" alt="Line Follower Robot" />
    <img class="project-img" src="assets/images/line_follower_connection.png" alt="Line Follower Circuit" />
  </div>
  <a class="github-link" href="https://github.com/parveezsyed28/line_follower_robot" target="_blank">GitHub</a>
</div>


<h1 id="automation-projects" class="section-title">🏭 Industrial Automation</h1>

<h2>🔹 Industrial Robotics</h2>

<h3>ABB RobotStudio + Teach Pendant Projects</h3>

<div class="project-card robotics-card">
<h3>Pick & Place / Sorting Simulation</h3>
<p>An industrial robot simulation that performs pick-and-place and sorting operations with precise motion control. The challenge was ensuring accurate positioning across varying object conditions while avoiding collisions. I learned how tool center point (TCP) configuration directly impacts repeatability and motion precision.
</p>  

<p><strong>Tools & Environment:</strong> ABB RobotStudio, ABB Teach Pendant, TCP configuration</strong></p>
<p><strong>Skills:</strong></p>
<div class="project-skills">
  <span class="skill-item skill-abb">ABB RobotStudio</span>
  <span class="skill-item skill-tcp">TCP Configuration</span>
  <span class="skill-item skill-motion">Motion Control</span>
 </div>
</div>


<div class="project-card robotics-card">
<h3>Drawing / Pattern Simulation</h3>
<p>A robotic system programmed to execute precise geometric drawing patterns. The challenge was maintaining smooth trajectories across curves and corners without accumulating positional error. I found that speed synchronization and TCP tuning are critical for consistent path accuracy.
</p>  
<p><strong>Tools & Environment:</strong> ABB RobotStudio, ABB Teach Pendant, TCP configuration</p>

<p><strong>Skills:</strong></p>
<div class="project-skills">
  <span class="skill-item skill-abb">ABB RobotStudio</span>
  <span class="skill-item skill-motion">Motion Control</span>
  <span class="skill-item skill-trajectory">Trajectory Planning</span>
 </div>
</div>


#### Nachi Robot Teach Pendant Projects

<div class="project-card robotics-card">
<h3>Pick & Place</h3>
<p>A teach pendant–programmed robot performing pick-and-place and color sorting tasks. The challenge was integrating sensor feedback with motion sequences while maintaining reliable positioning. I learned how structured motion sequencing improves repeatability and reduces errors in automated tasks.
</p>
<p><strong>Tools & Environment:</strong> Nachi Teach Pendant, TCP configuration, Sensor Integration, Motion Control </p>

<p><strong>Skills & Tools:</strong></p>
<div class="project-skills">
  <span class="skill-item skill-nachi">Nachi Teach Pendant</span>
  <span class="skill-item skill-tcp">TCP Configuration</span>
  <span class="skill-item skill-motion">Motion Control</span>
  <span class="skill-item">Sensor Integration</span>
  </div>
</div>

<div class="project-card robotics-card">
<h3>Color Sorting</h3>
<p>A teach pendant–programmed robot that sorts objects based on color by integrating sensor feedback with motion sequences. The challenge was aligning detection with precise positioning so that objects were consistently picked and placed without misalignment. I found that accurate TCP calibration and structured motion sequencing were key to reducing sorting errors and improving repeatability.</p>
<p><strong>Tools & Environment:</strong> Nachi Teach Pendant, TCP configuration, Sensor Integration, Motion Control </p>

<p><strong>Skills & Tools:</strong></p>
<div class="project-skills">
   <span class="skill-item skill-nachi">Nachi Teach Pendant</span>
  <span class="skill-item skill-tcp">TCP Configuration</span>
  <span class="skill-item skill-motion">Motion Control</span>
  <span class="skill-item">Sensor Integration</span>
  </div>
</div>


<div class="project-card robotics-card">
<h3>Drawing / Pattern Making</h3>
<p>A robot programmed to create geometric patterns using teach pendant control and precise trajectory execution. The challenge was maintaining smooth motion across curves and corners without introducing positional errors over repeated cycles. I found that synchronizing speed, orientation, and TCP calibration was essential for achieving consistent and accurate patterns.</p>
<p><strong>Tools & Environment:</strong> Nachi Teach Pendant, TCP configuration</p>

<p><strong>Skills & Tools:</strong></p>
<div class="project-skills">
  <span class="skill-item skill-nachi">Nachi Teach Pendant</span>
  <span class="skill-item skill-tcp">TCP Configuration</span>
  <span class="skill-item skill-motion">Motion Control</span>
  <span class="skill-item skill-trajectory">Trajectory Planning</span>
 </div>
</div>


### 🔹 PLC Projects

<div class="project-card plc-card">
<h3>Water Treatment Plant Backwash Automation</h3>
<p>A PLC-based system that automates pump and valve sequencing for a backwash process with interlocks and fail-safes. The challenge was designing safe and reliable sequences where incorrect timing could damage equipment. I learned that clear state control and interlock design are essential for fault-tolerant industrial systems.</p>  
<p><strong>Tools & Environment:</strong> RSLogix 500 / Studio 5000, Ladder Logic, PLC sensors and actuators</p>

<p><strong>Skills & Tools:</strong></p>
<div class="project-skills">
 <span class="skill-item skill-plc">PLC</span>
  <span class="skill-item skill-allenbradley">Allen Bradley</span>
  <span class="skill-item skill-ladder">Ladder Logic</span>
  <span class="skill-item skill-structuredtext">Structured Text</span>
  <span class="skill-item skill-fbd">Functional Block Diagram (FBD)</span>
 </div>
</div>

<div class="project-card plc-card">
<h3>Automatic Water Filling System</h3>
<p>A 7-stage automated filling system with sensor-based sequencing, timers, and HMI monitoring. The challenge was managing stage transitions without conflicts while maintaining accurate timing and synchronization. I found that properly structured logic with timers, counters, and interlocks is critical for stable and scalable automation.</p>
<p><strong>Tools & Environment:</strong> CODESYS V3, Ladder Logic, CODESYS Visualization (HMI), Software Simulation</p>

<div class="project-media">
  <!-- HMI Video -->
  <p><strong>HMI Simulation Demo:</strong></p>
  <p><em>Demo: Real-time monitoring and control of the 7-stage bottle filling process</em></p>
  <video controls>
    <source src="assets/images/Automatic_Bottle_Filling.mp4" type="video/mp4" />
  </video>
  <br><br>
  <!-- Ladder Logic Screenshots -->
  <p><strong>Ladder Logic Implementation:</strong></p>
  <p><em>Sequential control logic divided into stages</em></p>
  <div class="ladder-gallery">
    <img src="assets/images/Automatic_Water_Filling_1.png" alt="Ladder Logic Stage 1-3">
    <img src="assets/images/Automatic_Water_Filling_2.png" alt="Ladder Logic Stage 4-5">
    <img src="assets/images/Automatic_Water_Filling_3.png" alt="Ladder Logic Stage 6-7">
  </div>
</div>

<p><strong>Skills & Tools:</strong></p>
<div class="project-skills">
  <span class="skill-item skill-plc">PLC</span>
  <span class="skill-item skill-codesys">CODESYS V3</span>
  <span class="skill-item skill-ladder">Ladder Logic</span>
  <span class="skill-item skill-hmi">HMI Development</span>
  <span class="skill-item skill-simulation">Simulation</span>
</div>
</div>

---

<h1 id="skills" class="section-title">🧠 Skills</h1>

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.css" />
<script src="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.js"></script>
<script>
  AOS.init();
</script>

<div class="skills">
  <span class="skill-tag" data-aos="fade-up">ROS2</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="100">Gazebo</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="200">RViz</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="300">Python</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="400">Embedded C</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="500">Arduino</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="600">PLC (Allen Bradley / Delta)</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="700">ABB RobotStudio</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="800">Nachi Teach Pendant</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="900">Fusion 360</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="1000">Electromechanical Troubleshooting</span>
</div>

  

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

