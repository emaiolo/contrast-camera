CONTRAST CAMERA - TEST PROTOTYPE

WINDOWS PC: Test on your webcam
1. Save index.html in any folder.
2. Open it in Chrome or Edge. If the camera is blocked for a file:// page, use the localhost method below.
3. Press START CAMERA, allow access, adjust THRESHOLD and EDGE SENSITIVITY.

WINDOWS PC: Reliable localhost method (requires Python installed)
1. Open Command Prompt in the folder containing index.html.
2. Run: py -m http.server 8000
3. Open http://localhost:8000 in Chrome/Edge on the PC.

PIXEL 7: Phone camera requires a secure website
1. Sign into GitHub on the PC and make a new PUBLIC repository, for example contrast-camera.
2. Use Add file > Upload files, upload index.html, and commit.
3. Open repository Settings > Pages > Build and deployment, choose Deploy from a branch, branch main, folder /(root), and save.
4. Wait for the published HTTPS link, typically https://USERNAME.github.io/contrast-camera/.
5. On the Pixel 7, open the HTTPS link in Chrome, press START CAMERA, and allow camera permission.

Do not open http://PC_IP_ADDRESS:8000 on the phone. Non-HTTPS local network pages typically cannot request camera permission.

The page works offline after being loaded only while the browser retains its resources. Nothing is sent to a server by the page itself. Do not use for safety-critical navigation.
