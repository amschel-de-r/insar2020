## Example Videos

Autoplay silent video

<video autoplay muted loop width="320">

    <source src="Video/Test.webm"
            type="video/webm">

    <source src="Video/Test.mp4"
            type="video/mp4">

    Sorry, your browser doesn't support embedded videos.
</video>

Videos that can be muted

<div class="row">
  <div class="column">
    <video id="myVideo" src="TestWithSound.mp4" width="320" height="200" autoplay muted loop preload></video>
  </div>
  <div class="column">
    <img src="volumeOff.png" controlledVideoId="myVideo" onclick="toogleMute()">
  </div>
</div>

<div class="row">
  <div class="column">
    <video id="myVideo2" src="TestWithSound.mp4" width="320" height="200" autoplay muted loop preload></video>
  </div>
  <div class="column">
    <img src="volumeOff.png" controlledVideoId="myVideo2" onclick="toogleMute()">
  </div>
</div>

<script>
var vid = document.getElementById("myVideo");
function toggleMute(event) { 
    var el = event.target;
    var vidId = el.getAttribute('controlledVideoId');
    var vid = document.getElementById(vidId);
    vid.muted = !vid.muted;
    el.src = vid.muted ? "volumeOff.png" : "volumeOn.png";
}
</script>

## Example Game

<iframe src="Bubbles/index.html" style="width:960px; height:650px">
