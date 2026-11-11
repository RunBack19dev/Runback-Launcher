# RunBack 19

One more game.

RunBack 19 is a Windows launcher for the NBA Live 19 mod project. It brings the mascot roster, shootaround courts, and local 1v1 practice into one place.

- **Mascots:** Stuff, Champ, The Coyote, Burnie, Harry the Hawk, G-Wiz, The Gorilla, and Franklin.
- **Courts:** Rucker Park, Dyckman Park, Terminal 23, Venice Beach, Hoop Dome, Margaret Hie Ding Lin Park, Kezar Pavilion, and Barry Farms.
- **1v1 practice:** Start or return to shootaround through the in-game pause menu. Includes the live scoreboard and 24-second shot clock.
- **Game Files:** Select your NBA Live 19 directory, compare files with the signed RunBack 19 release, and repair outdated shared mod files.
- **Updates:** Check and download launcher and shared game-content updates from GitHub Releases.

## Status

Version 0.1.0 is being prepared. The redesigned launcher and update engine have been built and tested locally. Initial game-content download assets are not published yet. Friend connections, full team assignment, and selectable 15/21 finish rules are still in development.

## Installation

Use the files attached to a published release. Open RunBack 19, select your NBA Live 19 folder in **Game Files**, and choose your shadPS4 executable in **Settings**. The game folder must contain `eboot.bin` and the BIG archives.

Updates use a signed release manifest and SHA-256 file checks. Changed files are backed up before replacement. Close the game normally before applying a game-content update.

Your personal player saves and local paths stay on your PC. Shared releases carry the project's game modifications for everyone.

## Release hosting

The launcher checks this address:

`https://github.com/RunBack19dev/Runback-Launcher/releases/latest/download/latest.json`

Each public update needs `latest.json`, `latest.json.sig`, and every payload referenced by that manifest. Keep the publisher signing key private; it is never part of a download.
