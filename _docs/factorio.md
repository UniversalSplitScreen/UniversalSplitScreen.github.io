---
title: Factorio
permalink: /docs/guides/factorio/
---

## Factorio setup
1. You will need to install Factorio 0.17 first. On Steam, right click Factorio -> Properties -> Betas -> Select `0.17.x - Latest 0.17 Experimental`.
	Alternatively you can download the 0.17 version from the Factorio website. (You can do this even if you bought the game on Steam. You will need to register an account in-game).

1. For the Steam version, you will need to replace steam_api64.dll in the Factorio/bin/x64 directory with steam_api64.dll from the Goldberg Emulator. Rename the original steam_api64.dll to steam_api64.dll.original (or something) so you can use it later if needed. Download Goldberg [here](https://gitlab.com/Mr_Goldberg/goldberg_emulator/releases). On Steam, open the Factorio directory by right clicking Factorio -> Properties -> Local files -> Browse local files...

1. Open `Factorio\config-path.cfg`. Make sure the first line is `config-path=__PATH__system-write-data__/config`. If it is not, place a single hashtag # before the line and add it after. It should look like this:
	```
	#config-path=__PATH__executable__/../../config
	config-path=__PATH__system-write-data__/config
	```

	 * This will change your save directory. You may want to move your saves from `Factorio\saves` to `%APPDATA%\Factorio\saves`

1. Download the script files [here](https://github.com/UniversalSplitScreen/UniversalSplitScreenScripts/raw/master/Scripts/Factorio/Factorio_Universal_Split_Screen_Scripts.zip) and extract them into the `Factorio\bin\x64` folder.

1. Run the first instance by running SplitScreen1.bat. This first instance will be able to load your existing save games. Launch the other instances with SplitScreen2.bat, SplitScreen3.bat, etc.

1. Host a game on the first instance by going to Play -> Multiplayer -> Host new game or Host saved game. Make sure `Public` and `Steam` are disabled. Enable `LAN` and Disable `Verify user identity`. You can choose any username you like.

1. On the other instances, go to Play -> Multiplayer -> Play on LAN and select the game. You should now be in the same game.

## Split screen setup
1. Install and run Universal Split Screen: see the [Quick Start guide](https://universalsplitscreen.github.io/docs/quickstart/).

1. In options, load the Factorio preset.

1. Go back to the Current window tab. Alt+tab into the first instance. Set the mouse and keyboard. Repeat for the other instances.

1. You can optionally use Toggle window borders to trim the window borders.

1. Click Start split screen. You should now be able to play. Press End to stop.

1. The Alt key and mouse scrollwheels are ignored by Factorio in the current version of Universal Split Screen. You may wish to remap the controls for zooming and alt-mode.
