## Example Videos

Autoplay silent video

<video autoplay muted loop width="320">

    <source src="Video/Test.webm"
            type="video/webm">

    <source src="Video/Test.mp4"
            type="video/mp4">

    Sorry, your browser doesn't support embedded videos.
</video>

Video that can be muted

<video id="myVideo" src="TestWithSound.mp4" width="320" height="200" autoplay controls muted loop preload></video>

<button onclick="toggleMute()" type="button">Mute sound</button>

<script>
var vid = document.getElementById("myVideo");
function toggleMute() { 
    var vid = document.getElementById("myVideo");
    vid.muted = !vid.muted;
}
</script>

## Example Game

<iframe src="Bubbles/index.html" style="width:960px; height:650px">
