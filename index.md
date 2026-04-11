---
layout: default
title: "Portfolio – Parveez Banu Syed Azizuddin"
---

<!-- Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=DM+Sans:ital,wght@0,300;0,400;0,500;1,300&family=DM+Mono:wght@400;500&display=swap" rel="stylesheet"/>

<!-- Typed.js -->
<script src="https://cdn.jsdelivr.net/npm/typed.js@2.0.12"></script>

<!-- AOS -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.css" />
<script src="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.js"></script>

<!-- ========================= -->
<!--          HERO             -->
<!-- ========================= -->

<div class="hero">
  <div class="hero-bg"></div>
  <div class="hero-grid"></div>

  <nav class="hero-nav">
    <span class="hero-nav-name">Parveez</span>
    <button class="hamburger" id="hamburger" aria-label="Menu">
      <span></span><span></span><span></span>
    </button>
    <ul class="hero-nav-links" id="navLinks">
      <li><a href="#home">Home</a></li>
      <li><a href="#ros2-projects">ROS2</a></li>
      <li><a href="#embedded-projects">Embedded</a></li>
      <li><a href="#automation-projects">Automation</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <div class="hero-content" id="home">
    <p class="hero-eyebrow">INDUSTRIAL AUTOMATION &amp; CONTROLS</p>
    <h1 class="hero-name">Parveez Banu<br>Syed Azizuddin</h1>
    <p class="hero-typed"><span id="typed-output"></span></p>
    <div class="hero-cta-row">
      <a href="#ros2-projects" class="hero-btn">View Projects</a>
      <a href="#contact" class="hero-btn hero-btn-ghost">Get In Touch</a>
    </div>
  </div>

  <div class="hero-scroll">
    <span>scroll</span>
    <div class="hero-scroll-line"></div>
  </div>
</div>

<!-- ========================= -->
<!--        ALL STYLES         -->
<!-- ========================= -->

<style>

/* ── HIDE JEKYLL THEME HEADER ── */
header, .site-header, #header,
.page-header, .site-title,
.site-nav, nav.site-nav,
.masthead, #masthead,
.header-wrapper {
  display: none !important;
}

/* ── FORCE DARK BACKGROUND EVERYWHERE ── */
html, body,
.site-body, .site-wrapper,
.page-content, .post-content,
.wrapper, .inner, #main,
#main-content, .main-content-wrap,
.container, .content-wrapper {
  background: #0c1117 !important;
  color: #cbd5e1 !important;
}

/* ── RESET ── */
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

:root {
  --bg:       #0c1117;
  --surface:  #131c24;
  --panel:    #1a2530;
  --border:   #1e3040;
  --accent:   #38bdf8;
  --accent2:  #fb923c;
  --ok:       #4ade80;
  --warn:     #fbbf24;
  --text:     #cbd5e1;
  --muted:    #4a6278;
  --white:    #f1f5f9;
  --ros:      #7eb8f7;
  --embedded: #f7c97e;
  --plc:      #7ef7b8;
  --robotics: #f7a7e0;
  --head:     'Bebas Neue', sans-serif;
  --body:     'DM Sans', sans-serif;
  --mono:     'DM Mono', monospace;
}

html { scroll-behavior: smooth; }

body {
  background: var(--bg);
  color: var(--text);
  font-family: var(--body);
  font-weight: 300;
  line-height: 1.7;
}

/* ── HERO ── */
.hero {
  position: relative;
  width: 100%;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  overflow: hidden;
  background: var(--bg);
}

