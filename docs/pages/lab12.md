---
title: "Path Planning and Execution"
description: '"The final piece of puzzle is to have the robot navigate through a set of waypoints in that environment as quickly and accurately as possible."'
layout: default
---

## Prelab

Before this lab, I made a plan for how I wanted to complete the traversal of the environment. Due to time contstraints, I figured that open-loop control would be easiest. Although setting delays might take some time, for simple translations and turns it will be easy to fine-tune open-loop control than closed-loop, where I need to rely on sensor measuerments.

## Lab Tasks

With my above plan in mind, I created the below algorithm for navigating the environment:

<script src="https://gist.github.com/j-simp/2878f9a92c42c468d9759d6de875271e.js"></script>

I created variables for each action and pause my robot takes so that I can rapidly debug my algorithm via bluetooth. Additionally, I tried to minimize pauses as much as possible by only pausing enough to decouple sequential actions as much as possible.

Here is my best run though the environment, which visits every checkpoint tile:

<div style="text-align: center;">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/Gu4HOQactlY" 
    frameborder="0" allowfullscreen></iframe>
</div>

And, as a bonus, some of my 'rapid' debugging:

<div style="text-align: center;">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/o8hUlR6P96o" 
    frameborder="0" allowfullscreen></iframe>
</div>

## Acknowledgements

I collaborated with Kotey Ashie in completing this lab. Thank you Prof. Helbling and all the TAs for an amazing semester!!! 