## Example Video

Remove iframe

<video autoplay loop width="250">

    <source src="Video/Test.webm"
            type="video/webm">

    <source src="Video/Test.mp4"
            type="video/mp4">

    Sorry, your browser doesn't support embedded videos.
</video>

New video

<video id="myVideo" src="Video/TestWithSound.mp4" width="320" height="200" autoplay loop preload></video>

<button onclick="toggleMute()" type="button">Mute sound</button>
<script>
var vid = document.getElementById("myVideo");

function toggleMute() { 
    vid.muted = !vid.muted;
}
</script>

And another new video

<video src="Test.mp4" width="320" height="200" autoplay loop preload></video>

## Example Game
