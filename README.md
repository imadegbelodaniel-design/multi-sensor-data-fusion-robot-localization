# multi-sensor-data-fusion-robot-localization
Python simulation of mobile robot localization using GPS, wheel odometry, IMU measurements, Kalman Filtering and an Extended Kalman Filter.
# Multi-Sensor Data Fusion and Robot Position Estimation Using Python

## 1. Project Overview

This project explores sensor fusion techniques for estimating the position, velocity, and heading of a simulated mobile robot.

The work investigates how information from multiple simulated sensors can be combined to improve localization accuracy compared with relying on individual sensor measurements.

The project was developed using Python in Google Colab as a self-directed engineering and research learning project.

## 2. Research Objectives

- Understand the fundamentals of mobile robot localization.
- Simulate GPS, wheel odometry, accelerometer, and gyroscope measurements.
- Implement Kalman Filtering for sensor fusion.
- Explore coordinate transformations between robot body and world reference frames.
- Implement an Extended Kalman Filter (EKF) for nonlinear robot motion estimation.
- Investigate how sensor measurement noise affects localization performance.

## 3. Project Development

### Stage 1: One-Dimensional Kalman Filter

Developed a simulated straight-line robot model and combined GPS position measurements with encoder velocity measurements.

### Stage 2: Two-Dimensional Sensor Fusion

Extended the simulation to two-dimensional robot motion using GPS, IMU acceleration, and wheel odometry.

### Stage 3: Coordinate Transformations

Explored rotation matrices and transformations between body-frame and world-frame acceleration measurements.

### Stage 4: Extended Kalman Filter

Implemented an EKF for a simulated mobile robot with position, velocity, and heading states, using GPS, wheel-speed, accelerometer, and gyroscope measurements.


## 4. Selected Simulation Results

| Experiment | GPS Position RMSE | Fused Position RMSE | Improvement |
|---|---:|---:|---:|
| 1D Kalman Filter | 1.943 m | 0.2819 m | 85.49% |
| 2D Kalman Filter | 2.0866 m | 0.2599 m | 87.55% |
| Extended Kalman Filter | 2.1283 m | 0.3325 m | 84.37% |

Additional EKF results:
- Fused velocity RMSE: 0.0488 m/s
- Heading RMSE: 0.0704 rad (4.04°)

These results are from simulated experiments and have not been validated using physical robot hardware.
**Note:** These results are from separate simulation experiments, not physical robot tests. Performance depends on the assumptions, sensor noise settings, and implementation of each experiment.

## 5. Tools and Technologies

- Python
- NumPy
- Matplotlib
- Google Colab
- Kalman Filtering
- Extended Kalman Filtering
- Sensor Fusion
- Coordinate Transformations

## 6. Current Scope and Limitations

This project is currently simulation-based. It does not represent a physical multi-robot implementation. No physical robot hardware integration or ROS 2 implementation has been completed.

The work provides a foundation for further study in robot localization, state estimation, sensor integration, and multi-robot manufacturing research.

## 7. Future Research Directions

- Integration with ROS 2.
- Testing with real sensor measurements.
- Robot simulation and visualization.
- Multi-robot coordination.
- Advanced sensor calibration and state estimation.

## 8. Author

**Daniel Imadegbelo**

B.Eng. Mechanical Engineering  
University of Benin, Nigeria  
2023

**Research Interests:** Robotics, sensor fusion, intelligent manufacturing, state estimation, automation, and engineering simulation.
