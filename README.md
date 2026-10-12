# Nexus Studio: Early Access Preview

Nexus Studio is a free Windows editor for making small 3D games. You can create a project, build a scene, import assets, set up gameplay rules, play your game, save and reopen it, and export it as a single HTML file.

**Status: limited early-access preview, single-user, Windows only.** Nothing has been released here yet. When the preview is published, the installer and its SHA-256 checksum will appear under [Releases](../../releases).

This repository holds releases and bug reports only. It does not contain source code.

## About the installer
* The installer is **not code-signed**. Windows may show an "unknown publisher" warning. Compare the SHA-256 checksum of the file you downloaded with the one on the release page before you run it. Please do not turn off Windows Defender or SmartScreen.
* Tested on one Windows 11 PC plus automated smoke tests. Windows 10 has not been tested.
* The installer downloads the Microsoft Edge WebView2 runtime if it is missing, which needs an internet connection once.

## Privacy
Nexus Studio never uploads your projects and itself makes no network connections in this preview. The embedded Microsoft Edge WebView2 runtime may contact Microsoft services as part of normal operation. Your projects are stored in your Documents folder; if Windows syncs Documents to OneDrive, OneDrive will sync them.

## Known limitations (summary)
* **Collaboration is not included in this preview.**
* No user scripting; gameplay uses a rules system, a player controller and physics.
* Only `.glb` models import; one scene per project.
* Games over about 90 MB export as a folder instead of one HTML file; exports were verified only in Microsoft Edge.
* Uninstalling leaves one registry key behind.
* No auto-update.

## Report a problem
Open an issue with the **Bug report** template. In Nexus Studio open **Help, then About, then Copy diagnostics** and paste the result into the report. Nothing is sent automatically.
