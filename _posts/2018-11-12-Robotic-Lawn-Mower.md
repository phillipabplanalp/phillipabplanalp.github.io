---
layout: post
title:  "Robotic Lawn Mower"
date:   2018-11-12
desc: ""
keywords: "RTK,GNSS,Robotics,Lawns"
categories: [robot]
tags: []
icon: icon-html
---
<style>
p.ex1 {
  padding-top: 10px;
  padding-right: 400px;
  padding-bottom: 10px;
  padding-left: 400px;
}
p.ex2 {
  padding-top: 50px;
  padding-right: 250px;
  padding-bottom: 50px;
  padding-left: 250px;
}
</style>



<p class="ex1">
<h1>Project Progress</h1>

<h2>Architectural layout</h2>
</p>

<p class="ex1">

For the mechanical layout it was opted to use a differential steer setup with two individually driven BLDC hub motors on the rear and a single freewheeling jockey wheel at the front.  The differential steer layout offers simplicity, agility and allows for a compact overall design - as can be seen in the image below. The layout below also shows the basic positioning of the three individual cutter motors/blades (red circles) and the forward-facing Lidar.

 </p>

 <p class="ex1">

<img src="{{ site.img_path }}/blog/MowBot-Base.png" alt="drawing" width="400"/>

 </p>

  <p class="ex1">
With the mechanical designing having been somewhat constrained the core sensors and actuators could be considered - these are listed below:

</p>


<img src="{{ site.img_path }}/blog/MowBot-Core List of Sensors and Actuators.png" alt="drawing" width="400"/>

Next stage was to define the electronics architecture. This was split into three separate modules, which are as follows:

1. **Core Drive Module (CDM)**

    The “Core Drive Module” is the main module on the rover and includes all the power electronics (BLDC controllers, SMPS and regulators), single board PC (running ROS), PSoC 5LP MCU (controlling low level tasks). The module also includes numerus connectors.  

2. **Positioning and Comms Module (PCM)**

     The “Positioning and Comms Module” includes all the navigational components (RTK GNSS and 9 axis IMU) plus wireless communications needed to receive the correction data from the base station (required for full RTK).  The reason for splitting the PCM from the CDM was to reduce the EMI effects on noise sensitive components such as the U-blox NEO-08P.

3. **Positioning Base Station (PBM)**

     The “Position Base Station” is essentially the same module as the “Position and Comms Module”. The difference being that the “Positioning Base Station” is in a fixed location transmitting the RTK error codes back to the rover (PCM).


These are represented as follows:


<img src="{{ site.img_path }}/blog/MowBot-Electronics Hardware.png" alt="drawing" width="1000"/>



Still in progress, more to be added soon!








---
