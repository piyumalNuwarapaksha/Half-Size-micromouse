# Half-Sized Micromouse

A compact **half-sized Micromouse robot** designed for autonomous maze solving and high-speed navigation. The robot combines custom mechanical design, precise motor feedback, distance sensing, and closed-loop motion control.

## Features

* **ESP32** microcontroller for real-time control and navigation
* **4-wheel drive** configuration for improved traction and stability
* **Custom-made gear reduction mechanism** for compactness and higher torque
* **AS5048 magnetic encoders** for accurate wheel position and speed feedback
* **Pololu PWM Time-of-Flight (ToF) sensors** for wall and distance detection
* **BNO055 IMU** for orientation and gyro-based motion estimation
* **DRV8833 dual motor drivers** for controlling the four motors
* Custom 4 layer PCB and mechanical design optimized for a half-sized Micromouse

## System Overview

The ESP32 collects data from the ToF sensors, magnetic encoders, and BNO055 IMU. This sensor information is used to estimate the robot's position, detect maze walls, maintain alignment, and control the wheel motors.

The motor control system uses encoder feedback for closed-loop speed and motion control, while the ToF sensors provide information about the surrounding maze walls.

## Hardware

| Component                | Purpose                                  |
| ------------------------ | ---------------------------------------- |
| ESP32                    | Main microcontroller                     |
| 4 × DC Motors            | Four-wheel drive                         |
| Custom Gear Reduction    | Increase torque and optimize motor speed |
| AS5048 Magnetic Encoders | Wheel position/speed feedback            |
| Pololu PWM ToF Sensors   | Wall/distance measurement                |
| BNO055                   | Orientation and inertial measurement     |
| DRV8833                  | Dual-channel motor driver                |

## Control System

The robot is designed around closed-loop control. Encoder feedback is used to control motor speed and movement, while ToF sensors are used for wall following and maze navigation.

The BNO055 provides orientation information that can assist with accurate turning and heading estimation.

## Mechanical Design

The chassis and gear reduction mechanism are custom designed specifically for the half-sized Micromouse platform. The four-wheel configuration provides stable contact with the maze surface while keeping the robot compact.

## Project Goals

* Accurate wall detection
* Precise straight-line movement
* Reliable 90° and 180° turns
* Closed-loop motor control
* Fast and stable maze navigation
* Compact mechanical and electronic design

## Technologies

**Embedded:** ESP32
**Sensors:** AS5048, Pololu PWM ToF, BNO055
**Motor Control:** DRV8833, encoder-based closed-loop control
**Mechanical:** Custom gear reduction and chassis design

## Status

🚧 **In Development**

This project is being developed iteratively, with improvements to the mechanical system, motor control, sensor processing, and maze-solving algorithms.
