# ATF Harvest Blocker Mod

A mod for blocking harvest (in-game currency) gain in [After the Fall VR](https://www.afterthefall-vr.com/).

## What does this do?
Blocks all harvest additions to your harvest balance in the game. You’ll still see a harvest amount pop up on screen, however harvest won’t actually be added to your total. 

## Why block harvest gain?
This mod helps users who accidentally received excessive harvest from hackers. It allows players to reduce their balance by buying/recycling weapons and blocking harvest gain from recycling, thus removing unwanted 'free harvest' effectively.

## How to Reduce Harvest Balance
After installing the mod, go to the Armory. Buy guns and recycle them using the recycler machine to lower your balance. Normally, recycling refunds harvest, but this mod blocks the refund, allowing you to repeat the process until your balance is at the desired level. Adding attachments to weapons can further reduce your balance.

TIP: Combat Devices, like Sawblade Devices (costing 250,000 each), are the fastest way to spend harvest. Attach them to your wrist, use the drill from the bench to scrap them, and repeat. The mod blocks the usual refund, making it effective for reducing your balance.

Once finished, uninstall the mod to resume normal gameplay and harvest gain.

# Installation & Usage

## Compatibility
This mod is designed to work with version ***1.9.41947*** of After the Fall, aka the **'Nightfall Update'**. It is compatible and tested with the PCVR (Steam and Rift) versions of the game. It cannot be used with Meta Quest, Pico, or PSVR versions, unfortunately.

## Requirements
- **BepInEx 6.0.0-pre1**  
  This mod was built and tested with **BepInEx 6.0.0-pre1**. Other versions of BepInEx may not work correctly.

## Installation
1. Install **BepInEx 6.0.0-pre1**:
   - If you don’t already have it, grab the correct version of BepInEx from [the official BepInEx GitHub](https://github.com/BepInEx/BepInEx).
   - The version needed is: [BepInEx_UnityIL2CPP_x64_6.0.0-pre.1.zip](https://github.com/BepInEx/BepInEx/releases/download/v6.0.0-pre.1/BepInEx_UnityIL2CPP_x64_6.0.0-pre.1.zip)
   - Download it and extract the .zip to your After the Fall Game Folder.

2. Install the Mod:
   - Grab the latest `ATFHarvestBlocker-vx.x.x.zip` from the [Releases](https://github.com/Dteyn/ATFHarvestBlocker/releases) section of this repository.
   - Open the .zip and copy `BepInEx` to your After the Fall Game Folder:
     - Steam default location: `C:\Program Files (x86)\Steam\steamapps\common\After The Fall\`
	 - Rift default location: `C:\Program Files\Oculus\Software\Software\vertigo-games-snowbreed\`
   - You should now have `BepInEx\plugins\ATFHarvestBlocker.dll` in your game folder. The mod is now installed.

3. Launch the Game:
   - Start the game, and BepInEx will automatically load the mod.
   - NOTE: It is normal for the game to take a bit longer to start the first time as BepInEx does some background setup work.

## How to Uninstall
- Simply delete `ATFHarvestBlocker.dll` from the `BepInEx/plugins` folder, if you wish to leave BepInEx installed to use with other mods.
- OR you can disable BepInEx from loading by editing `doorstop_config.ini` and setting `enabled` to `false`, and change back to true if you want to re-enable the mod.
- OR you can completely remove everything and revert to 100% vanilla ATF by deleting these folders and files: `BepInEx` folder, `mono` folder, `doorstop_config.ini` file, `winhttp.dll` file, and `changelog.txt` file.

## Troubleshooting
If you run into any troubles, you can check two log files for information:
1. BepInEx `LogOutput.log` file:
   This is the first place to check for issues. You can find this in the After the Fall Game Folder, at `BepInEx\LogOutput.log`. If the `LogOutput.log` file doesn't exist, it means BepInEx is not installed correctly (see step 1 above).

2. After the Fall `Player.log` file:
   This is the game's Unity Engine log file and contains a lot of detailed information. The default location is: `C:\Users\YOUR_USERNAME\AppData\LocalLow\Vertigo Games\AfterTheFall`. Inside this folder are the last two log files, saved as `Player.log` and `Player-prev.log`. These can provide valuable insights.

You may also want to enable the BepInEx logging console which is disabled by default in version 6.0.0-pre1. The console displays logging in real-time as the game is running. To do so, you can edit `BepInEx\config\BepInEx.cfg` and find [Logging.Console] section and change Enabled to true.
   
## Known Issues
- This mod doesn’t stop the harvest gain notifications from showing on-screen - just the actual addition to your total. The harvest notifications on screen are simply a cosmetic leftover.

## Disclaimer
IMPORTANT: You’re modding at your own risk! Mods can cause unexpected behavior, crashes, or other issues. Be sure to back up your game files before installing any mods. I’m not responsible if something goes wrong, but I’ll do my best to help if you run into trouble.

## Feedback
Have questions, issues, or suggestions? Drop by the [Issues](https://github.com/Dteyn/ATFHarvestBlocker/issues) section of this repo. I’ll do my best to help when I can. You can also find me on the [After the Fall Discord Server](https://discord.gg/afterthefall).

## Shout-Outs
Be sure to check out my buddy [Astienth's VR mods](https://github.com/Astienth?tab=repositories)! He makes a ton of mods for flat2VR games, as well as bHaptics and ProVolver, including a [bHaptics Mod for After the Fall](https://github.com/Astienth/AftertheFall_bHaptics) and [ProVolver Mod for After the Fall](https://github.com/Astienth/AfterTheFall_Provolver). Check them out! :)
