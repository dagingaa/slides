##  RTCPeerConnection

````javascript
var pc = new RTCPeerConnection();
pc.onaddstream = function(obj) {
    var vid = document.createElement("video");
    document.appendChild(vid);
    vid.srcObject = obj.stream;
}

pc.addStream(localVideoStream);

pc.createOffer(function (offer) { ... }
pc.createAnswer(function (answer) { ... }

pc.setLocalDescription(...)
pc.setRemoteDescription(...)

pc.close();
````

note:
- But this is just a small part of webrtc, the really interesting stuff is the peer connection
- Everything revolves around the RTCPeerConnection object
- Not gonna go through everything

