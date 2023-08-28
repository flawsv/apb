# Preface
These modded files are all approved by Little Orbit and cannot and will not get your account suspended as of the time of writing this. If that ever changes this page, and the config itself, will be updated to reflect that. However, keep in mind that I take no responsibility for any harm caused to your account, your game or your software/hardware as a result of using these files. This config is still on a 'use at your own risk' basis. ***Be warned.***

Additionally, please read everything thoroughly before asking questions as I've done my best to be as thorough as possible and to answer almost any possible situation/outcome in this document. But if you are truly stumped, or you wish to report an issue, feel free to contact me on my [Discord server](https://discord.com/invite/MeMDVmj).

# Basics
Go into the `APB Reloaded\Binaries` folder and create a shortuct of `APB.exe` to your desktop. The executable may appear as only `APB` or `APB.exe` depending on your Windows settings but this does not matter. Next you will need to `right click` -> `Properties` on the newly created shortcut and input the launch arugments you wish to use into the `Target` field.

If you open the default APB launcher, most of your modded files will be automatically replaced with the vanilla ones, thus we must launch the game directly from the shortcut when using configs.

If you ever mess anything up or you want to revert *everything* to vanilla and start over, simply open the default APB launcher, click `Options` -> `Repair` and wait for it to finish. Once that is done you may close the launcher and start over with modding your game.

***Whenever a patch comes out for the game you must launch the default APB launcher, let it update, then close the launcher, reinstall your desired configs and launch the game from the `APB.exe` shortcut.***

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

***Make sure to add a space after the quotations and before the dash, also add a space between each launch argument as shown in the example!***