.hero-bg {
  position: absolute; inset: 0;
  background:
    radial-gradient(ellipse 80% 60% at 15% 40%, rgba(56,189,248,0.08) 0%, transparent 60%),
    radial-gradient(ellipse 50% 40% at 85% 70%, rgba(251,146,60,0.05) 0%, transparent 60%),
    linear-gradient(180deg, #0c1117 0%, #0f1923 100%);
  z-index: 0;
}

.hero-grid {
  position: absolute; inset: 0;
  background-image:
    linear-gradient(rgba(56,189,248,0.04) 1px, transparent 1px),
    linear-gradient(90deg, rgba(56,189,248,0.04) 1px, transparent 1px);
  background-size: 48px 48px;
  z-index: 0;
}

@keyframes scan {
  0%   { transform: translateY(-4px); opacity: 0; }
  5%   { opacity: 1; }
  95%  { opacity: 1; }
  100% { transform: translateY(100vh); opacity: 0; }
}
.hero::after {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 2px;
  background: linear-gradient(90deg, transparent, rgba(56,189,248,0.5), transparent);
  animation: scan 7s linear infinite;
  z-index: 1;
  pointer-events: none;
}

/* ── HERO NAV ── */
.hero-nav {
  position: relative;
  z-index: 100;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 28px 48px;
}

.hero-nav-name {
  font-family: var(--head);
  font-size: 22px;
  letter-spacing: 0.1em;
  color: var(--white);
}

.hero-nav-links {
  display: flex;
  list-style: none;
  gap: 24px;
}
.hero-nav-links a {
  font-family: var(--mono);
  font-size: 10px;
  letter-spacing: 0.10em;
  text-transform: uppercase;
  color: var(--muted);
  text-decoration: none;
  transition: color 0.2s;
  white-space: nowrap;
}
.hero-nav-links a:hover { color: var(--accent); }

.hamburger {
  display: none;
  flex-direction: column;
  gap: 5px;
  background: none;
  border: none;
  cursor: pointer;
  padding: 4px;
  z-index: 200;
}
.hamburger span {
  display: block;
  width: 26px;
  height: 2px;
  background: var(--white);
  transition: all 0.3s ease;
}
.hamburger.open span:nth-child(1) { transform: translateY(7px) rotate(45deg); }
.hamburger.open span:nth-child(2) { opacity: 0; }
.hamburger.open span:nth-child(3) { transform: translateY(-7px) rotate(-45deg); }

/* ── HERO CONTENT ── */
.hero-content {
  position: relative;
  z-index: 10;
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 40px 48px 100px;
  max-width: 960px;
}

@keyframes fadeUp {
  from { opacity: 0; transform: translateY(24px); }
  to   { opacity: 1; transform: translateY(0); }
}

.hero-eyebrow {
  font-family: var(--mono);
  font-size: 11px;
  letter-spacing: 0.22em;
  color: var(--accent);
  margin-bottom: 20px;
  opacity: 0;
  animation: fadeUp 0.7s 0.2s forwards;
}

.hero-name {
  font-family: var(--head);
  font-size: clamp(52px, 11vw, 110px);
  line-height: 0.95;
  letter-spacing: 0.02em;
  color: var(--white);
  margin-bottom: 32px;
  opacity: 0;
  animation: fadeUp 0.7s 0.4s forwards;
}

.hero-typed {
  font-family: var(--mono);
  font-size: clamp(14px, 2.2vw, 20px);
  color: var(--accent2);
  letter-spacing: 0.06em;
  min-height: 30px;
  margin-bottom: 44px;
  opacity: 0;
  animation: fadeUp 0.7s 0.6s forwards;
}

.hero-cta-row {
  display: flex;
  gap: 16px;
  flex-wrap: wrap;
  opacity: 0;
  animation: fadeUp 0.7s 0.8s forwards;
}

.hero-btn {
  font-family: var(--mono);
  font-size: 11px;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  text-decoration: none;
  padding: 14px 36px;
  background: var(--accent);
  color: var(--bg);
  font-weight: 500;
  transition: background 0.2s, transform 0.2s;
  border: 1px solid var(--accent);
}
.hero-btn:hover { background: #7dd3fc; transform: translateY(-2px); }

.hero-btn-ghost {
  background: transparent;
  color: var(--accent);
}
.hero-btn-ghost:hover { background: rgba(56,189,248,0.08); transform: translateY(-2px); }

/* Scroll indicator */
.hero-scroll {
  position: absolute;
  bottom: 36px; right: 48px;
  display: flex;
  align-items: center;
  gap: 12px;
  z-index: 10;
  opacity: 0;
  animation: fadeUp 0.7s 1.2s forwards;
}
.hero-scroll span {
  font-family: var(--mono);
  font-size: 9px;
  letter-spacing: 0.22em;
  text-transform: uppercase;
  color: var(--muted);
}
@keyframes scrollPulse {
  0%,100% { transform: scaleY(1); opacity: 0.4; }
  50%      { transform: scaleY(1.5); opacity: 1; }
}
.hero-scroll-line {
  width: 1px; height: 44px;
  background: var(--accent);
  transform-origin: top;
  animation: scrollPulse 2s ease-in-out infinite;
}

/* ── WELCOME BIO ── */
.bio-block {
  max-width: 960px;
  margin: 0 auto;
  padding: 64px 48px 0;
}
.bio-block p {
  font-size: 16px;
  color: var(--text);
  line-height: 1.8;
  max-width: 720px;
}
.bio-block strong { color: var(--white); }

/* ── MAIN CONTENT ── */
.main-content {
  max-width: 960px;
  margin: 0 auto;
  padding: 0 48px 80px;
}

/* ── SECTION TITLES ── */
.section-title {
  font-family: var(--head);
  font-size: clamp(28px, 5vw, 48px);
  letter-spacing: 0.04em;
  color: var(--white);
  margin-top: 72px;
  margin-bottom: 28px;
  padding: 14px 20px;
  background: rgba(56,189,248,0.04);
  border-left: 4px solid var(--accent);
  opacity: 0;
  animation: fadeUp 0.7s forwards;
}

/* ── PROJECT CARDS ── */
.project-card {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: 0;
  padding: 28px;
  margin-bottom: 20px;
  transition: transform 0.3s ease, box-shadow 0.3s ease, border-color 0.3s;
  opacity: 0;
  animation: fadeIn 0.6s forwards;
}
.project-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 16px 40px rgba(0,0,0,0.5);
  border-color: var(--muted);
}
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(15px); }
  to   { opacity: 1; transform: translateY(0); }
}

