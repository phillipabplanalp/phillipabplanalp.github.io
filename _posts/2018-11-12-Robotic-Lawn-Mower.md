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

With the mechanical designing having been somewhat constrained the core sensors and actuators could be considered - these are listed below: <br><br>

</p>

<p class="ex1">
<img src="{{ site.img_path }}/blog/MowBot-Core List of Sensors and Actuators.png" alt="drawing" width="300"/> <br><br>
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
These are represented as follows:
</p>

<p class="ex2">
<img src="{{ site.img_path }}/blog/MowBot-Electronics Hardware.png" alt="drawing" width="1000"/> <br>
</p>
<p class="ex2">
<h2 Positioning & Comms Module: /h2>

The Positioning & Comms Module has been has four key components:




<p class="ex1">
<iframe width="640" height="480" src="https://sketchfab.com/models/b04675d7dd3a4dbdbd7963be850abe44/embed" frameborder="0" allow="autoplay; fullscreen; vr" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
</p>

<p class="ex1">
Testing of U-blox neo M8P on the Positioning & Comms PCB using U-blox U-Centre <br>
</p>

<p class="ex2">
<img src="{{ site.img_path }}/blog/MowBot-Electronics Hardware.png" alt="drawing" width="1000"/> <br>
</p>
<h2> Positioning & Comms Module</h2>
<p class="ex1">

As outlined above, the "Positioning & Comms Module" is the core navigational sensor on the "rover", it will provide cm level positional accuracy(+-2.5cm) through RTK GNSS and magnetometer heading angle. For RTK GNSS to work, it requires a continues stream of correction data to be sent from a fixed known location (base station) to the "rover" so some form of wireless communication required to relay this information on. The key components that have been chosen for this module are:

<ol>
  <li> 9 axis IMU - ST LSM9DS1TR - First stage only the magnetometer will be used.
  <li> GNSS Module - NEO-M8P-0 - Provides high level of positional accuracy.
  <li> Wireless Comms - Microchip LoRa RN2903A – facilitates communication to base station.
  <li> MCU - Cypress PSoC 4 CY8C4245AZI-473 - Handles communication between NEO-M8P, LoRa module, Core Drive Module and IMU.

</ol>
<p class="ex1">

PCB imported into Solidworks to double checked component clearances to enclosure- See interactive 3D model of PCB and Cinch Enclosure.

<p class="ex1">

<iframe width="640" height="480" src="https://sketchfab.com/models/b04675d7dd3a4dbdbd7963be850abe44/embed" frameborder="0" allow="autoplay; fullscreen; vr" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe> <br> <br>
</p>

<p class="ex1">



Assembled PCB and Connector. Started testing of U-blox neo M8P on the Positioning & Comms PCB using U-blox U-Centre connected through USB <br>
</p>

<p class="ex1">
<img src="{{ site.img_path }}/blog/Testing Pos Module.jpg" alt="drawing" width="400"/> <br>
</p>
<p class="ex1">

Still in progress, more to be added soon!
</p>
