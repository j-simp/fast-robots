---
title: "Orientation Control"
description: '"The purpose of this lab is to get experience with orientation PID using the IMU."'
layout: default
---

## Prelab

Before this lab, I read over the lab tasks and devised a plan for rotation control. Like my [Linear PID lab](./lab5.md), I decided to start with P control, and if my car was not quickly converging to a set point, I would try to include the derivative and/or integral terms.

## Lab Tasks

### P Control

Below is the code I used to implement P control:

<script src="https://gist.github.com/j-simp/c5d799712cb72fdbc17fb3e0061c2ceb.js"></script>

Note that I have functionality to stop the control loop when the car has been at the target angle for enough time. This was included to ensure that the car's stopping location was consistent, and this functionality was disabled when I was testing if the robot could hold at an angle (and not have any unexpected jumps).

First, I tried this control with Kp = 0.5:

<div style="text-align: center;">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/G75Z7lFZ9no" 
    frameborder="0" allowfullscreen></iframe>
</div>

Since this led to constant overshooting of the target angle, I reduced Kp to 0.1:

<div style="text-align: center;">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/41SCoGXn5GQ" 
    frameborder="0" allowfullscreen></iframe>
</div>

While this was better, I figured that instead of incorporating another term into the control loop, I would try Kp = 0.05 to see if I could achieve satisfactory results:

<div style="text-align: center;">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/unKONuLc0ok" 
    frameborder="0" allowfullscreen></iframe>
</div>

Kp = 0.05 seemed to work very well, and I confirmed this with the 'kick test':

<div style="text-align: center;">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/9MLquNn8DDw" 
    frameborder="0" allowfullscreen></iframe>
</div>

Therefore, with Kp = 0.05, I was able to complete orientation control.  


## Acknowledgements

I referenced past students [Mikayla Lahr's](https://mikaylalahr.github.io/FastRobotsLabReports/startbootstrap-resume-master/dist/index.html#Lab%206) and [Nila Narayan's](https://nila-n.github.io/Lab6.html) websites for implementing the methods.