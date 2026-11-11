# RunBack 19

One more game.

RunBack 19 is a Windows launcher for the NBA Live 19 mod project. It brings the mascot roster, shootaround courts, and local 1v1 practice into one place.

- **Mascots:** Stuff, Champ, The Coyote, Burnie, Harry the Hawk, G-Wiz, The Gorilla, and Franklin.
- **Courts:** Rucker Park, Dyckman Park, Terminal 23, Venice Beach, Hoop Dome, Margaret Hie Ding Lin Park, Kezar Pavilion, and Barry Farms.
- **1v1 practice:** Start or return to shootaround through the in-game pause menu. Includes the live scoreboard and 24-second shot clock.
- **Game Files:** Select your NBA Live 19 directory, compare files with the signed RunBack 19 release, and repair outdated shared mod files.
- **Updates:** Check and download launcher and shared game-content updates from GitHub Releases.

## Status

**[Download RunBack 19 v0.1.2](https://github.com/RunBack19dev/Runback-Launcher/releases/tag/v0.1.2)** is available. The release contains the launcher and about 210 MB of game modification patches, including the shared Head 1 appearance. Friend connections, full team assignment, and selectable 15/21 finish rules are still in development.

Version 0.1.2 adds the red VH RunBack 19 Windows app icon. Existing users can get it through **Updates → Launcher only**.

The included 0.1.1 fixes address game repair being disabled and the false requirement for local texture exports. The five existing game-mod patches are retained unchanged.

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
