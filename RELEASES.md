# Publishing a RunBack 19 update

The owner prepares a release from the current working game installation in the launcher's Updates tab. A single version covers the launcher and all shared mod content.

1. Choose a numeric version that has never been published before, such as `0.1.2`.
2. Enter the release notes and choose **Prepare release**. Select an output folder outside the game folder.
3. Preparation hashes every game file. It includes changed game files automatically and reuses verified payload URLs for unchanged files from the previous release. The first release includes patches for all five existing modified game files, including Head 1. Game payloads contain compressed changed-byte ranges; full game archives are not distributed. Changed existing files need a supported original backup in the publisher's local baseline configuration.
4. Create a GitHub Release with the matching tag, for example `v0.1.2`.
5. Upload **all** generated `rb19-*.bin` parts, `latest.json`, `latest.json.sig`, and `RELEASE_NOTES.txt`. These are the public update assets. Do not upload signing keys or local settings.
6. Review the release and publish it as the latest stable release. Keep earlier releases available because later manifests can reuse their unchanged payloads.
7. In RunBack 19, check for updates and verify the release version before downloading.

Version 0.3.0 is the current release, combining the dashboard, Builds tools, trait fixes, jumpshot landings, and shot-speed controls with the existing shared game mods. Keep v0.1.0 available because its unchanged anim.big and graphics_demo.big patch payloads are reused. Earlier repair fixes are retained. Friend joining/P2P is still in development. File checks use the signed canonical manifest, and repair downloads reconstruct supported original game files into verified RunBack 19 versions.

## Applying an update

Players use **Updates → Check for updates → Download update → Apply & restart**. To repair the current game installation, use **Game Files → Update / repair** (a scan is optional).

The installer verifies the release signature, verifies downloaded parts and complete files, waits for the launcher to exit normally, and requires the game to be closed before replacing game files. It keeps backups and a transaction record under the launcher folder. Replacement failures roll back game files and installation metadata.

The public release manifest lists downloadable shared mods and the launcher. Local texture exports, backup archives, and other files without an update payload do not block repair. The publisher keeps its broader source inventory locally to detect future changes.

**Updates → Launcher only** can download a launcher hotfix before a game folder is chosen or repaired.

Player saves and local folder choices are separate from the shared game installation.

## Publisher key

The private signing key stays encrypted with Windows DPAPI on the publisher's PC. Keep a secure backup of the publisher account/profile. Losing access to this key requires a planned key transition; never post it in this repository or a release.
