##  Caller and Callee

<pre><code class="javascript">// Caller
pc.createOffer(function(offer) {
    pc.setLocalDescription(new RTCSessionDescription(offer), function() {
        // send the offer to a server to be forwarded to the friend you're
        // calling.
        }, error);
}, error);
</code></pre>

<pre><code class="javascript">// Callee
var offer = getOfferFromFriend();
pc.setRemoteDescription(new RTCSessionDescription(offer), function() {
    pc.createAnswer(function(answer) {
        pc.setLocalDescription(new RTCSessionDescription(answer), function(){
            // send the answer to a server to be forwarded back to the caller
            }, error);
        }, error);
    }, error);
}
</code></pre>

<pre><code class="javascript">// Caller
var offer = getResponseFromFriend();
pc.setRemoteDescription(new RTCSessionDescription(offer), function() { },
error);
</code></pre>

note:
    Put your speaker notes here.
    You can see them pressing 's'.
