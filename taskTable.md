---
title: "Tasks Table"
permalink: /taskTable/
---

# Task Clips

<div class="flex-grid">
  <div class="col">
    <h2>Gaze Following</h2>
    <video id="GDP" src="../Video/GDP.mp4" autoplay muted loop preload></video>
  </div>
  <div class="col">
    <h2>Inferring Desire</h2>
    <video id="UD" src="../Video/UD.mp4" autoplay muted loop preload></video>
  </div>
</div>
<div class="flex-grid">
  <div class="col">
    <h2>False Belief</h2>
    <video id="FB" src="../Video/FB.mp4" controls preload></video>
  </div>
  <div class="col">
    <h2>False Belief Word Learning</h2>
    <video id="FBW" src="../Video/FBW.mp4" controls preload></video>
  </div>
</div>
<div class="flex-grid">
  <div class="col">
    <h2>Reinforcement Learning</h2>
    <div class="container">
      <div class="navi">
        <video id="RL" src="../Video/RL.mp4" autoplay muted loop preload></video>
      </div>
      <div class="infoi">
        <img src="../volumeOff.png" controlledVideoId="RL" onclick="toggleMute(this)">
      </div>
    </div>
  </div>
  <div class="col">
    <h2>Social Reinforcement Learning</h2>
    <video id="RLS" src="../Video/RLS.mp4" autoplay muted loop preload></video>
  </div>
</div>
<div class="flex-grid">
  <div class="col">
    <h2>Emotion Recognition</h2>
    <video id="ER" src="../Video/ER.mp4" autoplay muted loop preload></video>
  </div>
  <div class="col">
    <h2>Attentional Bias</h2>
    <video id="EDP" src="../Video/EDP.mp4" autoplay muted loop preload></video>
  </div>
</div>
<div class="flex-grid">
  <div class="col">
    <h2>Inhibitory Control</h2>
    <div class="container">
      <div class="navi">
        <video id="GNG" src="../Video/GNG.mp4" autoplay muted loop preload></video>
      </div>
      <div class="infoi">
        <img src="../volumeOff.png" controlledVideoId="GNG" onclick="toggleMute(this)">
      </div>
    </div>
  </div>
  <div class="col">
    <h2>Sustained Attention</h2>
    <div class="container">
      <div class="navi">
        <video id="SA" src="../Video/SA.mp4" autoplay muted loop preload></video>
      </div>
      <div class="infoi">
        <img src="../volumeOff.png" controlledVideoId="SA" onclick="toggleMute(this)">
      </div>
    </div>
  </div>
</div>
<div class="flex-grid">
  <div class="col">
    <h2>Novelty/Familiarity</h2>
    <video id="NF" src="../Video/NF.mp4" autoplay muted loop preload></video>
  </div>
  <div class="col">
    <h2>Visual Decision-Making Under Uncertainty</h2>
    <video id="MC" src="../Video/MC.mp4" autoplay muted loop preload></video>
  </div>
</div>
<div class="flex-grid">
  <div class="col">
    <h2>Kittens</h2>
    <video id="EDP" src="../Test.mp4" autoplay muted loop preload></video>
  </div>
  <div class="col">
    <h2>Birds</h2>
    <video id="EDP" src="../Test.mp4" autoplay muted loop preload></video>
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
