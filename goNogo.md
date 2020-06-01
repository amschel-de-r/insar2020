---
title: "Go-NoGo \"Catch the Puppy\" task"
permalink: /gonogo/
---

# Task Breakdown
N.B. correct videos not yet added
## Pre-test: Motor Response
Bubble speed is varied, with response used to optimise the speed of the subsequent Go-NoGo task
<div class="FlexContainer">
  <div class="FlexContainerCol">
    <div class="FlexContainer">
      <video id="GDP" src="../Video/GDP.mp4" autoplay muted loop preload></video>
    </div>
  </div>
</div>
[Click here](../) to learn more about the Bayesian Optimisation process, including a playable version of the game
## Animated Cartoon
In the cartoon, the child is introduced to and familiarised with the task stimuli (puppy and cat), and given a sense of which is to be touched and which avoided
<div class="FlexContainer">
  <div class="FlexContainerCol">
    <div class="FlexContainer">
      <video id="GDP" src="../Video/GDP.mp4" autoplay muted loop preload></video>
    </div>
  </div>
</div>
## Categorisation Demo
The stimuli are introduced with symbols, a character (the scientist) and the parent both demonstrate to click the puppy
<div class="FlexContainer">
  <div class="FlexContainerCol">
    <div class="FlexContainer">
      <video id="GDP" src="../Video/GDP.mp4" autoplay muted loop preload></video>
    </div>
  </div>
</div>
## Pre-test: Categorisation
This pre-test determines base ability to distinguish the task stimuli and click the correct one
<div class="FlexContainer">
  <div class="FlexContainerCol">
    <div class="FlexContainer">
      <video id="GDP" src="../Video/GDP.mp4" autoplay muted loop preload></video>
    </div>
  </div>
</div>
## Task Demo
The scientist and parent both demonstrate how to play the game, this time with stimuli moving across the screen
<div class="FlexContainer">
  <div class="FlexContainerCol">
    <div class="FlexContainer">
      <video id="GDP" src="../Video/GDP.mp4" autoplay muted loop preload></video>
    </div>
  </div>
</div>
## Task Practice
The child is given a 10-trial practice, which can be repeated
<div class="FlexContainer">
  <div class="FlexContainerCol">
    <div class="FlexContainer">
      <video id="GDP" src="../Video/GDP.mp4" autoplay muted loop preload></video>
    </div>
  </div>
</div>
## Main Task
Consisting of 40 trials at optimised speed, the main task measures ability to inhibit motor response. If attention is lost and go-trials are missed, the puppy barks to re-engage the child.
<div class="FlexContainer">
  <div class="FlexContainerCol">
    <div class="FlexContainer">
      <video id="GDP" src="../Video/GDP.mp4" autoplay muted loop preload></video>
    </div>
  </div>
</div>

<script>
var vid = document.getElementById("myVideo");
function toggleMute(el) { 
    var vidId = el.getAttribute('controlledVideoId');
    var vid = document.getElementById(vidId);
    vid.muted = !vid.muted;
    el.src = vid.muted ? "../volumeOff.png" : "../volumeOn.png";
}
</script>