.ros-card      { border-top: 4px solid var(--ros); }
.embedded-card { border-top: 4px solid var(--embedded); }
.plc-card      { border-top: 4px solid var(--plc); }
.robotics-card { border-top: 4px solid var(--robotics); }

.project-card h3 {
  font-family: var(--head);
  font-size: 26px;
  letter-spacing: 0.04em;
  color: var(--white);
  margin-bottom: 14px;
}

.project-card h2 {
  font-family: var(--head);
  font-size: 20px;
  letter-spacing: 0.06em;
  color: var(--muted);
  margin: 32px 0 16px;
  text-transform: uppercase;
}

.project-card p {
  font-size: 14px;
  color: var(--text);
  line-height: 1.75;
  margin-bottom: 14px;
}

.project-card strong { color: var(--white); }

/* ── MEDIA ── */
.project-img, .project-media video {
  width: 100%;
  max-width: 680px;
  height: 320px;
  object-fit: cover;
  border: 1px solid var(--border);
  transition: transform 0.3s ease;
}
.project-media { margin-top: 20px; }
.project-card:hover .project-img,
.project-card:hover .project-media video { transform: scale(1.01); }

.media.side-by-side {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 16px;
}
.media.side-by-side img,
.project-media.side-by-side img {
  flex: 1 1 calc(50% - 6px);
  max-width: 100%;
  height: 220px;
  object-fit: cover;
  border: 1px solid var(--border);
}

.ladder-gallery {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 12px;
}
.ladder-gallery img {
  width: 100%;
  max-width: 900px;
  object-fit: cover;
  border: 1px solid var(--border);
}

