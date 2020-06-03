---
title: "Bayesian Optimisation"
permalink: /bayesopt/
---

## What is bayesian optimisation?
Bayesian optimization is a powerful iterative method to efficiently obtain the extrema of target functions that are expensive to evaluate ([Mockus, 1994](https://www.nature.com/articles/s41467-018-03657-3.pdf)). The approach employs a Bayesian statistical model to estimate the target function f(x) according to its posterior distribution, and an acquisition function that proposes the point in the space to be sampled in the next iteration.

![Alt Text](bayesopt.gif?raw=true)

See also [Brochu et al., 2010](https://arxiv.org/abs/1012.2599) and [Agnihotri & Batra, 2020](https://distill.pub/2020/bayesian-optimization/) for more thorough explanations.

## How do we use BO?

In our "Catch the Puppy" task, speed affects how valid the task is as a measure of inhibition.
_(Exaggerated speeds used for illustration)_
<div class="FlexContainer">
  <div class="FlexContainerCol">
    <div>Too slow and the participant has excessive time to prepare inhibition</div>
    <div class="FlexContainer">
      <video id="GNGSlow" src="Video/GNGslow.mp4" autoplay muted loop preload></video>
    </div>
  </div>
  <div class="FlexContainerCol">
    <div>Too fast and the participant is unable to even hit the "Go" trials</div>
    <div class="FlexContainer">
      <video id="GNGFast" src="Video/GNGfast.mp4" autoplay muted loop preload></video>
    </div>
  </div>
</div>

Finding an optimal speed ensures a reliable hit-rate for "Go" trials, making the error-rate on "No-Go" trials a more meaningful dependent variable. However, as this optimal speed will vary for different people, particularly in young children with varying levels of developmental delay. Having children do the task multiple times at different speed levels poses a significant demand on attention and motivation; using Bayesian Optimisation offers a way to find each individual's optimal speed in relatively few trials.

## Implementation
By using a warm-up task that serves to familiarise with tablet, we can test how well an individual can click bubbles moving across screen at variable speeds.
If we code (speed x hit-rate) as one variable, we can optimise to find the fastest speed where an individual can still achieve an 80-100% hit rate. Throughout the task the Bayesian Optimisation uses each new piece of data to update its estimate of the target function (how well the child will perform over the speed range), then runs an Acquisition Function to determine where in the speed range to sample next, determining the speed for the following trials.

<div class="FlexContainer">
  <div class="FlexContainerCol">
    <div class="FlexContainer">
      <video id="BAO" src="Video/BOBubbles.mp4" autoplay muted loop preload></video>
    </div>
  </div>
</div>

## Want to have a go for yourself? Try out below
N.B. optimisation still undergoing fine-tuning, and may as of yet not adapt perfectly to all individuals. Speed range may also not contain optimal speed for all individuals

<div style="position:relative;padding-bottom:62.5%;">
  <iframe style="width:100%;height:100%;position:absolute;left:0px;top:0px;" src="Bubbles/index.html"></iframe>
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