# List of all features
### Audio
+ Ambient Sounds - Removes a large majority of ambient sounds which are not needed for gameplay purposes, including music coming from cars and Joker Ammo Vending Machine voice lines.
+ Dialogue - Removes all speech and screams from your character and other NPCs, including contacts speech.
+ RTW Vegas Sound - Replaces the Patriot Vegas G20 and 4x4 sounds with the old [RTW Vegas sounds](https://youtu.be/tAJi1-57qLU?t=79) and leaves all other sounds vanilla. Bishada sounds not included.

### Features
+ Stutter Fix - Removal of APB's Garbage Collection 60 seconds timer. Please read further below on how to use this.
+ Disable Texture Streaming (FPS Boost)* - Free FPS boost on most systems without any visual differences. Please read further below on how to use this.
+ FPS Unlock - Allows you to either increase the game's FPS cap or unlock it to infinity. Smooth Frame Rate is also changed to 128fps when enabled in-game in each of the presets. ***Ignore if using Disable Texture Streaming (FPS Boost) OR Stutter Fix***
+ Keybinds - Adds several new bindable keybinds in the in-game controls menu that you can change on the fly including auto sprint, hold crouch, abandon mission, etc. More details below.
+ Login Screen - Sets login screen to a black scene with no music, making the game load significantly faster. Still allows character creation.
+ Disable VivoxVoiceService - Blanks the Vivox.exe file causing it to not load, fixes Steam sometimes getting stuck on APB due to Vivox not closing.
+ Muzzle Flash + Ragdolls + Audio Emitters - Several different configs that are all located in one file, thus having to add many different variants. More details below.

### Interface
+ Faster UI ([Preview](https://i.imgur.com/nSbbnRr.jpg)) - Changes what file the UI is to read from causing there to be parking signs throughout the inventory, can help to improve fps when changing mods quickly. Includes an additional variant - "White Mission Timer" (buggy and not recommended). ***Only pick one variant at a time!***
+ Localization
+ Notifications - Removes the district notification popups on the left of the screen for bounty, medals etc.

### Visuals
+ Graphics

# Graphics presets
+ Minimal - The main, Standard preset: High quality characters, cars, symbols, weapons, grenade/OPGL/rocket smoke is clearly visible, fences and doors are see-through. Transparent mission description and spawn screen. Everything else is lowest possible quality. Fog off but can be turned on from the Advanced tab in-game.
+ Low - Same as Standard but with lowest particles meaning no bullet holes, but also no fire from burning vehicles.
+ Medium - Low Poly: Everything is low polygon. Character, car and weapon texture quality is kept high so you can see designs. Fences and doors are see-through, grenade/OPGL/rocket smoke is visible. Transparent mission description and spawn screen. Fog off but can be turned on from the Advanced tab in-game.
+ High - Same as Low Poly but with lowest particles meaning no bullet holes, but also no fire from burning vehicles.
+ Maximum - Max graphics preset for highest quality with no regard for FPS, mainly used for screenshots and videos but can be played with on high-end systems.

***You may swap between Minimal-Low and Medium-High seamlessly without needing to restart, but if you go from standard to low poly or vice versa, you would need to restart.***

***You can also enable shadows on any of the presets by simply enabling "Dynamic Shadows" in the Advanced tab. The same applies for Double Buffering if you wish to use it.***

***If you are using either "Disabled Texture Streaming" OR "Stutter Fix", you can enable Bloom from the in-game settings as the actual "bloom" effect has been removed in those files, but the loadout/inventory menus will have a transparent, blurry background so you can see around you while changing loadouts.***

# Localization
`Localization` refers to the textual changes to the HUD/UI. This localization file set is designed with simplicity in mind as it strips away the dated, long-winded, orange walls of text the game is plagued by with short and concise messages, coupled with more pleasant and less dated colors. It comes in [several color presets](https://imgur.com/a/iy1z5zw).

***Please note that in order for the localization to load, you need to add the `-language=1031` launch argument to your APB.exe desktop shortcut's `Target` field as described above!***

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
Changes the chat channels from whole words to abbreviations. Works with any localization variant, just make sure to drag and drop it *after* the main localization file set. [Preview](https://imgur.com/a/KIrj2KN).

### Optional Vanilla addon: Mission Stages only
This is for those who want to keep the game's vanilla localization but want to see the mission stages in the description box which is normally present in any of the full localization variants. Simply only copy this and follow the rest of the steps for the APB.exe shortcut creation like you would with the full localization.


***You are free to edit this localization as you desire for personal use, however if you wish to build your own and use mine as a base and distribute it publicly, please credit me for making the base for it.***

# Disable Texture Streaming (FPS Boost)
In simple terms this disables the game's ability to smoothly transition between LOD states as it can cause slowdowns, increasing FPS on most systems. However, this can only be used on systems with at least 16GB RAM, otherwise it will cause game crashing.

***Do NOT use this with `FPS Unlock` as it edits the same file and this will unlock your FPS to infinite anyway, as well as set Smooth Frame Rate to 128fps when enabled in the in-game video settings.***

FPS gained may vary from system to system. This can also be coupled with enabling Double Buffering from the in-game Video settings -> Advanced for even higher FPS but it can add input lag to your game. Input lag added from Double Buffering varies from system to system and tolerance for it varies from person to person so you can try it and decide for yourself.

# Muzzle Flash + Ragdolls + Audio Emitters
All three of these entirely different configs are located within the same file (`DefaultGame.ini`) and so I've added many different variants for everyone to pick from. ***Only pick 1 at a time!***

### Muzzle Flash
Simply turn off/on the weapon muzzle flash and bullet casings like we could before through UPK file edits.

### Ragdolls
Either remove all ragdolls or NPC (civilian) ragdolls only. Helps with visibility and could help with performance slightly on some systems.

***My personal recommendation is to remove NPC ragdolls only and keep player ones. Reason is that if you remove player ragdolls, upon death your camera freezes in place and does not track the player who killed you, making it harder for you to see where they are going and give information to your teammates. This is especially true if they run out of your camera's field of view or run behind an object.***

### Audio Emitters
What this does it that it sets priorties of emitters and NPCs to 1 so they are only played when really close to you, this also has the effect of making them quieter. Highly recommend that you use this if you're using the ambient sounds removal to make the environment as quiet as possible.

# Keybinds
This new config adds a variety of new easily rebindable keys within the in-game controls settings, while still keeping all the old ones fully intact, allowing you to switch them on the fly. These are unbound by default so once you install this and launch your game, you will have to manually bind them to whatever you wish personally.
+ Auto-Sprint (Movement) - Bind it to Shift to get the classic auto-sprint like before. Holding Shift + W will make you jog like it did previously.
+ Hold Crouch (Movement) - Bind it to your crouch key to get the classic hold crouch like before. ***Beware the 'stuck in crouch' glitch when you press your jump key while holding crouch! To 'unstick' yourself, simply press the jump key again.***
+ Abandon Mission (Interface) - Allows you to directly abandon missions with a keybind without having to type anything in chat.
+ Hold Lean (Combat) - Hold key to lean instead of toggle while aiming down the sights.
+ Primary/Secondary weapon (Combat) - Switch to primary or secondary weapon without cycling through to the next weapon upon pressing the key multiple times.
+ Social Designers Anywhere (Interface) - Allows you to access the Wardrobe, Persona, Garage, Music Studio and Symbol designers from anywhere within the Social district, without having to go up to the actual kiosks. Only works in the Social district.
+ In-game music player volume up/down hotkeys (Music).
+ Camera look up/down hotkeys (Camera).

***Also with this installed, Alt + F4 finally works now, over a decade later. However it doesn't work in the character selection screen for now. But it works pretty much everywhere else.***

# Disabling UI elements

You can follow lazer's guide to disabling UI elements [here](https://github.com/lvzxr/apb-reloaded/blob/main/UI.md).

# ***[EXPERIMENTAL]*** Stutters Fix / Removal of Unreal Engine's Garbage Collection (GC) timer
### **[16GB+ RAM ONLY]**

In simplest terms this config by Kyouki should remove any stutters that occur in-game while you're playing missions or Fight Club caused by the game itself and should improve the overall performance of APB. Stutters in APB are caused by something called "Garbage Collection" (GC) which is a client side Unreal Engine system that APB relies on to not run out of memory and crash. This is normally on a 60 seconds timer and whenever it occurs it makes the game freeze/stutter. The stutter severity largely depends on the hardware the game is running on, particularly on CPU and hard drive speed. This is most often noticed whenever it occurs in fights, getting players killed. However, in recent times, APB devs have added an extra GC clear to occur on the respawn screen whenever you die which means that we can now afford to turn off the one that runs on a 60 seconds timer and play APB without it crashing within 20-30 minutes of gameplay.

### ***There is a downside to using this and that is the fact that, at least for now, designer kiosks (wardrobe, persona, etc) in Social do NOT work with this installed as they will load infinitely and softlock the game! This is intended for gameplay ONLY (missions/fight club), at least for now.***

The file also does other things such as disable texture streaming for a free FPS boost on almost any machine and several other misc back-end value adjustments to improve performance. This file does NOT affect the game visually and you will not see ANY visual difference so it can be used with any graphics including vanilla.

Please keep in mind that this file is EXPERIMENTAL as we are still testing it and while it does seem to work well for 95%+ of users so far, we may introduce adjustments or improvements in the future.

This file includes "Smooth Frame Rate" being set to 128fps in case you ever need to toggle it while in-game, to prevent character sliding.

### IMPORTANT
***Do **NOT** use this with "FPS Unlock" or "Disable Texture Streaming" files! This cannot be used in conjunction with those two!***

# Credits, Links and Special Thanks

### Massive thanks to the following:
+ Secrets and the rest of the APB dev team who actively work with us to improve the game both on vanilla level as well as on configs level.
+ lazer - Audio, Graphics optimizations, Engine Fonts, Localization, Faster UI/White Mission Timer, Texture Streaming, Keybinds
+ rooq - Engine Fonts, Localization, General assistance
+ Esurient - Engine Fonts, Localization, Faster UI/White Mission Timer
+ mewpri - Keybinds
+ Kyouki - Stutter Fix, Ambient Sounds, General assistance
+ ApollyoNite aka Ryderizm - RTW Vegas Sounds
+ jmilos - Texture Streaming, Keybinds
+ Leefekyn - Localization (killfeed stun icon)
+ Tobii & Dopefish - For placing some of the foundations for modding APB many years ago, before leaving for greener pastures. ([Tobii's APB repository, mostly outdated now.](https://apb.zone/))

You can find me on [Twitch](https://www.twitch.tv/flvws), [YouTube](https://www.youtube.com/c/FlawsAPB) and [Discord](https://discord.com/invite/MeMDVmj), as well as find my [APB Beginner's Guide](https://steamcommunity.com/sharedfiles/filedetails/?id=1445306227).

You can also find lazer's config on his [GitHub Page](https://github.com/lvzxr/apb-reloaded).
