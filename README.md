# Preface
These modded files are all approved by Little Orbit and cannot and will not get your account suspended as of the time of writing this. If that ever changes this page, and the config itself, will be updated to reflect that. However, keep in mind that I take no responsibility for any harm caused to your account, your game or your software/hardware as a result of using these files. This config is still on a 'use at your own risk' basis. 

***You've been warned.***

Additionally, please read everything thoroughly before asking questions as I've done my best to be as thorough as possible and to answer almost any possible situation/outcome in this document. But if you are truly stumped, or you wish to report an issue, feel free to contact me on my [Discord server](https://discord.com/invite/MeMDVmj).

# Basics
Go into the `APB Reloaded\Binaries` folder and create a shortuct of `APB.exe` to your desktop. The executable may appear as only `APB` or `APB.exe` depending on your Windows settings but this does not matter. Next you will need to `right click` -> `Properties` on the newly created desktop shortcut and input the launch arugments you wish to use into the `Target` field.

If you open the default APB launcher, most of your modded files will be automatically replaced with the vanilla ones, thus we must launch the game directly from the shortcut when using configs. Whenever a patch comes out for the game you must launch the default APB launcher, let it update, then close the launcher, reinstall your desired configs and launch the game from the `APB.exe` desktop shortcut.

If you ever mess anything up or you want to revert *everything* to vanilla and start over, simply open the default APB launcher, click `Options` -> `Repair` and wait for it to finish. Once that is done you may close the launcher and start over with modding your game.

# Installation
Most of the configs are very simple to install, simply drag and drop the folders into your APB Reloaded main directory and replace everything when prompted to.

For example, if you wish to install my graphics, simply open the `Graphics` folder and drag and drop `APBGame` into your own APB Reloaded main directory where your own `APBGame` folder is located but ***NOT inside `APBGame` itself!*** If Windows prompts you to replace files then you're doing it right. If not, check whether you are placing the files in the correct directory.

Some configs may require further setup and those will be covered further below.

# Launch arguments
+ `-language=1031` - Sets game to load with custom localization (must use for localization).
+ `-nomovies` / `-nomoviesstartup` - Removes loading screens.
+ `-nosplash` - Removes initial splash screen upon boot. (Easy Anti-Cheat splash screen cannot be hidden.)
+ `-nosteam` - Disables Steam integration, including the Steam auto-login.

Example correct Target field path:

`"C:\Program Files (x86)\Steam\steamapps\common\APB Reloaded\Binaries\APB.exe" -language=1031 -nomovies -nosplash`

> [!CAUTION]
> Be sure to add a space after the quotations and before the dash, as well as between each launch argument as shown in the example!

