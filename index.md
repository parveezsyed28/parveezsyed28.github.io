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

<h1 id="home" class="section-title">👋 Welcome</h1>

Hi! I'm **Parveez Banu Syed Azizuddin**, a Mechatronics Specialist with hands-on experience building robots, ROS2 simulations, automation systems, embedded controllers, and more.

---

<h1 id="ros2-projects" class="section-title">🤖 ROS2 Projects</h1>

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

<h1 id="embedded-projects" class="section-title">🔧 Embedded Projects</h1>

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

<h1 id="automation-projects" class="section-title">🏭 Industrial Automation</h1>

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

<h1 id="skills" class="section-title">🧠 Skills</h1>

- ROS2, Gazebo, RViz  
- Python for robotics  
- Fusion 360 modeling  
- Embedded C, Arduino  
- PLC basics (AB, Delta)  
- Electromechanical troubleshooting  

---

<h1 id="contact" class="section-title">📬 Contact</h1>

📧 **parveezsyed28@gmail.com**  
🌐 **parveezsyed28.github.io**  
📍 Toronto, Canada  

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

