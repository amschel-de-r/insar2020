---
title: "Tasks Table"
permalink: /taskTable/
---

# I am a test title

<p1>Which</p1>
<p2>Of us</p2>
<p3>Do you want?</p3>

<div class="flex-grid">
  <div class="col">
    <div>First video</div>
    <video id="myVideo2" src="../TestWithSound.mp4" autoplay muted loop preload></video>
  </div>
  <div class="col">
    <div>Second video</div>
    <div class="container">
    <div class="navi">
      <video id="myVideo" src="../TestWithSound.mp4" autoplay muted loop preload></video>
    </div>
    <div class="infoi">
      <img src="../volumeOff.png" controlledVideoId="myVideo" onclick="toggleMute(this)">
    </div>
</div>
  </div>
</div>
<div class="flex-grid">
  <div class="col">FB</div>
  <div class="col">FBW</div>
</div>
<div class="flex-grid">
  <div class="col">RL</div>
  <div class="col">RLS</div>
</div>
<div class="flex-grid">
  <div class="col">ER</div>
  <div class="col">BUtterfly</div>
</div>
<div class="flex-grid">
  <div class="col">GNG</div>
  <div class="col">SA</div>
</div>
<div class="flex-grid">
  <div class="col">NF</div>
  <div class="col">MC</div>
</div>
<div class="flex-grid">
  <div class="col">Kittens</div>
  <div class="col">Birds</div>
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
