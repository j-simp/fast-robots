---
title: "Stunts!"
description: '"The purpose of this lab is to combine everything you’ve done up till now to do fast stunts. This is the reason you labored all those long hours in the lab carefully soldering up and mounting your components!"'
layout: default
---

## Lab Tasks

For this lab, I decided to implememt the drift task. Below is the code that I used, which draws on previous labs:

<script src="https://gist.github.com/j-simp/12e0e6432999f09ad14d3f58dc43ce31.js"></script>

I first get the car to an appropiate distance from the wall, then the car does a 180 turn and drives in the direction it came from. I decided to only use P control because I knew that with an appropiate selection of the goal rotation angle the potential overshoot present would be negligable (and due to time constraints). At first, this led to a wide variation between trials:

<div style="display: flex; justify-content: center; gap: 20px;">
  <iframe width="350" height="200" src="https://youtube.com/embed/wOJgX0BGv40?feature=share" 
    frameborder="0" allowfullscreen></iframe>

  <iframe width="350" height="200" src="https://youtube.com/embed/qgVFY0Poscg?feature=share" 
    frameborder="0" allowfullscreen></iframe>
</div>

But after tuning the target angle I was able to get better results:

<div style="display: flex; justify-content: center; gap: 5px; flex-wrap: wrap;">
  <iframe width="350" height="200" src="https://youtube.com/embed/ccdulZH2w2I?feature=share" 
    frameborder="0" allowfullscreen></iframe>

  <iframe width="350" height="200" src="https://youtube.com/embed/zl4WBBpWMcA?feature=share" 
    frameborder="0" allowfullscreen></iframe>

  <iframe width="350" height="200" src="https://youtube.com/embed/S0pv9vBzzXg?feature=share" 
    frameborder="0" allowfullscreen></iframe>
</div>

To get more of a drift effect, what I could do is keep the wheels spinning faster when the car is doing the 180.

## Acknowledgements

I referenced past students [Mikayla Lahr's](https://mikaylalahr.github.io/FastRobotsLabReports/startbootstrap-resume-master/dist/index.html#Lab%208) and [Nila Narayan's](https://nila-n.github.io/Lab8.html) websites for code setup.

