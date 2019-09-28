---
title: Endless Space
permalink: /docs/guides/endlessspace/
---

This guide has been written by [Raepyrem](https://github.com/Raepyrem). See the original post [here](https://github.com/UniversalSplitScreen/UniversalSplitScreen/issues/15).

Please be aware there may be issues with save corruption: see [here](https://github.com/UniversalSplitScreen/UniversalSplitScreen/issues/15#issuecomment-534693140). Make sure to save frequently.

## Setup
1. #### Install the Goldberg Emulator

  1. Open the Endless Space directory by right-clicking Endless Space in Steam -> Properties -> Local files -> Browse local files.

  1. Create a text file called steam_appid.txt. Inside it, write `208140`. Save and exit.

  1. Rename `steam_api.dll` to `steam_api.dll.valve`.

  1. Download the latest release of the Goldberg Emulator [here](https://gitlab.com/Mr_Goldberg/goldberg_emulator/-/releases). The Goldberg Emulator is required to connect two or more instances together.

  1. Extract it anywhere by right-clicking -> Extract all...

  1. Copy the steam_api.dll from the Goldberg directory to the Endless Space directory.

1. Launch desired number of instances by running EndlessSpace.exe. Make sure to start each instance with different Steam IDs via the Goldberg tab under "Utilities" in the Universal Split Screen tool. (ie launch one instance, change the Steam ID, and repeat).
  * You may wish to experiment with the `AppData and user folder switch` option in Universal Split Screen to easily launch multiple instances.


3. The `Enable window resizing` option works, but you have to enable it multiple times for each and every adjustment you make. (`Toggle window borders` works when it feels like it.)

## Starting the game:
1. Select "New Game" from the main menu, and to the right under "Sessions" change "Single only" to either "(X) Multiplayer" option: You will see an error when you do this; ignore it and select "Continue Playing" (This error also shows up when loading multiplayer saves; ignore those also). After the error displays, return to the main menu.

1. Repeat the beginning of step 1 twice. After the third attempt in total, a new error will display; ignore this one also. Loading saves follows this same process.
(What you're looking for is the second error message that has "Steam ID" near the end of the first line.)

1. To the top left, under "Galaxy", change "Empires" to your desired number of Human and AI players.

1. Configure other match rules, and you're ready on this end.

1. #### Connecting Players:
  1. Select "Join Game" and wait for the host's game to show up.

  1. Select it and then select "Join" on the lower right.

  1. Choose/create your factions, confirm match rules, and select "Ready"
After everyone is ready, the host selects "Start Game".

5. (Optional) Have fun!

## Universal Split Screen Setup
1. Install Universal Split Screen: see the [quick start guide](https://universalsplitscreen.github.io/docs/quickstart/).
1. Download the config [here](https://raw.githubusercontent.com/UniversalSplitScreen/UniversalSplitScreenScripts/master/Configs/EndlessSpace/Endless%20Space.json). You may need to right-click and `Save page as`. Save it in the Config folder inside Universal Split Screen.
1. Run Universal Split Screen. In options, load the Endless Space config.
1. Go back to the Current window tab. Alt+tab into the first instance. Set the mouse and keyboard. Repeat for the other instances.
1. Click Start split screen. You should now be able to play. Press End to stop.

## Config options
The config is available [here](https://raw.githubusercontent.com/UniversalSplitScreen/UniversalSplitScreenScripts/master/Configs/EndlessSpace/Endless%20Space.json).
![Endless Space Options](https://raw.githubusercontent.com/UniversalSplitScreen/UniversalSplitScreen.github.io/master/img/endless_space_options.png)
