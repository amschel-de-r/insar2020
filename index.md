## Example Video

Remove iframe

<video autoplay muted loop width="250">

    <source src="Video/Test.webm"
            type="video/webm">

    <source src="Video/Test.mp4"
            type="video/mp4">

    Sorry, your browser doesn't support embedded videos.
</video>

New video

<video id="myVideo" src="TestWithSound.mp4" width="320" height="200" autoplay controls muted loop preload></video>

<button onclick="toggleMute()" type="button">Mute sound</button>

<script>
function toggleMute() { 
    var vid = document.getElementById("myVideo");
    vid.muted = !vid.muted;
}
</script>

And another new video

<video src="Test.mp4" width="320" height="200" autoplay muted loop preload></video>

## Example Game
