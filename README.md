# STATIC BELOW - game downloads

A two-player co-op horror game for Windows. Chapter One, *Kestrel Ridge*: two contractors, a dead
relay station, a storm at 02:13, and an intercom that already knows what you are going to say.

This repository only hosts the packaged builds. The source code lives in a separate private repository.

## Install

1. Download **[StaticBelowLauncher.exe](https://github.com/mniklas189-png/static-below-releases/releases/latest/download/StaticBelowLauncher.exe)**
   (about 250 KB) and run it.
2. Windows SmartScreen may show *"Windows protected your PC"* because the launcher is not code-signed.
   Click **More info**, then **Run anyway**.
3. Click **INSTALL**. The game (about 550 MB download, 690 MB on disk) goes into
   `%LOCALAPPDATA%\Programs\Static Below`. You can choose another folder under **MORE**. No
   administrator rights are needed.
4. Click **PLAY**. The launcher can also add desktop and Start menu shortcuts.

## What the launcher does

- **Checks for updates** every time it starts, or when you click CHECK FOR UPDATES. Both players need
  the same build to play together, and the launcher keeps you on the latest one.
- **Updates** by downloading the new build, checking its SHA-256 checksum, and only then replacing
  the old files. If something goes wrong, your installed build stays as it was. Interrupted downloads
  resume where they stopped.
- **VERIFY FILES** checks every installed file against the release. **REPAIR** reinstalls if anything
  is damaged.
- **Online relay** status shows whether the co-op relay is reachable. The launcher also writes the
  relay address into the game.
- **Updates itself** when a newer launcher is published.
- **MORE**:
  - open the game or log folder
  - change the install folder
  - create shortcuts
  - uninstall (your settings stay in `%LOCALAPPDATA%\StaticBelow`)

Everything is downloaded over HTTPS from this repository's releases. The launcher and the game never
ask for any account, and the game opens no network ports.

## Playing together

One player hosts and reads the six-character room code to the other. Talk over a voice call;
the game has no voice chat. Controls are in the game's menu and in `PLAYERS_README.txt` in the game
folder.

## Requirements

Windows 10 or 11 (64-bit) and a DirectX 12 graphics card. It was tested on an RTX 4070 with an i7-11700F.

## Credits and licences

Built with Unreal Engine 5.8. Surface textures are CC0 from Poly Haven. Epic template characters and
animations are used under the Unreal Engine EULA. Fonts are Apache 2.0. Everything else was made
for the game. The full list is in `CREDITS.md` in the game folder.
