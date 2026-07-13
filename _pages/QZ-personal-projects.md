---
layout: single
title: "Personal Projects"
permalink: /personal-projects/
author_profile: true
---

## Soft-Body Robotic Grasping Simulation with Franka FR3 and Custom Hand in Newton Physics

<div style="position: relative; width: 70%; max-width: 600px; aspect-ratio: 16 / 9; margin: 1rem 0;">
  <iframe src="https://www.youtube.com/embed/Rnt0spb0aDg" title="Soft-body robotic grasping simulation with Franka FR3 and custom hand in Newton Physics" style="position: absolute; inset: 0; width: 100%; height: 100%; border: 0;" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

This project builds a Newton Physics simulation for deformable-object grasping using a Franka FR3 arm and a custom multi-finger hand. I integrated custom MJCF hand assets with a Franka URDF model, added convex-hull collision geometry, and set up IK-driven control for coordinated arm-hand motion.

The simulation uses VBD soft-body dynamics to model a deformable rubber duck during grasping and lifting. This setup provides a testbed for studying contact-rich manipulation with custom robotic hands, deformable objects, and physics-based grasp execution before moving toward hardware experiments.

Tools: **Newton Physics, Franka FR3, custom hand, MJCF, URDF, IK control, VBD soft-body simulation, deformable-object grasping**.

## Vision-Language-Action Fine-Tuning Pipeline for Franka Pick-and-Place

<div style="display: flex; gap: 1rem; align-items: flex-start; flex-wrap: wrap; margin: 1rem 0;">
  <img src="/images/QZ-VLA-franka-pick-place.gif" alt="Franka Panda pick-and-place rollout for Vision-Language-Action policy fine-tuning" style="max-width: 55%; min-width: 260px; height: auto;">
</div>

This project builds an end-to-end simulation-to-training pipeline for fine-tuning a Vision-Language-Action policy on a Franka Panda cube pick-and-place task. I created a custom Isaac Lab environment with IK-relative Franka control, a target bin, a table-mounted RealSense-style RGB camera, and task success metrics for evaluating closed-loop policy behavior.

To generate training data, I built a scripted expert policy for demonstration collection and added domain randomization across object poses, lighting, camera perturbations, physics parameters, and action latency. The collected demonstrations include synchronized camera images, robot state, actions, language instructions, and success labels. I then converted the data into the LeRobot dataset format, trained baseline behavior-cloning models, fine-tuned SmolVLA, and evaluated the learned policies through closed-loop Isaac Lab rollouts.

Tools: **Isaac Lab, Franka Panda, Vision-Language-Action policies, LeRobot, SmolVLA, behavior cloning, domain randomization, Python**.

## Reinforcement Learning for Unitree Go2 Locomotion in Isaac Lab

<div style="display: flex; gap: 1rem; align-items: flex-start; flex-wrap: wrap; margin: 1rem 0;">
  <img src="/images/QZ_RL_go2_model_100.gif" alt="Unitree Go2 reinforcement learning policy after 100 training iterations" style="width: calc(50% - 0.5rem); min-width: 260px; height: auto;">
  <img src="/images/QZ_RL_go2_model_499.gif" alt="Unitree Go2 reinforcement learning policy after 500 training iterations" style="width: calc(50% - 0.5rem); min-width: 260px; height: auto;">
</div>

This project is my first hands-on experiment with reinforcement learning. To learn by doing, I tried to reproduce part of the method from an ICRA 2025 paper on adaptive energy regularization for quadruped locomotion. The goal is to train a Unitree Go2 robot in Isaac Lab to follow randomized velocity commands. Since I only had access to my laptop GPU, I trained the policy for 500 iterations, but the results were already encouraging. In the video on the left, after 100 iterations, the robot barely moves. In the video on the right, after 500 iterations, the robot can smoothly follow the randomized velocity commands.

Tools: **Isaac Lab, reinforcement learning, Unitree Go2, quadruped locomotion, Python**.

