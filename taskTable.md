---
title: "Tasks Table"
permalink: /taskTable/
---

<a href="../pipsWorldEposter.pdf" target="_blank">Link to poster (higher quality)</a>

<h1 padding-left="-4rem" padding-right="-4rem">Task Clips</h1>

<div class="FlexContainer">
  <div class="FlexContainerCol">
    <h3>Gaze Following</h3>
    <div class="FlexContainer">
      <video id="GDP" src="../Video/GDP.mp4" autoplay muted loop preload></video>
    </div>
  </div>
  <div class="FlexContainerCol">
    <h3>Inferring Desire</h3>
    <div class="FlexContainer">
      <video id="UD" src="../Video/UD.mp4" autoplay muted loop preload></video>
    </div>
  </div>
</div>

<div class="FlexContainer">
  <div class="FlexContainerCol">
    <h3>False Belief</h3>
    <div class="FlexContainer">
      <video id="FB" src="../Video/FB.mp4" controls preload></video>
    </div>
  </div>
  <div class="FlexContainerCol">
    <h3>False Belief Word Learning</h3>
    <div class="FlexContainer">
      <video id="FBW" src="../Video/FBW.mp4" controls preload></video>
    </div>
  </div>
</div>

<div class="FlexContainer">
  <div class="FlexContainerCol">
    <h3>Reinforcement Learning</h3>
    <div class="FlexContainer">
      <video id="RL" src="../Video/RL.mp4" autoplay muted loop preload></video>
    	<div class="Overlay">
        <img src="../volumeOff.png" controlledVideoId="RL" onclick="toggleMute(this)">
      </div>
    </div>
  </div>
  <div class="FlexContainerCol">
    <h3>Social Reinforcement Learning</h3>
    <div class="FlexContainer">
      <video id="RLS" src="../Video/RLS.mp4" autoplay muted loop preload></video>
    </div>
  </div>
</div>

<div class="FlexContainer">
  <div class="FlexContainerCol">
    <h3>Emotion Recognition (beta)</h3>
    <div class="FlexContainer">
      <video id="ER" src="../Video/ER.mp4" autoplay muted loop preload></video>
    </div>
  </div>
  <div class="FlexContainerCol">
    <h3>Attentional Bias (beta)</h3>
    <div class="FlexContainer">
      <video id="EDP" src="../Video/EDP.mp4" autoplay muted loop preload></video>
    </div>
  </div>
</div>

<div class="FlexContainer">
  <div class="FlexContainerCol">
    <h3>Inhibitory Control</h3>
    <div class="FlexContainer">
      <video id="GNG" src="../Video/GNG.mp4" autoplay muted loop preload></video>
    	<div class="Overlay">
        <img src="../volumeOff.png" controlledVideoId="GNG" onclick="toggleMute(this)">
      </div>
    </div>
  </div>
  <div class="FlexContainerCol">
    <h3>Sustained Attention</h3>
    <div class="FlexContainer">
      <video id="SA" src="../Video/SA.mp4" autoplay muted loop preload></video>
    	<div class="Overlay">
        <img src="../volumeOff.png" controlledVideoId="SA" onclick="toggleMute(this)">
      </div>
    </div>
  </div>
</div>

<div class="FlexContainer">
  <div class="FlexContainerCol">
    <h3>Novelty/Familiarity (beta)</h3>
    <div class="FlexContainer">
      <video id="NF" src="../Video/NF.mp4" autoplay muted loop preload></video>
    </div>
  </div>
  <div class="FlexContainerCol">
    <h3>Decision-Making Under Uncertainty</h3>
    <div class="FlexContainer">
      <video id="MC" src="../Video/MC.mp4" autoplay muted loop preload></video>
    </div>
  </div>
</div>

<div class="FlexContainer">
  <div class="FlexContainerCol">
    <h3>Tactile Processing (beta)</h3>
    <div class="FlexContainer">
      <video id="TP" src="../Video/Kitten.mp4" autoplay muted loop preload></video>
    </div>
  </div>
  <div class="FlexContainerCol">
    <h3>Auditory Processing (beta)</h3>
    <div class="FlexContainer">
      <video id="AP" src="../Video/Birds.mp4" autoplay muted loop preload></video>
      <div class="Overlay">
        <img src="../volumeOff.png" controlledVideoId="AP" onclick="toggleMute(this)">
      </div>
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
