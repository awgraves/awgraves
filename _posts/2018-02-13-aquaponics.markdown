---
layout: post
title: Aquaponics Crop Management "Software"
date: 2018-02-13 10:02:45
description: That time I created management "software" for farmers utilizing only spreadsheets.
img: /aquaponics/aquaponics.jpg # Add image post (optional)
tags: [Excel, SQL]
---
<p align = "center">
<b>
Using Google Sheets to build an interactive crop management program for farmers in the Dominican Republic

</b>
</p>
<br>
<br>

## The Story:

<head> 
  <!-- Your stuff --> 
  <link rel="stylesheet" href="style/slider-def.css"> 
</head>

<p align = "center">
    <div id="slider">
      <div class="slides">
        <div class="slider">
          <div class="legend"></div>
          <div class="content">
            <div class="content-txt">
              <h1>Identifying a Problem:</h1>
              <h2>Prior to August 2016, the aquaponics system at Finca Taino was not running on a plant / harvest schedule.  This made it difficult for the farmers to estimate when and how much of a crop would be ready to sell at market.</h2>
            </div>
          </div>
          <div class="image">
            <img src="../assets/img/aquaponics/semillado.JPG">
          </div>
        </div>
        <div class="slider">
          <div class="legend"></div>
          <div class="content">
            <div class="content-txt">
              <h1>Creating a Solution:</h1>
              <h2>The farmers were interested in a more systematic approach. They only had a Samsung tablet and a google account at their disposal.  I decided to build them a crop management system from scratch using Google Sheets.</h2>
            </div>
          </div>
          <div class="image">
            <img src="../assets/img/aquaponics/me.JPG">
          </div>
        </div>
        <div class="slider">
          <div class="legend"></div>
          <div class="content">
            <div class="content-txt">
              <h1>Dashboard Sheet</h1>
              <h2>The "dashboard" displays summary info about the plants growing in the system. It indicates the next planting and harvesting dates as well as the estimated crop yields in pounds.</h2>
            </div>
          </div>
          <div class="image">
            <img src="../assets/img/aquaponics/dash.png">
          </div>
         </div> 
        <div class="slider">
          <div class="legend"></div>
          <div class="content">
            <div class="content-txt">
              <h1>Crop Sheet</h1>
              <h2>There are many "batches" of the same crop that are planned to mature at regular intervals. The program highlights a harvest-ready batch in red and alerts the farmers when to plant a new group.</h2>
            </div>
          </div>
          <div class="image">
            <img src="../assets/img/aquaponics/crop.png">
          </div>
        </div> 
        <div class="slider">
          <div class="legend"></div>
          <div class="content">
            <div class="content-txt">
              <h1>Systemized Production</h1>
              <h2>Now the farmers can better estimate their crop yields and have automated to-do lists to keep their production running smoothly.</h2>
            </div>
          </div>
          <div class="image">
            <img src="../assets/img/aquaponics/aquaponics.jpg">
          </div>
        </div>
       </div>
      <div class="switch">
        <ul>
          <li>
            <div class="on"></div>
          </li>
          <li></li>
          <li></li>
          <li></li>
          <li></li>
        </ul>
      </div>
     </div> 
</p>

<br>
## What were the key Excel skills involved?
- Formulas
- Linking cells across multiple sheets
- Data validations
- Conditional formatting
- IF functions
- INDEX / MATCH functions
- QUERY functions (SQL statements)

<br>
## What is aquaponics?
It is a unique way to grow plants and raise fish together without any soil!  Learn more [here](https://www.theaquaponicsource.com/what-is-aquaponics/).

<br>
## Wouldn't this software work for traditional farming methods too?
Sure!  I chose to design this for the aquaponics system at [Finca Taino](http://tainofarm.com/) due to the popularity of the crops being grown as well as the shorter growth cycles that result from this special farming method - the quicker the growth the greater the potential volume of output!
<br>

# *See it in action!*

### Dashboard:
<p align = "center"><iframe width="560" height="315" src="https://www.youtube.com/embed/4MQ4N0x6m2s" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe></p>
<br>
### Planting:
<p align = "center"><iframe width="560" height="315" src="https://www.youtube.com/embed/tHZTc1DN1NY" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe></p>
<br>
### Harvesting &
### Transferring:
<p align = "center"> 
<iframe width="560" height="315" src="https://www.youtube.com/embed/8WiQcwp69Ik" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe></p>
<br>
## What are the calculations based on?

It is important to note that this is by no means a perfect system.  The program is meant to be a rough guide and the base numbers should be tweaked with trial and error.
<br>
<br>
### The program requires the following inputs for each crop:
 - Average length of growth cycle (in days)
 - Desired harvest frequency (in days)
 - Desired grow-space allocation (percentage)
 - An example harvest plant count
 - Total weight of example harvest
 <br>
 <br>
### These inputs are the basis for calculating:
- The next plant / harvest dates
- The size and # of groups that can fit in the system without exceeding the crop's alloted space
- Estimated yield in pounds per harvest
<br>
<br>
![first]({{site.url}}/assets/img/aquaponics/calculations.png)


<br>
[Slide Viewer Code](https://codepen.io/Eliteware/full/BoBgqV)