## Isaac Sim - xArm7 + LEAP Hand Contact-Aware Grasping Simulation

<div style="position: relative; width: 70%; max-width: 600px; aspect-ratio: 16 / 9; margin: 1rem 0;">
  <iframe src="https://www.youtube.com/embed/wdCbSE-yMbc" title="xARM7 and LEAP Hand grasping simulation in Isaac Sim" style="position: absolute; inset: 0; width: 100%; height: 100%; border: 0;" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

This project explores robotic grasping and manipulation in NVIDIA Isaac Sim using an xARM7 robot arm integrated with a LEAP Hand. I built the simulation environment to test coordinated arm and hand motion, object interaction, and grasp execution before moving toward physical hardware. The setup provides a useful platform for experimenting with dexterous manipulation strategies, tuning motion sequences, and visualizing contact-rich robotic tasks in a high-fidelity physics simulator.

Tools: **NVIDIA Isaac Sim, xARM7, LEAP Hand, Python, robotics simulation**.

## OpenPose-to-SMPL Human Body Reconstruction

<div style="display: flex; gap: 1rem; align-items: flex-start; flex-wrap: wrap; margin: 1rem 0;">
  <img src="/images/QZ-openpose-SMPL.png" alt="OpenPose keypoints and fitted SMPL human body model" style="width: calc(50% - 0.5rem); min-width: 260px; height: auto;">
  <img src="/images/QZ-openpose-SMPL.gif" alt="Animated 3D SMPL human motion reconstruction" style="width: calc(50% - 0.5rem); min-width: 260px; height: auto;">
</div>

I built a pipeline that applies OpenPose to an image sequence to estimate 2D human body keypoints, then fits a male SMPL parametric body model across 20 frames. The optimization estimates body pose, shape, global orientation, and camera parameters before reconstructing the fitted 3D meshes and skeletons. I exported the resulting motion sequence as an interactive Wis3D visualization for frame-by-frame inspection.

Tools: **Python, OpenPose, SMPL, 3D human body reconstruction, Wis3D**.

## Computer Vision - Teaching YOLO to Recognize My Dog


<div style="display: flex; gap: 1rem; align-items: flex-start; flex-wrap: wrap; margin: 1rem 0;">
  <img src="/images/QZ-yolo11.png" alt="Robotic hand grasping simulation" style="max-width: 40%; min-width: 200px;">
  <img src="/images/QZ-yolo11-dodo.png" alt="Vision-based tactile fingertip" style="max-width: 40%; min-width: 200px;">
</div>

**WHY?**

I’ve been playing with YOLO11 and wanted to try something that felt a bit more personal than just “detect cats and dogs from a stock dataset.” My dog is basically part of the family, so the idea of teaching an AI to recognize my dog specifically (and not just any random dog) sounded both fun and slightly ridiculous in the best way. It’s also a great excuse to walk through the whole deep-learning pipeline—collecting data, training a model, and actually seeing it do something cool on my own photos and videos.

**WHAT?**

The project is basically a “find my dog” system. When I feed it an image or video, it first finds all the dogs, and then tries to decide which ones are my dog and which ones aren’t. Instead of doing some super complicated custom architecture, I split the job in two: YOLO11 handles the “where are the dogs?” part, and a small classifier I trained handles the “is this my dog or not?” part. In the end, I get bounding boxes around every dog, with my dog highlighted differently from other dogs.

**HOW?**

Under the hood, the process is pretty straightforward. I started by using YOLO11 to detect dogs in a bunch of images of my dog plus images of other dogs, and I saved those dog crops. Then I split them into training and validation sets for training the a YOLO classification model. At runtime, each frame goes through YOLO11 to find all dogs, I crop each box, run the crop through the classifier, and then use OpenCV to draw colored boxes and labels back onto the original image or video frame. It’s basically a loop of detect → crop → classify → draw, repeated for every dog the model finds.