# List of all features
### Audio
+ Ambient Sounds - Removes a large majority of ambient sounds which are not needed for gameplay purposes, including music coming from cars and Joker Ammo Vending Machine voice lines.
+ Dialogue - Removes all speech and screams from your character and other NPCs, including contacts speech.
+ RTW Vegas Sound - Replaces the Patriot Vegas G20 and 4x4 sounds with the old [RTW Vegas sounds](https://youtu.be/tAJi1-57qLU?t=79) and leaves all other sounds vanilla. Bishada sounds not included.

### Features
+ FPS Unlock + DTS + GC - FPS Uncap + Disabled Texture Streaming + Garbage Collection variants. More details below.
+ Keybinds - Adds several new bindable keybinds in the in-game controls menu that you can change on the fly including auto sprint, hold crouch, abandon mission, etc. More details below.
+ Login Screen - Sets login screen to a black scene with no music, making the game load significantly faster.
+ VivoxVoiceService Removal - Blanks the Vivox.exe file causing it to not load, fixes Steam sometimes getting stuck on APB due to Vivox not closing.
+ Muzzle Flash + Ragdolls - Muzzle Flash on/off + Ragdolls on/off variants.

### Interface
+ Faster UI ([Preview](https://i.imgur.com/nSbbnRr.jpg)) - Helps to reduce stuttering when changing loadout. Includes an additional variant - "White Mission Timer" (buggy and not recommended).
+ Localization
+ Notifications - Removes the district notification popups on the left of the screen for bounty, medals etc.

### Visuals
+ Graphics
+ Black Sky - Includes regular Black Sky and Black Sky Full Bright. Social is always full bright regardless of variant.
+ Bloom - There are no files for this, its explained further down in this document.

# Graphics presets

The following are all contained in a single file and can be changed from the in-game Video options:
+ Minimal - The main, Standard preset: High quality characters, cars, symbols, weapons, grenade/OPGL/rocket smoke is clearly visible, fences and doors are see-through. Transparent mission description and spawn screen. Everything else is lowest possible quality. Fog off but can be turned on from the Advanced tab in-game.
+ Low - Same as Standard but with lowest particles meaning no bullet holes, but also no fire from burning vehicles.
+ Medium - Low Poly: Everything is low polygon. Character, car and weapon texture quality is kept high so you can see designs. Fences and doors are see-through, grenade/OPGL/rocket smoke is visible. Transparent mission description and spawn screen. Fog off but can be turned on from the Advanced tab in-game.
+ High - Same as Low Poly but with lowest particles meaning no bullet holes, but also no fire from burning vehicles.
+ Maximum - Max graphics preset for highest quality with no regard for FPS, mainly used for screenshots and videos but can be played with on high-end systems.

> [!NOTE]
> You may swap between Minimal-Low and Medium-High seamlessly without needing to restart, but if you go from standard to low poly or vice versa, you would need to restart. You can also enable shadows on any of the presets by simply enabling "Dynamic Shadows" in the Advanced tab. The same applies for Double Buffering if you wish to use it.

# Localization
`Localization` refers to the textual changes to the HUD/UI. This localization file set is designed with simplicity in mind as it strips away the dated, long-winded, orange walls of text the game is plagued by with short and concise messages, coupled with more pleasant and less dated colors. It comes in several color presets:

![localization color presets](https://i.imgur.com/jsbdUv9.png)

>[!CAUTION]
>Please note that in order for the localization to work, you need to add the `-language=1031` launch argument to your APB.exe desktop shortcut's `Target` field as described above!

### Key features of this localization
+ Missions that are usually avoided by players now have their names in full bright red so that you know to abandon quickly.
+ Simplifies the overall interface, giving maximum information while remaining compact and much easier to read with just a quick glance compared to vanilla UI.
+ Enhances and recolors text and makes everything look much cleaner, nicer and easier on the eyes allowing you to focus more on the actual game.
+ Included is a variant of rooq and lazer's mission stages config with timers and other extras.

### Slash command changes
+ `/exit` -> `/q`
+ `/abandonmission` -> `/a`
+ `/dance` variants without the word dance -> `/urban`, `/michael,`, `/techno`, etc
+ `/strikeapose1`, `/strikeapose2` -> `/pose1`, `/pose2`
+ `/groupinvitemodedefault` -> `/gimd` (When not in a group type, `/gimd true` to allow all members of group to be able to invite everytime)

### Optional addon: Shortened Chat Channels 
Changes the chat channels from whole words to abbreviations. Works with any localization variant, just make sure to drag and drop it *after* the main localization file set. 

<details>
  <summary>Click here to preview the shortened chat channels</summary>
  
![shortened chat channels](https://i.imgur.com/NAfIVNl.png)

</details>

### Optional Vanilla addon: Mission Stages only
This is for those who want to keep the game's vanilla localization but want to see the mission stages in the description box which is normally present in any of the full localization variants. Simply only copy this and follow the rest of the steps for the APB.exe shortcut creation like you would with the full localization.

***You are free to edit this localization as you desire for personal use, however if you wish to build your own and use mine as a base and distribute it publicly, please credit me for making the base for it.***

# FPS Unlock + DTS + GC
This does a few things all at once (+/- 32GB RAM):
- Uncaps your fps to infinite.
- Disabled Texture Streaming (DTS) - Universal FPS boost without any loss of graphics quality.
- Changes the "Smooth Frame Rate" setting in the in-game Video options to cap your fps at 128 which is the highest you can go without your character randomly sliding. Useful for precision weapons such as the HVR.
- Garbage Collection (GC) - Additional feature which turns off GC, which will completely eliminate the stutters that occur every 60 seconds.

> [!CAUTION]
> Removing GC will prevent you from using any customization kiosks in the Social district. Swapping between "DTS only" and DTS + GC is the only way to customize your character currently if you wish to keep GC off. You have to restart the game every time you swap them. For casual players who only wish to uncap their FPS and gain a performance boost, simply use "DTS only".

# Muzzle Flash + Ragdolls
Both of these entirely different configs are located within the same file (`DefaultGame.ini`) and so I've added multiple variants to pick from.

### Muzzle Flash
Turn off/on the weapon muzzle flash and bullet casings.

### Ragdolls
Either remove all ragdolls or NPC (civilian) ragdolls only. Helps with visibility and could help with performance slightly on some systems.

> [!NOTE]
> My personal recommendation is to remove NPC ragdolls only and keep player ones. Reason is that if you remove player ragdolls, upon death your camera freezes in place and does not track the player who killed you, making it harder for you to see where they are going and give information to your teammates. This is especially true if they run out of your camera's field of view or run behind an object.

# Keybinds
This new config adds a variety of new easily rebindable keys within the in-game controls settings, while still keeping all the old ones fully intact, allowing you to switch them on the fly. These are unbound by default so once you install this and launch your game, you will have to manually bind them to whatever you wish personally.
+ Auto-Sprint (Movement) - Bind it to Shift to get the classic auto-sprint like before. Holding Shift + W will make you jog like it did previously.
+ Hold Crouch (Movement) - Added new hold crouch method which prevents you from getting stuck in crouch (highly recommended). The old 'stuckable' method is also still present for those who prefer it but it is now labeled "Crouch (Hold) [Classic]". Simply bind your crouch button to either one.
+ Abandon Mission (Interface) - Allows you to directly abandon missions with a keybind without having to type anything in chat.
+ Hold Lean (Combat) - Hold key to lean instead of toggle while aiming down the sights.
+ Primary/Secondary weapon (Combat) - Switch to primary or secondary weapon without cycling through to the next weapon upon pressing the key multiple times.
+ Social Designers Anywhere (Interface) - Allows you to access the Wardrobe, Persona, Garage, Music Studio and Symbol designers from anywhere within the Social district, without having to go up to the actual kiosks. Only works in the Social district.
+ In-game music player volume up/down hotkeys (Music).
+ Camera look up/down hotkeys (Camera).

***Also with this installed, Alt + F4 finally works now, over a decade later. However it doesn't work in the character selection screen for now. But it works pretty much everywhere else.***

# Black Sky

Black sky comes in 4 variants. The "No Weather" variants get rid of the greenish tint and give more color/vibrance to the whole game.

<details>
  <summary>Click here to see the differences</summary>
  
![black sky](https://i.imgur.com/lTxUUt6.png)
![black sky no weather](https://i.imgur.com/xpJsdPD.png)
![black sky fullbright](https://i.imgur.com/36PfzHD.png)
![black sky fullbright no weather](https://i.imgur.com/4777H8X.png)

</details>

# Bloom

If you wish to disable the actual effects of bloom in-game but retain the blurry transparent background in the inventory/loadout menus, simply navigate to `APB Reloaded\Engine\Config\BaseEngine.ini`, find `DefaultPostProcessName=APBPostEffectMaterials.APBPostEffect_Process` and add ; in front of it like so: `;DefaultPostProcessName=APBPostEffectMaterials.APBPostEffect_Process` then save the file. I recommend doing this only after you've installed any of the DTS variants as those replace BaseEngine.ini, assuming you wish to use a DTS config (but it is not required for this to work).

Once that's done simply open the game and enable Bloom from the Video > Advanced settings.

# Disabling UI elements

You can follow lazer's guide to disabling UI elements [here](https://github.com/lvzxr/apb-reloaded/blob/main/UI.md).

# Credits, Links and Special Thanks

### Massive thanks to the following:
+ Secrets and the rest of the APB dev team who actively work with us to improve the game both on vanilla level as well as on configs level.
+ lazer - Audio, Graphics optimizations, Engine Fonts, Localization, Faster UI/White Mission Timer, Texture Streaming, Keybinds
+ rooq - Engine Fonts, Localization, General assistance
+ Esurient - Engine Fonts, Localization, Faster UI/White Mission Timer
+ mewpri - Black Sky, Keybinds
+ Kyouki - Stutter Fix, Ambient Sounds, General assistance
+ ApollyoNite aka Ryderizm - RTW Vegas Sounds
+ jmilos - Texture Streaming, Keybinds
+ Leefekyn - Localization (killfeed stun icon)
+ Tobii & Dopefish - For placing some of the foundations for modding APB many years ago, before leaving for greener pastures. ([Tobii's APB repository, mostly outdated now.](https://apb.zone/))

You can find me on [Twitch](https://www.twitch.tv/flvws), [YouTube](https://www.youtube.com/c/FlawsAPB) and [Discord](https://discord.com/invite/MeMDVmj), as well as find my [APB Beginner's Guide](https://steamcommunity.com/sharedfiles/filedetails/?id=1445306227).

You can download the Advanced APB Launcher from Little Orbit's official link [here](https://media.gamersfirst.com/gamersmedia/apb/Advanced_APB_Launcher.zip).

You can also find lazer's config on his [GitHub Page](https://github.com/lvzxr/apb-reloaded).
