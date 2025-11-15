# self-balancing-bot

## Demo
![Demo](assets/Self-Balancing%20Robot%20Demo.gif)

![Demo](assets/Kalman%20Demo.gif)

## Overview

This project implements a real-time embedded control system for a two-wheeled, inverted pendulum robot. The core of the system is a closed-loop C++ pipeline running on an Arduino Uno that handles sensor fusion, state estimation, and motor control to maintain balance.

## Achievements

- **Real-Time Control Pipeline:** Developed and optimized a custom control loop, achieving a consistent 100 Hz (10ms latency) execution rate
- **Advanced State Estimation:** Engineered a custom Kalman Filter to fuse noisy MPU6050 accelerometer and gyro data, providing a robust tilt estimate by eliminating noise
- **Control System Tuning:** Implemented and tuned a PID controller, achieving stable self-balancing

## Architecture

Sensing via IMU -> State Estimation via Kalman filter -> State -> Control (PID) -> Actuation Signal (Arduino PWM) -> Actuation (DC Motors and L298N Driver)

## Components

- Arduino Uno R4 WiFi
- 2x TT DC Gear Motor
- MPU6050 IMU
- L298N Motor Driver

