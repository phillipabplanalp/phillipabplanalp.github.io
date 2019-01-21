---
layout: post
title:  "Robotic Lawn Mower"
date:   2018-11-12
desc: ""
keywords: "RTK,GNSS,Robotics,Lawns"
categories: [robotics]
tags: []
icon: icon-html
---

Project Progress
================
## Architectural layout

For the mechanical layout it was opted to use a differential steer setup with two individually driven BLDC hub motors on the rear and a single freewheeling jockey wheel at the front.  The differential steer layout offers simplicity, agility and allows for a compact overall design - as can be seen in the image below. The layout below also shows the basic positioning of the three individual cutter motors/blades (red circles) and the forward-facing Lidar.

<img src="{{ site.img_path }}/blog/MowBot-Base.png"=20x>

With the mechanical designing having been somewhat constrained the core sensors and actuators could be considered - these are listed below:

<img src="{{ site.img_path }}/blog/MowBot-Core List of Sensors and Actuators.png" =250x>

Next stage was to define the electronics architecture. This was split into three sperate modules, which are as follows:

1.	Motor Drive Module
        The “Motor Drive Module” includes all the power electronics (BLDC controllers, SMPS, and regulators), single board PC (running ROS), PSoC 5LP MCU (controlling low level tasks). The module would also include numerus connectors.

2. Position and Comms Module (GNSS RTK Rover)

3.	Position Base Station (GNSS RTK Base)

This is a JavaScript snippet:

```
const add = (a, b) => a + b
const minus = (a, b) => a - b

console.log(add(100,200))  // 300
console.log(minus(100,200))  // -100
```

This is a Python snippet:

```
def say_hello():
    print("hello world!")

say_hello()   // "hello world!"
```

---

Side note comment: applied a bug fix similar to [this commit](https://github.com/Atlas7/atlas7.github.io/commit/6659f4a47f6ec66987adb0f683a9c6f3842252ae#diff-818954a41dbfb01af70050a459c603b9) to ensure code snippet does not collapse unexpectly upon clicking on it. This issue is tracked [here](https://github.com/jarrekk/Jalpc/issues/97).
