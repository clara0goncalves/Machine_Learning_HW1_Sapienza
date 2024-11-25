# Homework 1: Robot Kinematics

## Overview
This repository contains the implementation for Homework 1: **Robot Kinematics**, part of the Machine Learning course (2024/25). The assignment involves generating datasets using robotic simulators, training models to predict forward kinematics.

### Course Details
- **Course**: Machine Learning 2024/25  
- **Professor**: Luca Iocchi  
- **Master Program**: Artificial Intelligence and Robotics  
- **Deadline**: 8th December 2024, 23:59 CET  

---

## Objectives
1. **Dataset Generation**:
   - Simulate robots with 2D (2 joints, 3 joints) and 3D (5 joints) configurations using Mujoco.
   - Collect and preprocess data of joint angles, fingertip positions, and orientations.
   
2. **Forward Kinematics**:
   - Train models to predict fingertip positions based on joint angles.
   - Compare learned Jacobians with analytical Jacobians (focus on the 2-joint robot).

---

## Steps to Complete the Assignment

### 1. Dataset Generation
- Use the Mujoco simulator to generate datasets for robots with different configurations:
  - 2D (2 joints and 3 joints)
  - 3D (5 joints)
  - Save the generated data in CSV format, including:
  - Joint angles, fingertip positions, and orientations.
  - Perform preprocessing (e.g., normalizing angles, representing them with `sin` and `cos`).

### 2. Train Forward Kinematics Models
- Define feedforward models to learn forward kinematics for each robot.
- Train the models on joint angle inputs to predict fingertip positions.
- Split the data into training and testing sets, ensuring logs from different seeds are used for training and testing.

### 3. Compare Jacobians
- Compute the Jacobian matrix for the learned forward kinematics using automatic differentiation.
- Compare the computed Jacobian with the analytical Jacobian for the 2-joint robot.

### 6. Documentation and Submission
- Write a detailed report covering:
  - Data generation and preprocessing.
  - Model architecture and hyperparameter configurations.
  - Training process and evaluation results.
  - Comparisons of Jacobians and any additional findings.
  - Submit a ZIP file containing the code and a separate PDF report.

---

## Tools and Environment
- **Platform**: Google Colab  
- **Framework**: PyTorch  
- **Simulation Tool**: Mujoco  
- **Data Handling**: Pandas  
- **Visualization**: Matplotlib 

---

## Deliverables
1. **Report**:
   - PDF document including:
     - Data generation/preprocessing steps.
     - Model design and configurations.
     - Training process and hyperparameter search results.
     - Performance metrics (e.g., training curves, test accuracy).
     - Comparisons of analytical vs. learned Jacobians.
     - Conclusions and future work.

2. **Code**:
   - ZIP file containing all the implemented code for the project.
   - Ensure it includes:
     - Dataset generation scripts.
     - Model training and evaluation scripts.
     - Jacobian computation and comparison.

---

## Notes
- Adhere strictly to the deadline: **8th December 2024, 23:59 CET**.
- Ensure all deliverables are submitted via Classroom.  
