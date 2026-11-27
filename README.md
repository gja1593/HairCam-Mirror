[README.txt](https://github.com/user-attachments/files/35492069/README.txt)
HairCam Mirror — free iPhone-to-iPad live haircut mirror

WHAT IT DOES
- iPhone uses its front/ rear camera and generates a 12-character private connection code.
- iPad connects to that camera, shows live video, mirror flip, flashlight, and zoom.
- There is no subscription, microphone capture, recording, or account in the app.
- Built with WebRTC and the free PeerJS Cloud for signaling (the initial connection handshake).

IMPORTANT: The HTML file must be served from an HTTPS site for iPhone camera access.
You cannot rely on opening this file directly in Safari from the Files app.

FREE HOSTING USING GITHUB PAGES
1. Create a free GitHub account if you do not have one.
2. Create a NEW PUBLIC repository named haircam-mirror.
3. Upload index.html to the root of that repository.
4. Open the repository Settings > Pages.
5. Under Build and deployment, choose "Deploy from a branch", branch main, folder /(root), then Save.
6. Open https://YOUR-GITHUB-USERNAME.github.io/haircam-mirror/ in Safari on BOTH iPhone and iPad.
7. On iPhone choose Use as camera > Start camera > Allow.
8. Use Share viewing link to open it on the iPad, or type the 12-character code into the iPad.
9. On iPad choose Use as mirror > Connect to iPhone (if the link does not open the viewer automatically).
10. Adjust Mirror and Zoom.

PRACTICAL TIPS
- Start iPhone first; keep Safari open and keep the iPhone unlocked.
- Connect both devices to the same Wi-Fi network for the best chance of low latency.
- Strong lighting helps the camera maintain a clear image.
- Test hand-to-screen delay before using clippers near your head.
- Secure any wall arm properly in a wall stud or appropriate anchors.
- The initial handshake requires internet; video usually travels directly between devices,
  but network restrictions may prevent connection in some environments.

PRIVACY / LIMITATIONS
- The site source code is public if hosted on GitHub Pages with a free GitHub account;
  your private live video is NOT posted to GitHub.
- PeerJS Cloud handles signaling to establish the call. Video is encrypted with WebRTC.
- Anyone who has your currently active 12-character room code can attempt to connect;
  keep the link private. Generate a fresh code each time you start the camera.
- WebRTC may not connect on every network. No TURN relay is supplied by this example.
- The app has not been tested on your exact iPhone/iPad models.
