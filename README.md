# RunBack 19

One more game.

RunBack 19 is a Windows launcher for the NBA Live 19 mod project. It brings the mascot roster, shootaround courts, and local 1v1 practice into one place.

- **Mascots:** Stuff, Champ, The Coyote, Burnie, Harry the Hawk, G-Wiz, The Gorilla, and Franklin.
- **Courts:** Rucker Park, Dyckman Park, VH Headquarters, Venice Beach, Hoop Dome, Margaret Hie Ding Lin Park, Kezar Pavilion, and Barry Farms.
- **Local 1v1:** CPU selection, 15/21-point rules, make-it-take-it, scoreboard and 24-second shot clock. The running pause menu applies to 1v1; shootaround stays pausable.
- **Builds:** Read created-player slots and use Max out build or the separate Unlock all action for shared animations and clothing. Save edits create backups and require the game to be closed.
- **Jumpshot landings:** Choose a landing in Animations, then pull the left stick toward you through the shot landing. A green release is not required.
- **Shot speed:** In Shots, R1/RB selects Quick (1.15x); L1/LB restores Normal (1.00x).
- **Custom gear:** Ushanka over the basic CAP headband, Rick-style low-tops over black canvas Converse, and pink/chrome Raf Ozweego over brown leather Converse.
- **Game Files:** Select your NBA Live 19 directory, compare files with the signed RunBack 19 release, and repair outdated shared mod files.
- **Updates:** Check and download launcher and shared game-content updates from GitHub Releases.

## Status

**[Download RunBack 19 v0.4.0](https://github.com/RunBack19dev/Runback-Launcher/releases/tag/v0.4.0)**. This release adds VH Headquarters and custom gear, and includes the current black/purple launcher and local 1v1 changes. VH Headquarters replaces the Terminal 23 slot. The final Earth correction removes geometry beneath the playing surface; its in-game visual check remains pending.

**[Download the separate online test kit](https://github.com/RunBack19dev/Runback-Launcher/releases/download/v0.4.0/RunBack19-Online-Test-Kit-v0.4.0.zip)**. Both PCs need the matching RunBack 19 content and the [community NBA19 Online v2.3 client](https://github.com/danilenko22/nba19-online-servidor/releases/tag/v2.3). Read the kit's README before launching. The native test route is Live Run 3v3; shared friend 1v1 is unverified. Searching failures, re-entry crashes and online mascot visibility remain under investigation. The kit includes the updated connection report tool and a separate native crash-trace helper.

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

## Asset credit

“Ushanka - Trapper Hat” by [PeteDeee / vileguypete](https://sketchfab.com/vileguypete), [source model](https://sketchfab.com/3d-models/ushanka-trapper-hat-1046cd56a67d4b79902e47aa0daf3ccb), licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Adapted for native RunBack geometry, fitting records and rebaked textures. Attribution is included in the setup and online kit.
