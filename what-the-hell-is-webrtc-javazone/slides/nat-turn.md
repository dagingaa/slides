## But it's not always that easy...

<h1>
<span class="fragment">NAT</span> <span class="fragment">+ TURN</span> <span class="fragment">= <span class="highlight-alt">❤</span></span>
</h1>

<small class="fragment highlight">About 15% of connections needs TURN</small>

note:
- However, it's not always that easy...
- You see, we live in a world of NAT
- The NAT is great, it translates your external IP into several local IPs, but it's a fiend of p2p communication
- You can try to get around it using STUN to find the external ip, and find
  ways around it, but sometimes, even that doesn't work
- THis is where TURN comes in
- TURN is Traversal using relays around NAT, so TURN is a media relay, that
  acts as a third aprty, which both parties connect to
- One party uploads their video, and the other party downloads
- TURN also means a worse user experience, because it introduces latency
- The good part is that only around 15% of connections require TURN (actual numbers)
- So you end up with an architecture like this
