##  What about security?

#### <span class="highlight">Media is fully encrypted between peers using DTLS-SRTP</span>

note:
- A very common question when talking about WebRTC is security. Well, I can
  assure you that according to the spec, WebRTC MUST implement DTLS-SRTP.
- This means that the key exchange takes place in the media plane, which
  doesn't require the cryptographic parameters to leak into the SDP which are
  sent via the signalling server
- For you this means that WebRTC is by default end-to-end encrypted
