# Preface
The modified files in this config are all safe to use and have been approved directly by Little Orbit staff and will not get your account suspended. If that ever changes the config will be updated to reflect it. That being said — keep in mind that I take no responsibility for any harm caused to your account, your game, your software/hardware or any other negative consequences as a result of using these files. Modding live service games is on a ***'use at your own risk'*** basis.

There is plenty of fearmongering going around in the community about configs resulting in account suspensions. If you're worried about that you can find the official configs/mods rules on [this blog post from Little Orbit](https://www.gamersfirst.com/apb/news/2024/8/14/sard-faq). This was posted when the SARD anti-cheat was being implemented but despite the fact that we've now moved over to GFAC, the rules are exactly the same. GFAC is Little Orbit/GamersFirst's own proprietary anti-cheat and as such they have full control over what is allowed and what isn't.

Many of the edits present in these files are not my own discovery/creation and as such credit is given where credit is due at the bottom of this page. This config is meant to serve as a one stop shop for everyone who wishes to mod APB within the boundaries of the Little Orbit Terms of Service without fear of suspension or other negative outcomes.

Many things have changed or are no longer allowed post-APB 1.31 'New Horizon' and as such those files are no longer distributed/supported here. Please read everything thoroughly first and if you wish to ask a question or report an issue, feel free to post about it on my [discord server](https://discord.com/invite/MeMDVmj).

> [!IMPORTANT]
> **It is super strongly recommended that you only download the newest and latest release version as I ensure those are always safe and most functional with the most amount of features. I take no responsibility for damages in case you download and use an old version. Those are only there for archiving purposes.**

> [!NOTE]
> ### Regarding the 'incorrect' usage of GitHub
> I am fully aware that the way I upload my config to GitHub is technically incorrect but the reason I made the choice to keep it like this is to make it less confusing for the average, everyday user who might not be familiar with all the modding/config and github ('nerd') stuff. For the average person who might be new to modding, it's far easier to simply download a zip file that has all the files they need instead of having to navigate folders on GitHub to figure out which files they need to download, how to download them and so on. This keeps it more accessible and easier for just about anyone to download and use the files without much stress.

# Setup & Basics
First, you need to do the following steps regardless of which configs you're going to use:

1. Navigate to `APB Reloaded\Binaries` and create a shortuct of `APB` or `APB.exe` (depending on your Windows settings) to your desktop.
2. Right click -> Properties on the newly created desktop shortcut and input the [launch arguments](https://github.com/flawsv/apb?tab=readme-ov-file#launch-arguments) you wish to use into the `Target` field.

From now on you must launch your game through this new desktop shortcut in order for the configs to work.

> [!IMPORTANT]
> Whenever a game update comes out you must open the default APB launcher, let it update, then close the launcher, reinstall your desired configs and launch the game from your desktop shortcut. Do NOT create new APB shortcuts every time there is an update, it is unnecessary. Creating a shortcut of APB.exe is a single-time thing, you DON'T need to re-do it for updates/patches.

> [!NOTE]
> In order to revert everything back to vanilla and start over, open the default APB launcher, click Options -> Repair and let it finish. Once that is done you may close the launcher and start over with modding your game.

# Installation
Drag and drop the folders into your APB Reloaded main directory and replace everything when prompted to.

For example, if you wish to install my graphics open the `Graphics` folder and drag and drop the `APBGame` folder into your own APB Reloaded main directory where your own `APBGame` folder is located but ***NOT inside `APBGame` itself!*** If Windows prompts you to replace files then you're doing it right. If not, check whether you are placing the files in the correct directory.

The only config that requires one additional step is localization because you need to add the `-language=1031` launch argument to your shortcut in case you haven't already done that.

# Launch arguments
+ `-language=1031` - Sets game to load with custom localization (required for localization).
+ `-nomovies` / `-nomoviesstartup` - Removes loading screens.
+ `-nosplash` - Removes initial splash screen upon boot (GFAC logo cannot be removed).
+ `-nosteam` - Disables Steam integration, including Steam auto-login.

<details>
  <summary>Click here for an image example of launch arguments</summary>
  
![targetfield](https://i.imgur.com/o0vQdAr.png)

</details>


Example correct Target field path: <br >
`"C:\Program Files (x86)\Steam\steamapps\common\APB Reloaded\Binaries\APB.exe" -language=1031 -nomovies -nosplash`
> [!CAUTION]
> Be sure to add a space after the quotations and before the dash, as well as between each launch argument as shown in the examples.

# Features
+ FPS Unlock + Login Screen + DTS + GC — Multiple game performance-enhancing edits that do not affect the game's visuals.
+ Keybinds — Adds several new keybinds to the in-game controls menu that you can change on the fly including auto sprint and hold crouch.
+ Muzzle Flash — Ragdolls - Muzzle Flash on/off and Ragdolls on/off.
+ Localization — Textual changes to the HUD/UI.
+ Graphics — Visual changes/optimizations and visibility improvements.
+ Transparent UI — Makes the entire UI slightly transparent and also gets rid of the black background when you are in the loadout menu so you can see what is going on around you while you're swapping loadouts.

More details regarding each of these further down.

# Graphics presets

The following are all contained in a single file and can be changed from the in-game Video options by changing the quality preset:
+ Minimal (Standard) — High quality player characters and cars, symbols and weapons. Grenade/OPGL/rocket smoke is clearly visible, fences and doors are see-through. Transparent mission description and respawn screen.
+ Low — Same as Minimal but with lowest particles meaning no bullet holes, but also no fire from burning vehicles.
+ Medium (Low poly) — Low poly models. Player characters, cars and weapon textures quality is kept high so you can see designs. Fences and doors are see-through, grenade/OPGL/rocket smoke is visible. Transparent mission description and respawn screen.
+ High — Same as Medium but with lowest particles meaning no bullet holes, but also no fire from burning vehicles.
+ Maximum — Max graphics preset for highest quality with no regard for FPS, mainly used for screenshots and videos.

> [!NOTE]
> You may swap between the Minimal-Low and Medium-High presets seamlessly without needing to restart, but if you go from standard to low poly or vice versa, you would need to restart. You can also enable shadows on any of the presets by simply enabling "Dynamic Shadows" in the Advanced tab, as well as Double Buffering and Fog.

# Localization
Localization simplifies the overall interface and changes text colors in the HUD/UI so you can focus more on the game while still providing you with all the vital information on screen. Included is a variant of rooq and lazer's mission stages config with stage timers and other extras. It comes in several color presets:
<details>
  <summary>Click here to preview the color presets</summary>

  ![localization color presets](https://i.imgur.com/jsbdUv9.png)

</details>

### This localization changes the following /slash commands
+ `/exit` -> `/q`
+ `/abandonmission` -> `/a` (obsolete)
+ `/dance` variants without the word dance -> `/urban`, `/michael,`, `/techno`, etc
+ `/strikeapose1`, `/strikeapose2` -> `/pose1`, `/pose2`
+ `/groupinvitemodedefault` -> `/gimd` (When not in a group type, `/gimd true` to allow all members of group to be able to invite everytime)

>[!IMPORTANT]
>Please note that in order for the localization to work, you need to add the `-language=1031` launch argument to your APB.exe desktop shortcut's `Target` field as mentioned previously.

> [!CAUTION]
> **Remember to always wipe the entire GER folder first when updating localization or switching between different localizations, otherwise certain inconsistencies might occur. Not all localizations edit all the same files therefore weird mix-ups can occur.**

>[!NOTE]
>You are free to edit this localization as you desire for personal use, however if you wish to build your own and use mine as a base and then distribute it publicly, please credit me for making the base for it.

# Optional addons for localization

## Shortened chat channels 
Changes the chat channels from whole words to abbreviations.

<details>
  <summary>Click here to preview the shortened chat channels</summary>
  
![shortened chat channels](https://i.imgur.com/NAfIVNl.png)

</details>

## Street names removal
Removes street names from the bottom right corner of the screen under the radar.
<details>
  <summary>Click here to preview the street names removal</summary>
  
![street names removal](https://i.imgur.com/ZQvV1q2.png)

</details>

## Weapon and Vehicle stats
Changes the in-game item description for every weapon and vehicle to show the exact stats of weapons and vehicles such as damage, effective range for weapons and top speed, health for vehicles.

<details>
  <summary>Click here to preview the Weapon/Vehicle stats</summary>
  
![stats](https://i.imgur.com/k1F9r1W.png)

</details>

## Equipment+stages in mission names
Changes mission titles to show the equipment required for the mission as well as the total number of stages and the final stage. Supports both Standard font as well as Engine font.

## Mission stages only (Vanilla localization)
This is for those who want to keep the game's vanilla localization but want to see the mission stages in the description box which is normally present in any of the full localization variants.

>[!IMPORTANT]
>These addons work with any localization. Make sure to only apply these AFTER you've applied your desired localization otherwise these addons will be overwritten. Even if you only use addons, you still need to add the `-language=1031` launch argument to your APB.exe desktop shortcut's `Target` field.

# FPS Unlock + Login Screen + DTS + GC
This does several things all at once (+/- 32GB RAM):
- Uncaps your FPS to infinite. If you wish to cap it: APB Reloaded\Engine\Config\BaseEngine.ini -> MaxClientFrameRate=0 ; simply change the 0 to your desired FPS cap.
- Disabled Texture Streaming (DTS) — Universal FPS boost without any loss of graphics quality.
- Changes the "Smooth Frame Rate" setting in the in-game Video options to cap your fps at 128 which is the game's default fps cap.
- Garbage Collection (GC) Removal<sup>1</sup> — Additional feature which turns off GC, which will completely eliminate the stutters that occur every 60 seconds.
- Black Login Screen<sup>2</sup> — Changes the login screen and character select screen to a black background with no music and makes the game load faster.

> [!CAUTION]
> **(1)** Using the 'No GC' variant will prevent you from using any customization kiosks in the Social district. Swapping between 'DTS only' and 'DTS + No GC' is the only way to customize your character currently if you wish to keep GC off. You have to restart the game every time you swap them. For those who only wish to uncap their FPS and gain a performance boost, simply use 'DTS only'.

> [!CAUTION]
> **(2)** Using 'Black Login Screen' will prevent you from creating new characters due to the new login screen config method breaking the character creator screen. The old method is no longer allowed and there is no way to solve this issue while using this method. As such, if you need to make a new character use 'Vanilla Login Screen' to create it and once you're done, you may swap back to 'Black Login Screen'. I apologise for the inconvenience but there is no easier way to do it for now.

> [!NOTE]
> **If you wish to undo some of the individual changes I've made, please refer to the [file changes breakdown](https://github.com/flawsv/apb/blob/main/filechangesbreakdown.md#file-changes-breakdown) document and edit the settings to your liking.**

# Muzzle Flash + Ragdolls

### Muzzle Flash
Turn off/on the weapon muzzle flash and bullet casings.

### Ragdolls
Either remove all ragdolls or NPC (civilian) ragdolls only. Helps with visibility and could help with performance slightly on some systems.

> [!NOTE]
> My personal recommendation is to remove NPC ragdolls only and keep player ones. Reason is that if you remove player ragdolls, upon death your camera freezes in place and does not track the player who killed you, making it harder for you to see where they are going and give information to your teammates. This is especially true if they run out of your camera's field of view or run behind an object, such as a building.

> [!NOTE]
> Refer to the [file changes breakdown](https://github.com/flawsv/apb/blob/main/filechangesbreakdown.md#file-changes-breakdown) document if you wish to adjust these to your liking.

# Keybinds
This file adds a variety of new easily rebindable keys within the in-game controls settings, while still keeping all the old ones fully intact, allowing you to switch them on the fly. These are unbound by default so once you install this and launch your game, you will have to manually bind them to whatever you wish personally.
+ Auto-Sprint (Movement) — Bind it to Shift to get the classic auto-sprint like before. Holding Shift + W will make you jog like it did previously.
+ Hold Crouch (Movement) — Added new hold crouch method which prevents you from getting stuck in crouch (highly recommended). The old 'stuckable' method is also still present for those who prefer it but it is now labeled "Crouch (Hold) [Classic]". Simply bind your crouch button to either one.
+ Abandon Mission (Interface) — Allows you to directly abandon missions with a keybind without having to type anything in chat. Button is still there and it *works* but it can't be used anywhere anymore.
+ Hold Lean (Combat) — Hold key to lean instead of toggle while aiming down the sights.
+ Primary/Secondary weapon (Combat) — Switch to primary or secondary weapon without cycling through to the next weapon upon pressing the key multiple times.
+ Social Designers Anywhere (Interface) — Allows you to access the Wardrobe, Persona, Garage, Music Studio and Symbol designers from anywhere within the Social district, without having to go up to the actual kiosks. Only works in the Social district.
+ In-game music player volume up/down hotkeys (Music).
+ Camera look up/down hotkeys (Camera).

> [!NOTE]
>Also with this installed, Alt + F4 finally works now, over a decade later. However it doesn't work in the character selection screen for now. But it works pretty much everywhere else.

# Transparent UI

This makes the entire UI slightly transparent across the board and also gets rid of the black overlay/background when you are in the inventory/loadout menu so you can see what is going on around you while you're swapping loadouts. It can also be adjusted to your liking to become even more transparent by editing the file yourself. The file is DefaultUI.ini and the line is "OverlaySceneAlphaModulation=0.999" where the value goes from 0 to 1, so to really adjust it you need to do 0.XX, 0.XXX or 0.XXXX and so on. I personally found that 0.999 is the least intrusive while still getting the job done.

<details>
  <summary>Click here to preview Transparent UI</summary>
  
![transparent ui](https://i.imgur.com/lTJSGBc.png)
![transparent ui2](https://i.imgur.com/0pmQk5y.png)

</details>

There is only one minor issue with this change and thats the Joker Tickets and APB$ icons disappearing in the inventory menu

![missing icons](https://i.imgur.com/w8LlXkb.png)

# Disabling UI elements

You can follow lazer's guide to disabling UI elements [here](https://github.com/lvzxr/apb-reloaded/blob/main/UI.md).

# Credits, Links and Special Thanks

### Massive thanks to the following:
+ The APB dev team who've actively worked with us to improve the game both on vanilla level as well as on configs level.
+ lazer — Additional graphics optimizations, Engine Fonts, Localization, Texture Streaming, Keybinds
+ rooq — Engine Fonts, Localization, General assistance
+ Esurient — Engine Fonts, Localization
+ mewpri — Keybinds, Localization (Weapon & Vehicle stats); Check out his localization generator which was used to create the weapon and vehicle stats [here](https://mew.re/config/).
+ Kyouki — No GC/Stutter Fix, General assistance
+ jmilos — Texture Streaming, Keybinds, New hold crouch method, New black login screen method
+ Leefekyn — Localization (killfeed stun icon)
+ Tobii & Dopefish — For placing some of the foundations for modding APB many years ago, before leaving for greener pastures.

You can find me on [Twitch](https://www.twitch.tv/flvws), [YouTube](https://www.youtube.com/c/FlawsAPB) and [Discord](https://discord.com/invite/MeMDVmj), as well as find my [APB Beginner's Guide](https://steamcommunity.com/sharedfiles/filedetails/?id=1445306227).

You can download the Advanced APB Launcher from Little Orbit's official link [here](https://media.gamersfirst.com/gamersmedia/apb/Advanced_APB_Launcher.zip).

You can also find lazer's config on his [GitHub Page](https://github.com/lvzxr/apb-reloaded).
