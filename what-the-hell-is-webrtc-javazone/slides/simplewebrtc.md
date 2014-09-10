<h2><span style="color: #ec008c;">simple</span><span style="color: #12acef;">WebRTC</span></h2>

````javascript
var webrtc = new SimpleWebRTC({
    localVideoEl: 'localVideo',
    remoteVideosEl: 'remotesVideos',
    autoRequestMedia: true
});
webrtc.on('readyToCall', function () {
    webrtc.joinRoom('your awesome room name');
});
````

note:
- Luckily, some really nice guys have created a simple way for you to try WebRTC
- Consists of a server and client part that you can host yourself
- Also comes in modules if you just want some parts of it
- The code above is all you need to get this working
- Pretty simple, right?
