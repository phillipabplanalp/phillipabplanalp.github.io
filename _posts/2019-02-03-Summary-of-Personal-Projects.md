---
layout: post
title:  "Summary of Personal Projects"
date:   2019-02-03
desc: ""
keywords: ""
categories: [misc]
tags: []
icon: icon-html
---

<style>
p.ex1 {
 width: 100%;
  margin-left: auto;
   margin-right: auto;
  max-width: 800px;
  margin-top:0


}
p.ex2 {
  padding-top: 50px;
  padding-right: 250px;
  padding-bottom: 50px;
  padding-left: 250px;
}
</style>

<style>
ul {
 width: 100%;
  margin-left: auto;
   margin-right: auto;
  max-width: 800px
}

ul li {
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
    padding-top:0px;


  margin-bottom:1;
}
div.d {
  text-align: justify;
  }

div.gallery {
    margin: auto;
    border: 1px solid #ccc;
    float: left;
    width: 180px;
  }

  div.gallery:hover {
    border: 1px solid #777;
  }

  div.gallery img {
    width: 100%;
    height: auto;
    float: centre;

  }

  div.desc {
    padding: 15px;
    text-align: center;
  }
  .center {
    width: 100%;
  margin-left: auto;
   margin-right: auto;
  max-width: 800px;
  margin-top:0;
  margin-bottom:0px;


</style>
<body>
<div class = "d">

<p class="ex1">


      <h2>House Renovations</h2>
      <p class="ex1">
      <font face = "blank" size =" 2">Date: 2015-2019</font><br /><br>
      I bought a house in Palmerston North mid 2015 and have been doing a number of renovations to it over this period. I'm currently busy renovating the bathroom. <br>



      <div class="center">
      <div class="gallery">
        <a target="blank" href="{{ site.img_path }}/blog/Project Photos/House_Renovations/1.jpg">
          <img src="{{ site.img_path }}/blog/Project Photos/House_Renovations/1.jpg" width="600" height="400">
        </a>
        <div class="desc">Starting demolition of old bathroom</div>
      </div>

      </div>
      <div class="gallery">
        <a target="blank" href="{{ site.img_path }}/blog/Project Photos/House_Renovations/2.jpg">
          <img src="{{ site.img_path }}/blog/Project Photos/House_Renovations/2.jpg" width="600" height="400">
        </a>
        <div class="desc">Old shower having been removed</div>
      </div>

      <div class="gallery">
        <a target="blank" href="{{ site.img_path }}/blog/Project Photos/House_Renovations/3.jpg">
          <img src="{{ site.img_path }}/blog/Project Photos/House_Renovations/3.jpg" width="600" height="400">
        </a>
        <div class="desc">Entropy! New shower and toilet on the left and old shower and toilet on the right</div>
      </div>

      <div class="gallery">
        <a target="blank" href="{{ site.img_path }}/blog/Project Photos/House_Renovations/4.jpg">
          <img src="{{ site.img_path }}/blog/Project Photos/House_Renovations/4.jpg" width="600" height="400">
        </a>
        <div class="desc">Built a small corner retaining wall</div>
      </div>
      <br clear="all" /><br />  




      <h2>Robotic Lawn Mower v2.0</h2>
      <p class="ex1">
      <font face = "Verdana" size =" 2">Date: 2018-Ongoing</font><br><br>
       This project was a continuation of the robotic lawn mover v1.0, with many learnings from years of industry experience. This makes use of the most recent developments in low cost RTK GNSS receivers from Ublox. <a href="https://phillipabplanalp.github.io/robotics/2018/11/12/Robotic-Lawn-Mower.html"> I have started documenting this in more detail here</a><br>

       <div class="center">
       <div class="gallery">
         <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Robotic Lawn Mower v2.0/1.jpg">
           <img src="{{ site.img_path }}/blog/Project Photos/Robotic Lawn Mower v2.0/1.jpg" width="600" height="400">
         </a>
         <div class="desc">GNSS receiver and LoRa Transceiver for RTK (real time kinematics) correction data </div>
       </div>

       </div>
       <div class="gallery">
         <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Robotic Lawn Mower v2.0/2.JPG">
           <img src="{{ site.img_path }}/blog/Project Photos/Robotic Lawn Mower v2.0/2.JPG" width="600" height="400">
         </a>
         <div class="desc">5 x BLDC motor driver</div>
       </div>

       <div class="gallery">
         <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Robotic Lawn Mower v2.0/5.png">
           <img src="{{ site.img_path }}/blog/Project Photos/Robotic Lawn Mower v2.0/5.png" width="600" height="400">
         </a>
         <div class="desc">Initial PCB layout of GNSS and LoRa Module</div>
       </div>
       <div class="gallery">
         <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Robotic Lawn Mower v2.0/6.jpg">
           <img src="{{ site.img_path }}/blog/Project Photos/Robotic Lawn Mower v2.0/6.jpg" width="600" height="400">
         </a>
         <div class="desc">Testing the prototype of the BLDC motor controller with driver MOSFETs</div>
       </div>

       <div class="gallery">
         <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Robotic Lawn Mower v2.0/4.png">
           <img src="{{ site.img_path }}/blog/Project Photos/Robotic Lawn Mower v2.0/4.png" width="600" height="400">
         </a>
         <div class="desc">GNSS schematics</div>
       </div>
       <br clear="all" /><br />  

     <h2> Automated MTB Map Holder </h2>
     <p class="ex1">
     <font face = "Verdana" size =" 2">Date: 2013-2014</font><br /><br>

        For Mountain Bike Orienteering and Adventure racing you often use what is known as "Map Holder" (see left most image) which is essentially a mechanical mechanism that holds maps and allows you to rotate the map to keep the map facing north. The idea of this project was to Electromechanical control the map holder to always stay facing north. To do this I used a magnetometer (sense magnetic north) and a stepper motor to rotate the map to stay facing north<br>

        <div class="center">
        <div class="gallery">
          <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Automated MTB Map Holder/1.jpg">
            <img src="{{ site.img_path }}/blog/Project Photos/Automated MTB Map Holder/1.jpg" width="700" height="450">
          </a>
          <div class="desc">Existing manual map holder</div>
        </div>

        </div>
        <div class="gallery">
          <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Automated MTB Map Holder/2.jpg">
            <img src="{{ site.img_path }}/blog/Project Photos/Automated MTB Map Holder/2.jpg" width="700" height="450">
          </a>
          <div class="desc">Exploded view of complete assembly</div>
        </div>

        <div class="gallery">
          <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Automated MTB Map Holder/3.jpg">
            <img src="{{ site.img_path }}/blog/Project Photos/Automated MTB Map Holder/3.jpg" width="700" height="450">
          </a>
          <div class="desc">Test PCB with stepper motor</div>
        </div>

        <div class="gallery">
          <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Automated MTB Map Holder/4.jpg">
            <img src="{{ site.img_path }}/blog/Project Photos/Automated MTB Map Holder/4.jpg" width="1300" height="600">
          </a>
          <div class="desc">Stepper motor schematics</div>
        </div>
        <br clear="all" /><br />  


     <h2> Electroluminescent Driver </h2>
     <p class="ex1">
     <font face = "Verdana" size =" 2">Date: 2013</font><br /><br>

       This project used a 3.7V (Li-Po) input and stepped it up to 60V square wave AC.  It used custom buck boost with a H – Bridge to generate the AC .<br>



     <h2> Final Year Uni Project </h2>
     <div> <p class="ex1">
     <font face = "Verdana" size =" 2">Date: 2012</font><br /><br>
         <a href="https://drive.google.com/open?id=0B0ZJQaZUAgXhRVVOZDRtRVVPMGVhZ0NuT1o3eFJqMTdwMWZZ"> Copy of the report can be found here </a>
       </p>
      </div>
      <div class="center">
      <div class="gallery">
        <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Final Year Uni Project/1.jpg">
          <img src="{{ site.img_path }}/blog/Project Photos/Final Year Uni Project/1.jpg" width="700" height="450">
        </a>
        <div class="desc">Differential steer robot</div>
      </div>

      <div class="gallery">
        <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Final Year Uni Project/2.jpg">
          <img src="{{ site.img_path }}/blog/Project Photos/Final Year Uni Project/2.jpg" width="700" height="450">
        </a>
        <div class="desc">Brushed DC motors, Motor Drivers, MCU, GPS and Magnetometer</div>
      </div>


      <br clear="all" /><br />  



     <h2> Robotic Lawn Mower v1.0</h2>
     <p class="ex1">
     <font face = "Verdana" size =" 2">Date: 2010</font><br /><br>


      During my second year Uni summer break, I had started a robotic lawn mower project. This involved designing and building 2 x 200W H-Bridges as well as designing and building a sub frame around an existing lawn mower.
        <br>

        <div class="center">
        <div class="gallery">
          <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Robotic Lawn Mower v1.0/1.jpg">
            <img src="{{ site.img_path }}/blog/Project Photos/Robotic Lawn Mower v1.0/1.jpg" width="700" height="450">
          </a>
          <div class="desc">Old lawn mower fixed to a subframe</div>
        </div>


        <br clear="all" /><br />  


      <h2> Engine Dyno </h2>
      <p class="ex1">
      <font face = "Verdana" size =" 2">Date: 2005-2006 </font><br /><br>


       This was a project to build a test bench for testing our kart racing engines. It was designed to be an inertia-based dyno, using two old truck flywheels as its accelerating inertia. Using the equation τ = Iα the torque could be calculated. Using RPM and torque, power can be calculated . <br>

       <h2> Enclosed Kart Racing Trailer </h2>
       <p class="ex1">
       <font face = "Verdana" size =" 2">Date: 2004</font><br /><br>

       This was designed and built by my brother(12y) and I(14y) to carry two karts + spare parts. The images below show the trailer bare frame prior to it being enclosed<br>

       <div class="center">
       <div class="gallery">
         <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Enclosed Kart Racing Trailer/1.jpg">
           <img src="{{ site.img_path }}/blog/Project Photos/Enclosed Kart Racing Trailer/1.jpg" width="700" height="450">
         </a>
         <div class="desc">Trailer being tested before enclosing it</div>
       </div>

       <div class="gallery">
         <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Enclosed Kart Racing Trailer/2.JPG">
           <img src="{{ site.img_path }}/blog/Project Photos/Enclosed Kart Racing Trailer/2.JPG" width="700" height="450">
         </a>
         <div class="desc">Frame close to being completed in our parents’ workshop!</div>
       </div>

        <br clear="all" /><br />  

       <h2>Radio-Controlled Model aeroplane</h2>
       <p class="ex1">
       <font face = "Verdana" size =" 2">Date: 2001-2002 </font><br /><br>
       Built an ethanol-powered radio-controlled model airplane from a kitset (11y). <br>

       <div class="center">
       <div class="gallery">
         <a target="blank" href="{{ site.img_path }}/blog/Project Photos/Radio-Controlled Model Airplane/1.jpg">
           <img src="{{ site.img_path }}/blog/Project Photos/Radio-Controlled Model Airplane/1.jpg" width="700" height="450">
         </a>
         <div class="desc">Completed aeroplane - Photo taken about 20 years after it was completed</div>
       </div>

        <br clear="all" /><br />  




---
