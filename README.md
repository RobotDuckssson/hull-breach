# Hull Breach

A 3D space shooter in a single HTML file. You stand on a grated turret platform high above a giant starship, holding a cannon in each hand, and blast incoming asteroids before they breach your hull.

## Play

Open `index.html` in a browser, or upload it to any web host. No build step. The page loads three.js and its fonts from public CDNs, so it needs an internet connection.

## Controls

| Action | Desktop | Touch | VR |
| --- | --- | --- | --- |
| Aim | Move the mouse | Drag a finger | Point the controllers |
| Fire | Hold click or Space | Hold your finger down | Pull the trigger |
| Look around | Cursor to a screen edge, or WASD / arrow keys | Drag to the screen edge | Turn your head |
| End run | Esc or the End run button | End run button | Squeeze the grip |
| Mute | M or the Sound button | Sound button | — |

## Rules

- Big rocks take 4 hits and split into shards.
- Shoot the cyan crystals to repair your hull.
- Shoot the glowing green supply crates to upgrade your cannons: Standard → Rapid → Spread → Nova. Any hit drops you back to Standard.
- Quick kills in a row build a score multiplier up to ×5.
- Each wave brings faster, more frequent rocks.
- Your best score is saved in your own browser.

## VR

VR uses WebXR and only works when the page is served over **https**. Open it in the headset's browser (for example on Meta Quest) and press **Enter VR**.

## Deploy

Every push to `main` uploads the game to <https://anderssons.info/hull-breach/> through the workflow in `.github/workflows/deploy.yml`. It connects to `ssh.anderssons.info` as `anderssons.info` and needs one repository secret, `SFTP_PASSWORD`, set in the one.com Control Panel.
