![Turn diagram](img/turn.png)

<small>Source: <a href="http://www.html5rocks.com/en/tutorials/webrtc/infrastructure/">html5rocks.com</a></small>

note:
- You have your two peers behind each of their own NATs
- They broker the connection through your signalling server, and use your STUN
  server to try and poke a hole in the NAT
- If that fails, they will transfer the media through one or several TURN
  servers at your disposal
- There are several services that offer TURN-as-a-Service out there if you
  don't want to host it yourself
- But if you are just starting out and want to experiment...
