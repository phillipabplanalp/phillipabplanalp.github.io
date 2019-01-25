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
 width: 100%;
  margin-left: auto;
   margin-right: auto;
  max-width: 800px;


}
p.ex2 {
  padding-top: 50px;
  padding-right: 250px;
  padding-bottom: 50px;
  padding-left: 250px;
}
</style>

<style>
ol {
 width: 100%;
  margin-left: auto;
   margin-right: auto;
  max-width: 800px
}

ol li {
 width: 100%;
  margin-left: auto;
   margin-right: auto;
  max-width: 800px
}
h1{
 width: 100%;
  margin-left: auto;
   margin-right: auto;
  max-width: 800px;
}

h2{
 width: 100%;
  margin-left: auto;
   margin-right: auto;
  max-width: 800px;
}
div.d {
  text-align: justify;
}


</style>
<body>
<div class = "d">
<h1>Project Progress</h1>

<h2>Architectural layout</h2>


<p class="ex1">

For the mechanical layout it was opted to use a differential steer setup with two individually driven BLDC hub motors on the rear and a single freewheeling jockey wheel at the front.  The differential steer layout offers simplicity, agility and allows for a compact overall design - as can be seen in the image below. The layout below also shows the basic positioning of the three individual cutter motors/blades (red circles) and the forward-facing Lidar.
 </p>

 <p class="ex1">

<img src="{{ site.img_path }}/blog/MowBot-Base.png" alt="drawing" width="300"/><br>

 </p>

  <p class="ex1">

With the mechanical designing having been somewhat constrained the core sensors and actuators could be considered - these are listed below: <br>

</p>

<p class="ex1">
<img src="{{ site.img_path }}/blog/MowBot-Core List of Sensors and Actuators.png" alt="drawing" width="300"/> <br>
</p>

<p class="ex1">
Next stage was to define the electronics architecture. This was split into three separate modules, which are as follows:
</p>

<ol>
  <li> <b> Core Drive Module (CDM) </b> <br>

    The “Core Drive Module” is the main module on the rover and includes all the power electronics (BLDC controllers, SMPS and regulators), single board PC (running ROS), PSoC 5LP MCU (controlling low level tasks). The module also includes numerus connectors.  </li>

  <li> <b>Positioning and Comms Module (PCM) </b> <br>


     The “Positioning and Comms Module” includes all the navigational components (RTK GNSS and 9 axis IMU) plus wireless communications needed to receive the correction data from the base station (required for full RTK).  The reason for splitting the PCM from the CDM was to reduce the EMI effects on noise sensitive components such as the U-blox NEO-08P. </li>

<li> <b> Positioning Base Station (PBM) </b> <br>

     The “Position Base Station” is essentially the same module as the “Position and Comms Module”. The difference being that the “Positioning Base Station” is in a fixed location transmitting the RTK error codes back to the rover (PCM). </li>

</ol>

<p class="ex1">
These are represented as follows:<br>
</p>

<p class="ex2">
<img src="{{ site.img_path }}/blog/MowBot-Electronics Hardware.png" alt="drawing" width="1000"/> <br>
</p>


<p class="ex1">
<class="sketchfab-embed-wrapper"> <iframe width="640" height="480" src="https://sketchfab.com/models/b04675d7dd3a4dbdbd7963be850abe44/embed" frameborder="0" allow="autoplay; fullscreen; vr" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
</p>


Still in progress, more to be added soon!
