---
title: "Tasks Table"
permalink: /taskTable/
---

# I am a test title

<div class="flex-grid">'
  <div class="col" position="relative">
    <img src="../volumeOff.png" controlledVideoId="myVideo2" z-index="3000" position="absolute" onclick="toggleMute(this)">
    <video id="myVideo2" src="../TestWithSound.mp4" width="320" height="200" position="absolute" autoplay muted loop preload></video>
  </div>
  <div class="col">What does pip want</div>
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
