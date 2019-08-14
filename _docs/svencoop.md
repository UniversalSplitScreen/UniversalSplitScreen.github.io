---
title: Sven Co-op
permalink: /docs/guides/svencoop/
---

## Universal Split Screen setup
1. Install and run Universal Split Screen: see the [quick start guide](https://universalsplitscreen.github.io/docs/quickstart/).

1. In options, load the GoldSrc Engine preset.

1. Go back to the Current window tab.

## Half Life setup
1. Open the Sven Co-op directory by right-clicking Sven Co-op in Steam -> Properties -> Local files -> Browse game files...

1. Launch svencoop.exe as many times as you need.
     * GoldSrc Engine games will usually not let you launch more than one instance. In Universal Split Screen, alt-tab into Sven Co-op so the window is selected, then click 'Unlock'. The handle name should have been automatically filled with `LauncherMutex` when you loaded the preset.

1. Go to Options -> Mouse. Set Raw mouse input to **disabled**.

1. On the first instance, go to Start New Game. In the Server tab, select `-sp_campaign_portal` as the map. In the Game tab, make sure LAN Game is enabled.

1. In all instances, at the main menu, use the ` (tilde) key to open the console. This key is usually above the tab key.

1. Type `connect 127.0.0.1` and click Submit.

1. You should now be connected to the same game.

## Tips before you start
* If you have inconsistent mouse movement, especially when moving multiple mice, make sure the polling rates on your mice are set as low as possible. You can usually set this in your mouse configuration program (look on the manufacturer's website).

* Disable steam overlay by right-clicking Sven Co-op in Steam -> Properties and un-check 'Enable the Steam Overlay while in-game'

## Split screen setup
1. Install and run Universal Split Screen: see the [quick start guide](https://universalsplitscreen.github.io/docs/quickstart/)

1. In options, load the GoldSrc Engine preset (if you have not already done so).

1. Go back to the Current window tab. Alt+tab into the first instance. Set the mouse and keyboard. Repeat for the other instances.

1. Click Start split screen. You should now be able to play. Press End to stop.
