---
title: Borderlands 3
permalink: /docs/guides/borderlands3/
---

This guide has been written by [/u/TerrawattSurge](https://www.reddit.com/user/TerrawattSurge). See the original post [here](https://www.reddit.com/r/localmultiplayergames/comments/daal6l/howto_borderlands_3_splitscreen_pc_tutorial/).

This guide is for multiple gamepads only. You may wish to experiment with the settings in Universal Split Screen to make multiple keyboards and mice possible.

![Borderlands 3 Split Screen](https://i.redd.it/fgiffsd1usu31.png)

## Setup:

1. Download Sandboxie and install https://www.sandboxie.com/DownloadSandboxie

1. Run Sandboxie and create a new sandbox called "BL3"

1. Go to BL3 sandbox settings, Resource Access, File Access, Full Access, and add `C:/` drive

1. Download WASP.dll from [here](https://github.com/UniversalSplitScreen/UniversalSplitScreenScripts/blob/master/Scripts/Borderlands3/Modules/WASP/WASP.dll) and save it to \Documents\WindowsPowershell\Modules\WASP\WASP.dll

1. Copy the Split Screen script from [here]( https://raw.githubusercontent.com/UniversalSplitScreen/UniversalSplitScreenScripts/master/Scripts/Borderlands3/Borderlands3_SplitScreen.ps1) into Powershell ISE (or your favourite editor) and edit the variables at the top to match your setup

1. Save the script to `\Documents\WindowsPowershell\Scripts\Borderlands3_SplitScreen.ps1`

1. Open Powershell and enable running of scripts using the following command, and press A at the prompt to enable 
`Set-ExecutionPolicy RemoteSigned`

## Procedure:

1. Hide the task bar. In Windows10, right click on the taskbar and go to 'Taskbar Settings', then enable 'Automatically hide the taskbar in desktop mode'

1. Launch Powershell and run the script (don't forget the `.\` before the script to tell it to execute). 
`.\Documents\WindowsPowershell\Scripts\Borderlands3_SplitScreen.ps1`

1. If you want to swap position of the windows or change to a vertical split, alt+tab back to Powershell and follow the on screen instructions

1. In Universal Split Screen, go to the Options tab and disable 'Draw mouse' on the left and enable 'Hook XInput for gamepads' if you are using controllers

1. Select the first instance of Borderlands 3 then Alt+tab back to Universal Split Screen and switch to the 'Current Window' tab. Make sure in the 'Window Title' box it shows 'Borderlands® 3' and change the controller index to 1 (this instance of the game is the 'online' instance)

1. Select the second instance of Borderlands 3 and Alt+tab back to Universal Split Screen and make sure in the 'Window Title' box it shows '[#] Borderlands® 3 [#]', then change the controller index to 2

1. Press 'Start Split Screen'

1. In game, change your group settings to 'LAN Play' on both windows

1. In one of the windows, go to the Social Menu, select LAN Browser and select the game to join

1. Happy Vault Hunting!

** There are a few limitations with this method. If anyone figures out a way to overcome them, let me know. **

* Only one window is 'online', so some functions are only available in that window. In the title menu, the online window will have a scrolling news feed, while the offline windows will just show the Borderlands 3 logo. In the screenshot attached, the bottom window is online

* The profile is shared between both characters, so cosmetic items are stored only for the person that closes the game last. I suggest giving trinkets and skins to the person playing on the online window to unlock and make sure to quit the offline window first.

* The bank is only saved for the online window, so if you want to store something, give it to the person playing on the online window to store. Next time you start the game, the offline player will have the same items as the online player in their bank.

* Guardian ranks are only saved for the online window. Whatever upgrades you choose for the online window will be loaded for the offline window next time you start the game.

* The offline window cannot use 'weapon pack' weapons, or DLC skins or trinkets

* Audio isn't always in sync, so you may want to turn down the dialogue volume on one of the windows

* Settings are shared between both players on startup, but can be tweaked when in the game

* Weapon skins and characters aren't shown correctly in the title menu (see screenshot)

* The two instances of Borderlands3 don't share CPU resources equally, so I've added a section in the script to change processor affinity to assign unique processor cores to each window

* I have included code for dual monitors, but it is still a bit buggy so might not work for everyone

* Check out https://borderlands.com/en-US/news/2019-09-18-borderlands-3-troubleshooting-optimization-guide/ for general Borderlands 3 issues and how to fix them


If you have any comments, please leave them on the [original guide post](https://www.reddit.com/r/localmultiplayergames/comments/daal6l/howto_borderlands_3_splitscreen_pc_tutorial/).
