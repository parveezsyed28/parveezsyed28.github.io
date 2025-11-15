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

.project-img {
  width: 100%;
  border-radius: 12px;
  transition: transform 0.3s ease;
}

.project-card:hover .project-img {
  transform: scale(1.03);
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

# <span id="home"></span>👋 **Welcome**

Hi! I'm **Parveez Banu Syed Azizuddin**, a Mechatronics Specialist with hands-on experience building robots, ROS2 simulations, automation systems, embedded controllers, and more.

---

# <span id="ros2-projects"></span>🤖 **ROS2 Projects**

## 🟦 **Wall Follower Bot – ROS2**
<div class="project-card">
  <img class="project-img" src="images/wall_follower.png">
  <p>Custom ROS2 robot with LIDAR-based wall detection.  
  <strong>Tools:</strong> ROS2, Gazebo, RViz, Fusion 360</p>
</div>

## 🟦 **TortoiseBot Navigation**
<div class="project-card">
  <img class="project-img" src="images/tortoisebot_nav.png">
  <p>Navigation stack with Nav2, map saving, SLAM.</p>
</div>

## 🟦 **ROS2 Obstacle Avoidance (Simulation)**
<div class="project-card">
  <img class="project-img" src="images/ros2_obstacle.png">
  <p>LIDAR-based obstacle avoidance simulation.</p>
</div>

---

# <span id="embedded-projects"></span>🔧 **Embedded Projects**

## 🟩 **Obstacle Avoider – Microcontroller Version**
<div class="project-card">
  <img class="project-img" src="images/obstacle_avoider_embedded.png">
  <p>Hardware robot using ultrasonic sensors + motor drivers.</p>
</div>

## 🟩 **Line Follower Robot**
<div class="project-card">
  <img class="project-img" src="images/line_follower.png">
  <p>IR sensor tracking + PID tuning.</p>
</div>

## 🟩 **ADC Controlled Robot**
<div class="project-card">
  <img class="project-img" src="images/adc_robot.png">
  <p>Analog-input motion control using ADC.</p>
</div>

---

# <span id="automation-projects"></span>🏭 **Industrial Automation**

## 🟪 **ABB RobotStudio**
<div class="project-card">
  <img class="project-img" src="images/abb_robotstudio.png">
  <p>Pick & place, trajectory planning, TCP setup.</p>
</div>

## 🟪 **Nachi Robotics – Color Sorting**
<div class="project-card">
  <img class="project-img" src="images/nachi_robot.png">
  <p>Motion sequences + pattern making.</p>
</div>

---

# <span id="skills"></span>🧠 **Skills**

- ROS2, Gazebo, RViz  
- Python for robotics  
- Fusion 360 modeling  
- Embedded C, Arduino  
- PLC basics (AB, Delta)  
- Electromechanical troubleshooting  

---

# <span id="contact"></span>📬 **Contact**

📧 **parveezsyed28@gmail.com**  
🌐 **parveezsyed28.github.io**  
📍 Toronto, Canada  

---
