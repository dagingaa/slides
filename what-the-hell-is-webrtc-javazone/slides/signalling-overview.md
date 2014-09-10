![JSEP architecture](img/jsep.png)

<small>Source: <a href="http://www.html5rocks.com/en/tutorials/webrtc/infrastructure/">html5rocks.com</a></small>

note:
- As you can see, we have a middle man that relays the initial connection
  messages, called the signalling server, which accepts messages from the apps
  themselves
- The app then relays the session description down to the browser layer through
  the setDescription functions
- The browser layer then does a lot of connection magic, and media eventually
  flows between the browsers
- The browser then exposes the MediaStream object, which the application can show in the GUI
- However....
