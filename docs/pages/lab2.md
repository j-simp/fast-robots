---
title: "Lab 2: IMU"
description: " "
layout: default
---

## Prelab
## Lab Tasks

### 1: IMU SETUP

Note the AD0_VAL definition. What does it represent, and should it be 0 or 1?
- It represents whether the ADR jumper is soldered closed (0) or not (1). Since it is not soldered closed, we want it to be 1.

Check out the change in sensor values as you rotate, flip, and accelerate the board. Explain what you see in both acceleration and gyroscope data.
- I noticed that when the IMU is held with one axis facing towards the ground, the magnitude of the scaled acceleration is about 1000 in that axis. Additionally, the gyroscope reports displacement values from the previous position, and the orientation is relative to the previous orientation and not a global orientation.

### 2: Accelerometer
### 3: Gyroscope
### 4: Sample Data
### 5: Stunt!
[![Watch the video](https://img.youtube.com/vi/4z1Af2QlYwI/0.jpg)](https://www.youtube.com/watch?v=4z1Af2QlYwI)

## Reflection

