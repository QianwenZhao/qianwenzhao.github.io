---
layout: single
title: "Academic Projects"
permalink: /academic-projects/
author_profile: true
---

## Vision-based Tactile Fingertip for Grasping

<div style="display: flex; gap: 1rem; align-items: flex-start; flex-wrap: wrap; margin: 1rem 0;">
  <img src="/images/QZ-leap-hand-grasp.png" alt="Robotic hand grasping simulation" style="max-width: 20%; min-width: 200px;">
  <img src="/images/QZ-vision-tactile.png" alt="Vision-based tactile fingertip" style="max-width: 48%; min-width: 200px;">
</div>

**Advanced Robot Manipulators Lab, Stevens Institute of Technology, 2025 - present**

* Developed robotic hand grasping simulations integrated with a vision-based tactile sensor in NVIDIA Isaac Sim.
* Conducted fingertip material characterization and fatigue analysis to support sensor and fingertip design.
* Tools: **NVIDIA Isaac Sim, mechatronics**.

## Consensus-Driven Uncertainty for Robotic Grasping based on RGB Perception

<div style="position: relative; width: 70%; max-width: 600px; aspect-ratio: 16 / 9; margin: 1rem 0;">
  <iframe src="https://www.youtube.com/embed/YZgaBkHnuSc" title="Consensus-driven uncertainty for robotic grasping based on RGB perception" style="position: absolute; inset: 0; width: 100%; height: 100%; border: 0;" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

**Collaborative research with the Department of Computer Science, Stevens Institute of Technology, 2025**

* Developed a robotic grasping framework that estimates whether a grasp will succeed before execution by reasoning about uncertainty in RGB-based 6-DoF object pose estimation.
* Generated training data by combining object pose estimation on real images with simulated grasping trials, connecting perception uncertainty to downstream grasping performance.
* Trained lightweight deep networks across diverse objects to support uncertainty-aware grasp decisions, helping the robot avoid acting when pose estimates are unreliable.
* Tools: **RGB perception, object pose estimation, deep learning, robotic grasping simulation**.

## Underactuated Robotic Hand for Combat Casualty Care

<div style="display: flex; gap: 1rem; align-items: flex-start; flex-wrap: wrap; margin: 1rem 0;">
  <img src="/images/QZ-hand-3d.png" alt="Underactuated robotic hand CAD model" style="max-width: 20%; min-width: 110px;">
  <img src="/images/QZ-robotic-hand-finger-details-short-vertical.png" alt="Robotic hand finger mechanism details" style="max-width: 20%; min-width: 150px;">
  <img src="/images/QZ-scalpel-proposal-figure.png" alt="Robotic hand combat casualty care task concept" style="max-width: 40%; min-width: 220px;">
</div>

**Advanced Robot Manipulators Lab, Stevens Institute of Technology, 2024 - present**

* Led end-to-end development of an underactuated multi-finger robotic hand, including mechanical design, hardware optimization, sensor integration, and motion control.
* Developed and extended physics-based simulation environments in MuJoCo to test functionality, validate new features, and evaluate design changes before manufacturing new hardware revisions.
* Tools: **SolidWorks, Arduino, mechatronics, 3D printing, MuJoCo, FEA**.

## High-Fidelity Simulation for Casualty Manipulation

<div style="display: flex; gap: 1rem; align-items: stretch; flex-wrap: wrap; margin: 1rem 0;">
  <div style="display: flex; flex-direction: column; gap: 1rem; flex: 1 1 200px; max-width: 300px;">
    <img src="/images/QZ-casualty-manipulation.png" alt="Casualty manipulation simulation" style="width: 80%; height: auto;">
    <img src="/images/QZ-CAVEMAN.png" alt="Digital human model for casualty manipulation" style="width: 80%; height: auto;">
  </div>
  <div style="position: relative; flex: 0 1 280px; max-width: 320px; min-width: 220px; aspect-ratio: 1 / 1;">
    <iframe src="https://www.youtube.com/embed/iQlDu4bcJdQ" title="High-fidelity simulation for casualty manipulation" style="position: absolute; inset: 0; width: 100%; height: 100%; border: 0;" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
  </div>
</div>

**Advanced Robot Manipulators Lab, Stevens Institute of Technology, 2022 - 2025**

* Designed and extended a high-fidelity robotics simulation framework for casualty manipulation, integrating ROS-based motion planning, physics-based multi-body dynamics in MuJoCo, and finite element analysis to capture complex contact and deformation behaviors.
* Implemented biomechanically accurate human body models, enabling realistic simulation of nonlinear soft-contact interactions between robots and human casualties.
* Developed and tested telemanipulation behaviors for a mobile robot platform, coordinating base motion, robotic arm motion, and end-effector control within the simulated environment.
* Used simulation environments to support algorithm development, debugging, and performance evaluation before deployment on physical robotic systems.
* Tools: **Python, ROS, MuJoCo, OpenSim, FEA**.

## Integrating 3D Human Pose Reconstruction into a Physics-Based Robotic Casualty Manipulation Framework

<div style="display: flex; gap: 1rem; align-items: flex-start; flex-wrap: wrap; margin: 1rem 0;">
  <img src="/images/QZ-human-pose-reconstruction.png" alt="3D human pose reconstruction for robotic casualty manipulation" style="max-width: 99%; min-width: 280px;">
</div>

**Advanced Robot Manipulators Lab, Stevens Institute of Technology, 2026**

* Developed a vision-to-simulation pipeline that uses multi-view RGB images to estimate human joint locations and reconstruct a 3D casualty pose.
* Applied OpenPose for 2D keypoint detection and Direct Linear Transformation triangulation to recover a simulation-ready 3D skeleton from calibrated camera views.
* Integrated reconstructed human poses into OpenSim and Gazebo, enabling robot motion planning and trajectory testing while monitoring biomechanical safety metrics.
* Tools: **OpenPose, Intel RealSense RGB-D cameras, OpenSim, Gazebo, ROS, human pose reconstruction**.


## Aerial Continuum Manipulator

<div style="display: flex; gap: 1rem; align-items: flex-start; flex-wrap: wrap; margin: 1rem 0;">
  <img src="/images/QZ-aerial-continuum-vision_platforms.png" alt="Aerial continuum manipulator platform" style="max-width: 30%; min-width: 260px;">
  <img src="/images/QZ-aerial-continuum-assembly.png" alt="Aerial continuum manipulator assembly" style="max-width: 30%; min-width: 260px;">
</div>

**Advanced Robot Manipulators Lab, Stevens Institute of Technology, 2022**

* Designed a compact, lightweight, and modular cable-driven continuum manipulator for aerial drones.
* Tools: **SolidWorks, mechatronics, 3D printing, Arduino, ROS**.
