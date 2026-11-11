# RunBack 19

One more game.

RunBack 19 is a Windows launcher for the NBA Live 19 mod project. It brings the mascot roster, shootaround courts, and local 1v1 practice into one place.

- **Mascots:** Stuff, Champ, The Coyote, Burnie, Harry the Hawk, G-Wiz, The Gorilla, and Franklin.
- **Courts:** Rucker Park, Dyckman Park, Terminal 23, Venice Beach, Hoop Dome, Margaret Hie Ding Lin Park, Kezar Pavilion, and Barry Farms.
- **1v1 practice:** Start or return to shootaround through the in-game pause menu. Includes the live scoreboard and 24-second shot clock.
- **Builds:** Read created-player slots and use Max out build or the separate Unlock all action for shared animations and clothing. Save edits create backups and require the game to be closed.
- **Jumpshot landings:** Choose a landing in Animations, then pull the left stick toward you through the shot landing. A green release is not required.
- **Shot speed:** In Shots, R1/RB selects Quick (1.10x); L1/LB restores Normal (1.00x).
- **Game Files:** Select your NBA Live 19 directory, compare files with the signed RunBack 19 release, and repair outdated shared mod files.
- **Updates:** Check and download launcher and shared game-content updates from GitHub Releases.

## Status

**[Download RunBack 19 v0.3.0](https://github.com/RunBack19dev/Runback-Launcher/releases/tag/v0.3.0)**. This version adds the redesigned dashboard, Builds tools, Gold traits and trait slots, the Jumpshot Landing menu, and the Quick/Normal shot-speed selector. All eight mascots, eight courts, the shared Head 1 appearance, CPU 1v1, scoreboard, and 24-second shot clock are retained.

This release brings testers onto the same game files before networking work. Friend joining and P2P are not enabled yet. Full team assignment and 15/21 finish rules remain in development. Menu clothing clipping and some landing previews still need work; the Quick selector and its revised position need wider gameplay testing.

Existing users can use **Updates → Check for updates → Download update → Apply & restart**, with the game closed, then **Game Files → Update / repair** if needed. You can also extract the new setup over the existing launcher folder while the launcher is closed; keep the existing Backups folder so later patches can reuse your original files.

## Installation

Download and extract **RunBack19-Setup.zip** from the release. Open RunBack 19, select your NBA Live 19 folder in **Game Files**, and choose your shadPS4 executable in **Settings**. The game folder must contain `eboot.bin` and the BIG archives. Close the game, then use **Game Files → Update / repair**. A scan is optional.

If upgrading from 0.1.0 and repair is disabled or mentions `generic001_head_col.gnf`, close RunBack 19 and extract the new **RunBack19-Setup.zip** over the existing launcher folder. Reopen it and run Update / repair.

Game patches require a supported original NBA Live 19 installation. Existing updater backups are checked automatically for later updates. The launcher reports an unsupported original instead of applying a patch to a different file.

Updates use a signed release manifest and SHA-256 file checks. Changed files are backed up before replacement. Close the game normally before applying a game-content update.

Your personal player saves and local paths stay on your PC. Shared releases carry the project's game modifications for everyone.

## Release hosting

The launcher checks this address:

`https://github.com/RunBack19dev/Runback-Launcher/releases/latest/download/latest.json`

Each public update needs `latest.json`, `latest.json.sig`, and every payload referenced by that manifest. Keep the publisher signing key private; it is never part of a download.