/* ── SKILL TAGS ── */
.project-skills {
  margin-top: 14px;
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.skill-item {
  display: inline-block;
  padding: 4px 12px;
  font-family: var(--mono);
  font-size: 11px;
  letter-spacing: 0.06em;
  border: 1px solid var(--border);
  color: var(--text);
  background: var(--panel);
  transition: border-color 0.2s, color 0.2s;
}
.skill-item:hover { border-color: var(--accent); color: var(--accent); }

.skill-ros        { border-color: #2a4f72; color: var(--ros); background: rgba(126,184,247,0.06); }
.skill-gazebo     { border-color: #3a2f72; color: #c4b5fd; background: rgba(196,181,253,0.06); }
.skill-rviz       { border-color: #1a3f60; color: #93c5fd; background: rgba(147,197,253,0.06); }
.skill-urdf       { border-color: var(--border); }
.skill-turtlesim  { border-color: #1a4a2a; color: #86efac; background: rgba(134,239,172,0.06); }
.skill-python     { border-color: #4a3a1a; color: var(--embedded); background: rgba(247,201,126,0.06); }
.skill-cad        { border-color: #1a4a2a; color: #6ee7b7; background: rgba(110,231,183,0.06); }
.skill-fusion360  { border-color: #1a3a2a; color: #6ee7b7; background: rgba(110,231,183,0.06); }
.skill-stl        { border-color: var(--border); }
.skill-embedded   { border-color: #4a3a1a; color: var(--embedded); background: rgba(247,201,126,0.06); }
.skill-atmega16   { border-color: #4a3010; color: #fdba74; background: rgba(253,186,116,0.06); }
.skill-ir         { border-color: #4a3a10; color: #fcd34d; background: rgba(252,211,77,0.06); }
.skill-l293d      { border-color: #4a2a10; color: #fed7aa; background: rgba(254,215,170,0.06); }
.skill-pwm        { border-color: #4a3010; color: #fde68a; background: rgba(253,230,138,0.06); }
.skill-adc        { border-color: #4a3a10; color: #fef3c7; background: rgba(254,243,199,0.06); }
.skill-hardware   { border-color: var(--border); }
.skill-555        { border-color: #4a1a2a; color: #fda4af; background: rgba(253,164,175,0.06); }
.skill-7805       { border-color: #4a1a30; color: #fbcfe8; background: rgba(251,207,232,0.06); }
.skill-voltreg    { border-color: var(--border); }
.skill-plc        { border-color: #1a4a40; color: var(--plc); background: rgba(126,247,184,0.06); }
.skill-allenbradley{ border-color: #1a4040; color: #67e8f9; background: rgba(103,232,249,0.06); }
.skill-delta      { border-color: #1a3a38; color: #5eead4; background: rgba(94,234,212,0.06); }
.skill-rslogix    { border-color: #1a4040; color: #a5f3fc; background: rgba(165,243,252,0.06); }
.skill-studio5000 { border-color: #1a4040; color: #cffafe; background: rgba(207,250,254,0.06); }
.skill-ladder     { border-color: #2a4010; color: #d9f99d; background: rgba(217,249,157,0.06); }
.skill-structuredtext{ border-color: #3a4010; color: #fef9c3; background: rgba(254,249,195,0.06); }
.skill-fbd        { border-color: #1a3a4a; color: #bae6fd; background: rgba(186,230,253,0.06); }
.skill-abb        { border-color: #1a2a4a; color: #93c5fd; background: rgba(147,197,253,0.06); }
.skill-nachi      { border-color: #101a3a; color: #bfdbfe; background: rgba(191,219,254,0.06); }
.skill-tcp        { border-color: #1a4a2a; color: #bbf7d0; background: rgba(187,247,208,0.06); }
.skill-motion     { border-color: #2a4a1a; color: #d9f99d; background: rgba(217,249,157,0.06); }
.skill-trajectory { border-color: #3a4a1a; color: #ecfccb; background: rgba(236,252,203,0.06); }
.skill-linux      { border-color: var(--border); color: var(--text); }
.skill-git        { border-color: var(--border); color: var(--text); }
.skill-vscode     { border-color: #1a2050; color: #c7d2fe; background: rgba(199,210,254,0.06); }
.skill-codesys    { border-color: #1a4040; color: #67e8f9; background: rgba(103,232,249,0.06); }
.skill-hmi        { border-color: #2a4a1a; color: #d9f99d; background: rgba(217,249,157,0.06); }
.skill-simulation { border-color: #3a1a4a; color: #e9d5ff; background: rgba(233,213,255,0.06); }
.skill-lidar      { border-color: #1a3f60; color: #93c5fd; background: rgba(147,197,253,0.06); }

/* ── GITHUB LINK ── */
a.github-link {
  display: inline-block;
  margin-top: 16px;
  font-family: var(--mono);
  font-size: 11px;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--accent);
  text-decoration: none;
  border: 1px solid var(--accent);
  padding: 9px 22px;
  transition: background 0.2s, color 0.2s;
}
a.github-link:hover { background: var(--accent); color: var(--bg); }

/* ── SKILLS SECTION ── */
.skills {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 16px;
}
.skill-tag {
  display: inline-block;
  background: var(--panel);
  color: var(--text);
  border: 1px solid var(--border);
  padding: 8px 18px;
  font-family: var(--mono);
  font-size: 12px;
  letter-spacing: 0.06em;
  transition: border-color 0.2s, color 0.2s, transform 0.2s;
  cursor: default;
}
.skill-tag:hover {
  border-color: var(--accent);
  color: var(--accent);
  transform: translateY(-2px);
}

/* ── CONTACT ── */
.contact-info p { font-size: 14px; margin-bottom: 10px; }
.contact-info a { color: var(--accent); text-decoration: none; }
.contact-info a:hover { text-decoration: underline; }

/* ── BACK TO TOP ── */
#topBtn {
  position: fixed;
  bottom: 32px; right: 32px;
  z-index: 9999;
  background: var(--accent);
  color: var(--bg);
  border: none;
  width: 44px; height: 44px;
  font-size: 18px;
  font-weight: bold;
  cursor: pointer;
  opacity: 0;
  pointer-events: none;
  transition: opacity 0.3s, transform 0.2s;
}
#topBtn:hover { transform: scale(1.1); }

/* ── DIVIDERS ── */
hr { border: none; border-top: 1px solid var(--border); margin: 40px 0; }

/* ── MOBILE ── */
@media (max-width: 768px) {
  .hero-nav { padding: 20px 24px; }
  .hero-content { padding: 32px 24px 80px; }
  .bio-block { padding: 48px 24px 0; }
  .main-content { padding: 0 20px 60px; }

  .hero-nav-links {
    display: none;
    position: fixed;
    inset: 0;
    background: rgba(12,17,23,0.97);
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 44px;
    z-index: 150;
  }
  .hero-nav-links.open { display: flex; }
  .hero-nav-links a { font-size: 15px; letter-spacing: 0.18em; color: var(--white); }
  .hamburger { display: flex; }

  .hero-name { font-size: clamp(44px, 13vw, 72px); }
  .hero-scroll { display: none; }

  .project-img, .project-media video { height: 200px; }
  .media.side-by-side img,
  .project-media.side-by-side img { flex: 1 1 100%; height: auto; }

  .section-title { font-size: 26px; padding: 12px 16px; }
}

</style>

<!-- ========================= -->
<!--        BIO / WELCOME      -->
<!-- ========================= -->

<div class="bio-block" id="home-bio">
  <p>Hi! I'm <strong>Parveez Banu Syed Azizuddin</strong>. Welcome to my portfolio — a collection of projects I've been working on while exploring industrial automation and control systems. With a background in Electrical and Electronics Engineering and experience as a Mechatronics Engineer, I've been drawn to how systems behave in real-world conditions — especially how sensors, control logic, and timing come together to make something work reliably. I've been building projects across PLCs, embedded systems, and ROS 2, trying to understand not just how to make things work, but how to make them stable and predictable.</p>
</div>

<!-- ========================= -->
<!--        PROJECTS           -->
<!-- ========================= -->

<div class="main-content">

<h1 id="ros2-projects" class="section-title">ROS 2 Projects</h1>

<div class="project-card ros-card">
  <h3>Wall Following Robot</h3>
  <p>A mobile robot that uses LiDAR data to maintain a consistent distance from walls while navigating corridors and turns without human input. The challenge was handling unstable readings at corners and openings, where simple control logic caused oscillations and drift. I found that stabilizing distance control and prioritizing side-wall feedback produced significantly smoother and more reliable motion.</p>
  <p><strong>Tools:</strong> ROS 2 Humble · Python · Gazebo Classic · URDF/Xacro · Fusion 360</p>
  <div class="project-skills">
    <span class="skill-item skill-ros">ROS 2</span>
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

<div class="project-card ros-card">
  <h3>Obstacle Avoidance Robot</h3>
  <p>A differential-drive robot that detects and avoids obstacles in real time using LiDAR data in a simulated environment. Noisy sensor input translated into abrupt stops and erratic behavior with naive control logic — filtering scan data and tuning control loop timing had a greater impact on stability than the avoidance algorithm itself.</p>
  <p><strong>Tools:</strong> ROS 2 Humble · Python · Gazebo Classic · URDF/Xacro · Ubuntu</p>
  <div class="project-skills">
    <span class="skill-item skill-ros">ROS 2 Humble</span>
    <span class="skill-item skill-python">Python</span>
    <span class="skill-item skill-gazebo">Gazebo Classic</span>
    <span class="skill-item skill-urdf">URDF/Xacro</span>
    <span class="skill-item skill-lidar">LiDAR</span>
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

<div class="project-card ros-card">
  <h3>Robot Description & Simulation</h3>
  <p>A custom-designed two-wheeled robot modeled in Fusion360 and simulated in Gazebo using URDF/Xacro with integrated plugins. Aligning mechanical design, URDF structure, and simulation parameters so the robot behaved realistically was the core challenge — correct plugin configuration and consistent frame definitions turned out to be critical for stable motion.</p>
  <p><strong>Tools:</strong> ROS 2 Humble · Gazebo Classic · URDF/Xacro · Fusion 360 · STL Meshes</p>
  <div class="project-skills">
    <span class="skill-item skill-ros">ROS 2 Humble</span>
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

<div class="project-card ros-card">
  <h3>Turtlesim Shape Drawer</h3>
  <p>A ROS 2 Python node that controls a simulated robot to draw geometric shapes based on user input. Coordinating service calls and velocity commands without timing conflicts was the tricky part — synchronization between communication patterns directly affects motion accuracy, even in a simple system like this.</p>
  <p><strong>Tools:</strong> ROS 2 Humble · Python · Turtlesim · Publishers/Subscribers · Services</p>
  <div class="project-skills">
    <span class="skill-item skill-ros">ROS 2 Humble</span>
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

<h1 id="embedded-projects" class="section-title">Embedded Projects</h1>

<div class="project-card embedded-card">
  <h3>ADC-Based Multi-Behaviour Robot</h3>
  <p>A microcontroller-based robot that combines obstacle avoidance, edge detection, and line following with dynamic speed control using ADC input. Balancing multiple sensor inputs and control behaviors on limited hardware without causing conflicts was the core challenge — prioritizing behaviors and tuning response timing was what made consistent performance possible.</p>
  <p><strong>Tools:</strong> Embedded C · ATmega16 · IR Sensors · ADC · PWM · L293D</p>
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

<div class="project-card embedded-card">
  <h3>Obstacle Avoider Robot</h3>
  <p>A real-time obstacle-avoiding robot built on a microcontroller using IR sensors and direct motor control. Reliable sensor detection under varying lighting conditions was the main challenge — simple, well-timed control logic turned out to be more effective than complex decision-making on constrained hardware.</p>
  <p><strong>Tools:</strong> Embedded C · ATmega16 · IR Sensors · L293D · PCB Design</p>
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
  <div class="media side-by-side">
    <img src="assets/images/obstacle_avoider.png" alt="Obstacle Avoider Robot" />
    <img src="assets/images/Obstacle_avoider_connection.png" alt="Obstacle Avoider Circuit" />
  </div>
  <a class="github-link" href="https://github.com/parveezsyed28/obstacle_avoider_robot" target="_blank">GitHub</a>
</div>

<div class="project-card embedded-card">
  <h3>Table Top Edge Detection Robot</h3>
  <p>A robot that detects table edges and prevents falls by continuously monitoring IR sensor feedback. Achieving fast and reliable detection without false triggers was the challenge — tuning sensor thresholds and response timing was critical for stable and safe operation.</p>
  <p><strong>Tools:</strong> Embedded C · ATmega16 · IR Sensors · Real-time Control</p>
  <div class="project-skills">
    <span class="skill-item skill-embedded">Embedded C</span>
    <span class="skill-item skill-atmega16">ATmega16</span>
    <span class="skill-item skill-ir">IR Sensors</span>
    <span class="skill-item">Real-time Embedded Control</span>
  </div>
  <div class="project-media">
    <img class="project-img" src="assets/images/table_top.png" alt="Table Top Robot" />
  </div>
  <a class="github-link" href="https://github.com/parveezsyed28/table_top_robot" target="_blank">GitHub</a>
</div>

<div class="project-card embedded-card">
  <h3>Line Follower Robot</h3>
  <p>A robot that follows a path using IR sensors to continuously correct its trajectory. Maintaining stability through turns and recovering quickly from deviations without overshooting was the main challenge — balancing correction speed and control response is what makes smooth, accurate tracking possible.</p>
  <p><strong>Tools:</strong> Embedded C · ATmega16 · IR Sensors · L293D Motor Driver</p>
  <div class="project-skills">
    <span class="skill-item skill-embedded">Embedded C</span>
    <span class="skill-item skill-atmega16">ATmega16</span>
    <span class="skill-item skill-ir">IR Sensors</span>
    <span class="skill-item skill-l293d">L293D Motor Driver</span>
  </div>
  <div class="media side-by-side">
    <img src="assets/images/line_follower.png" alt="Line Follower Robot" />
    <img src="assets/images/line_follower_connection.png" alt="Line Follower Circuit" />
  </div>
  <a class="github-link" href="https://github.com/parveezsyed28/line_follower_robot" target="_blank">GitHub</a>
</div>

---

<h1 id="automation-projects" class="section-title">Industrial Automation</h1>

<h2 style="font-family:'Bebas Neue',sans-serif;font-size:22px;letter-spacing:0.1em;color:var(--muted);margin:32px 0 16px;text-transform:uppercase;">ABB RobotStudio Projects</h2>

<div class="project-card robotics-card">
  <h3>Pick & Place / Sorting Simulation</h3>
  <p>An industrial robot simulation that performs pick-and-place and sorting operations with precise motion control. Ensuring accurate positioning across varying object conditions while avoiding collisions was the challenge — TCP configuration directly determines repeatability and motion precision in ways that aren't obvious until things go wrong.</p>
  <p><strong>Tools:</strong> ABB RobotStudio · Teach Pendant · TCP Configuration</p>
  <div class="project-skills">
    <span class="skill-item skill-abb">ABB RobotStudio</span>
    <span class="skill-item skill-tcp">TCP Configuration</span>
    <span class="skill-item skill-motion">Motion Control</span>
  </div>
</div>

<div class="project-card robotics-card">
  <h3>Drawing / Pattern Simulation</h3>
  <p>A robotic system programmed to execute precise geometric drawing patterns. Maintaining smooth trajectories across curves and corners without accumulating positional error was the hard part — speed synchronization and TCP tuning are what make consistent path accuracy possible.</p>
  <p><strong>Tools:</strong> ABB RobotStudio · Teach Pendant · TCP Configuration · Trajectory Planning</p>
  <div class="project-skills">
    <span class="skill-item skill-abb">ABB RobotStudio</span>
    <span class="skill-item skill-motion">Motion Control</span>
    <span class="skill-item skill-trajectory">Trajectory Planning</span>
  </div>
</div>

<h2 style="font-family:'Bebas Neue',sans-serif;font-size:22px;letter-spacing:0.1em;color:var(--muted);margin:32px 0 16px;text-transform:uppercase;">Nachi Robot Projects</h2>

<div class="project-card robotics-card">
  <h3>Pick & Place</h3>
  <p>A teach pendant–programmed robot performing pick-and-place tasks. Integrating sensor feedback with motion sequences while maintaining reliable positioning was the challenge — structured motion sequencing is what improves repeatability and reduces errors in automated tasks.</p>
  <p><strong>Tools:</strong> Nachi Teach Pendant · TCP Configuration · Sensor Integration</p>
  <div class="project-skills">
    <span class="skill-item skill-nachi">Nachi Teach Pendant</span>
    <span class="skill-item skill-tcp">TCP Configuration</span>
    <span class="skill-item skill-motion">Motion Control</span>
    <span class="skill-item">Sensor Integration</span>
  </div>
</div>

<div class="project-card robotics-card">
  <h3>Color Sorting</h3>
  <p>A robot that sorts objects based on color by integrating sensor feedback with motion sequences. Aligning detection with precise positioning so objects are consistently placed without misalignment required accurate TCP calibration — small errors in calibration compound quickly across repeated cycles.</p>
  <p><strong>Tools:</strong> Nachi Teach Pendant · TCP Configuration · Sensor Integration</p>
  <div class="project-skills">
    <span class="skill-item skill-nachi">Nachi Teach Pendant</span>
    <span class="skill-item skill-tcp">TCP Configuration</span>
    <span class="skill-item skill-motion">Motion Control</span>
    <span class="skill-item">Sensor Integration</span>
  </div>
</div>

<div class="project-card robotics-card">
  <h3>Drawing / Pattern Making</h3>
  <p>A robot programmed to create geometric patterns using teach pendant control and precise trajectory execution. Maintaining smooth motion across curves without positional errors over repeated cycles required synchronizing speed, orientation, and TCP calibration — all three have to be right for consistent output.</p>
  <p><strong>Tools:</strong> Nachi Teach Pendant · TCP Configuration · Trajectory Planning</p>
  <div class="project-skills">
    <span class="skill-item skill-nachi">Nachi Teach Pendant</span>
    <span class="skill-item skill-tcp">TCP Configuration</span>
    <span class="skill-item skill-motion">Motion Control</span>
    <span class="skill-item skill-trajectory">Trajectory Planning</span>
  </div>
</div>

<h2 style="font-family:'Bebas Neue',sans-serif;font-size:22px;letter-spacing:0.1em;color:var(--muted);margin:32px 0 16px;text-transform:uppercase;">PLC Projects</h2>

<div class="project-card plc-card">
  <h3>Water Treatment Plant Backwash Automation</h3>
  <p>A PLC-based system that automates pump and valve sequencing for a backwash process with interlocks and fail-safes. Designing safe and reliable sequences where incorrect timing could damage equipment was the core challenge — clear state control and interlock design are what make fault-tolerant industrial systems possible.</p>
  <p><strong>Tools:</strong> Allen Bradley PLC · RSLogix 500 / Studio 5000 · Ladder Logic · Structured Text</p>
  <div class="project-skills">
    <span class="skill-item skill-plc">PLC</span>
    <span class="skill-item skill-allenbradley">Allen Bradley</span>
    <span class="skill-item skill-ladder">Ladder Logic</span>
    <span class="skill-item skill-structuredtext">Structured Text</span>
    <span class="skill-item skill-fbd">FBD</span>
  </div>
</div>

<div class="project-card plc-card">
  <h3>Automatic Water Filling System</h3>
  <p>A 7-stage automated filling system with sensor-based sequencing, timers, and HMI monitoring built in CODESYS. Managing stage transitions without conflicts while maintaining accurate timing was the challenge — properly structured logic with timers, counters, and interlocks is critical for stable and scalable automation.</p>
  <p><strong>Tools:</strong> CODESYS V3 · Ladder Logic · CODESYS Visualization (HMI) · Software Simulation</p>
  <div class="project-media">
    <p><strong>HMI Simulation Demo</strong></p>
    <video controls>
      <source src="assets/images/Automatic_Bottle_Filling.mp4" type="video/mp4" />
    </video>
    <br><br>
    <p><strong>Ladder Logic Implementation</strong></p>
    <div class="ladder-gallery">
      <img src="assets/images/Automatic_Water_Filling_1.png" alt="Ladder Logic Stage 1-3">
      <img src="assets/images/Automatic_Water_Filling_2.png" alt="Ladder Logic Stage 4-5">
      <img src="assets/images/Automatic_Water_Filling_3.png" alt="Ladder Logic Stage 6-7">
    </div>
  </div>
  <div class="project-skills">
    <span class="skill-item skill-plc">PLC</span>
    <span class="skill-item skill-codesys">CODESYS V3</span>
    <span class="skill-item skill-ladder">Ladder Logic</span>
    <span class="skill-item skill-hmi">HMI Development</span>
    <span class="skill-item skill-simulation">Simulation</span>
  </div>
</div>

---

<h1 id="skills" class="section-title">Skills</h1>

<div class="skills">
  <span class="skill-tag" data-aos="fade-up">ROS 2</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="50">Gazebo</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="100">RViz</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="150">Python</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="200">Embedded C</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="250">Arduino</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="300">PLC — Allen Bradley / Delta</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="350">CODESYS V3</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="400">Ladder Logic</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="450">HMI Development</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="500">ABB RobotStudio</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="550">Nachi Teach Pendant</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="600">Fusion 360</span>
  <span class="skill-tag" data-aos="fade-up" data-aos-delay="650">Electromechanical Troubleshooting</span>
</div>

---

<h1 id="contact" class="section-title">Contact</h1>

<div class="contact-info">
  <p>📧 <a href="mailto:parveezbanu.s@gmail.com">parveezbanu.s@gmail.com</a></p>
  <p>🔗 <a href="https://github.com/parveezsyed28" target="_blank">GitHub</a></p>
  <p>💼 <a href="https://linkedin.com/in/parveez-banu2807" target="_blank">LinkedIn</a></p>
  <p>📍 Toronto, Canada</p>
</div>

</div><!-- end .main-content -->

<!-- ========================= -->
<!--     BACK TO TOP           -->
<!-- ========================= -->

<button id="topBtn" title="Go to top">▲</button>

<!-- ========================= -->
<!--        SCRIPTS            -->
<!-- ========================= -->

<script>
document.addEventListener('DOMContentLoaded', function () {

  // Typed.js
  new Typed('#typed-output', {
    strings: [
      'PLC Programmer',
      'Automation Engineer',
      'Embedded Systems',
      'ROS 2 Developer',
      'Controls Engineer'
    ],
    typeSpeed: 50,
    backSpeed: 28,
    backDelay: 1800,
    loop: true,
    cursorChar: '|'
  });

  // AOS
  AOS.init({ once: true, duration: 600 });

  // Hamburger
  const btn = document.getElementById('hamburger');
  const nav = document.getElementById('navLinks');
  if (btn && nav) {
    btn.addEventListener('click', function () {
      btn.classList.toggle('open');
      nav.classList.toggle('open');
    });
    nav.querySelectorAll('a').forEach(function(link) {
      link.addEventListener('click', function() {
        btn.classList.remove('open');
        nav.classList.remove('open');
      });
    });
  }

  // Back to top
  window.onscroll = function () {
    const b = document.getElementById('topBtn');
    if (!b) return;
    if (document.documentElement.scrollTop > 200) {
      b.style.opacity = '1';
      b.style.pointerEvents = 'auto';
    } else {
      b.style.opacity = '0';
      b.style.pointerEvents = 'none';
    }
  };
  const topBtn = document.getElementById('topBtn');
  if (topBtn) topBtn.onclick = function () {
    window.scrollTo({ top: 0, behavior: 'smooth' });
  };

});
</script>
