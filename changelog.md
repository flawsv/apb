## v1.6 - 28.08.2023

**Localization:**
- Fixed the "Dance Urban" emote command which was not consistent with the rest of the dance commands. (/danceurban -> /urban)
- /strikeapose1 & /strikeapose2 -> /pose1 & /pose2



## 26.08.2023

- Graphics: APBCompat.ini - ParticleMaxWorldSpaceArea=50000.0 -> ParticleMaxWorldSpaceArea=0 for better grenade visibility, especially O-PGL. Only for the "Minimal" preset!
 
- When using "Disabled Texture Streaming" OR "Stutter Fix", you can now enable Bloom from the in-game settings as the actual "bloom" effect has been removed in those files, but the loadout/inventory menus will have a transparent, blurry background so you can see around you while changing loadouts.
 
- Various small localization fixes and updates.

- Small fix to the keybinds file.



## 24.06.2023

- Updated Keybinds file once again due to the Primary and Secondary weapon buttons not appearing in the controls menu in the previous release.



## 18.06.2023

- Very small bugfix to the Keybinds file which *potentially* prevents the game soft-locking in the login screen if you're not using the login screen config and -nomovies.



## 11.06.2023

- Added "Stutter Fix" to Features. This is an experimental config by Kyouki so please read the readme before using this!

- Added "Mission Stages only" to Localization which is a small addon for those who want to keep the game's vanilla localization but want the mission stages info in the description box.

- If using "Disable Texture Streaming" separately, you may now install "Notifications" alongside it like you would normally as it no longer relies on changes within the same file as the notifications to function properly.



## 27.05.2023 - Github Update - v1.0

- Migrated to Github and as such changed the entire structure of everything.

- Renaming and resetting the versions again, potentially one last time...?

- Added "Keybinds".

- Added proper integration for "Audio Emitters".

- Big update to the graphics file. Added option for no bullet holes.

- Small update to all localizations.

# Pre-Github Release



## 17.05.2023

- Added new Localization color preset "E-girl (Light Pink & Dark Grey)" which is sort of a work in progress still but should be fully functional.

- Removed "Graphics (MUST USE)" as it is no longer needed for disabled texture streaming. You may now use the regular graphics file again together with texture streaming disabled.

- Small optimizations to "Graphics".



## 11.05.2023

- Added a graphics preset in the "Disable Texture Streaming" folder which you MUST use if you're going to disable texture streaming as the last APB patch changed some things.

- Updated all Graphics presets to make grenade trail particles properly visible. Makes it easier to tell between frag and conc grenades and makes OPGL grenades easier to see, especially with not having Rainbow Concs/Glowing OPGL nades anymore.



## 03.05.2023

- Added "Disable Texture Streaming" to Features - Free FPS boost. Highly recommended to at least try. Check the folder for more info.

- Updated graphics file. Credit to lazer.

- Removed "Bloom Menu Transparency" as it is no longer needed and because shaders can no longer be modified.

- Moved "Remove Muzzle Flash + Remove Ragdolls" from Features to Visuals. Also removed the "Remove Player Ragdolls Only" variants as I doubt anyone would actually want to keep NPC ragdolls but remove player ones and to tone down file bloat.

- Moved "Remove Notifications" from Features to "Interface".



## 27.04.2023 (Easy Anti-Cheat launch)

- The following features have been stripped/adjusted as they either no longer work due to Easy Anti-Cheat (EAC)'s implementation OR have been included as in-game options and config files are no longer needed:

- Remove Muzzle Flash Particles - Integrated into "Remove Muzzle Flash + Remove Ragdolls". Read the readme in that file for clarification. | Added as a true/false toggle in DefaultGame.ini | .upk files are no longer modifiable.
- Rainbow Concs & Glowing OPGL Nades - .upk files are no longer modifiable.
- Remove Blood Particles - .upk files are no longer modifiable.
- Remove Bullet Holes & Effects Particles - .upk files are no longer modifiable.
- Remove Spray Objective Particles - .upk files are no longer modifiable.
- Extended Engine Font - Engine Font localization only from now on as .upk files are no longer modifiable.
- No Fog - Implemented as an in-game setting; shader edits no longer needed.

- Updated all localization.

- Added "Shortened Chat Channels" to Localization. Check the folder for details.

- Updated "Recommended Config Build" to reflect the changes following EAC and moved it to the bottom of the main README text file to cut down on bloat.

- Reset the version number once again.



## 15.03.2023

- Brought back "Remove Bullet Holes & Effects Particles" in Particles. Updated and now works on 64-bit. Credit to lazer.

- Fixed the in-game customer support URL (F1 key by default) - Mostly irrelevant as most people probably contact support outside of the game in a browser.

- Added several fps cap/uncap options to "FPS Unlocker" for the most common monitor refresh rates if you feel the need to cap your fps for whatever reason. Generally no reason to use anything less than "Unlimited" but still could be useful to some people having issues on their systems.

- Updated all localization.

- Added "Recommended Config Build" containing a recommended config build for APB by me, in case you are new to configs and modding.



## 05.03.2023

- Added "Remove Dialogue" to Audio which removes all/most character dialogue from the game. Read the text file inside for more info.

- Added "Lower Misc Audio Emitters" to Audio. Please read the text file.

- "Remove Ambient Sounds" in Audio will now also entirely remove the Joker Ammo vending machine voice lines. No more "NEED SOME AMMO??? GET SOME JOKER AMMO!!!"

- Updated graphics file.

- Updated all localization.

- Re-added "Remove VivoxVoiceService" to Features which was removed in V1.

- Fixed Player Only Ragdolls Removal folder structure.



## 08.02.2023 (APB 1.30 64-bit Upgrade)

- APB 1.30 is now released so I'm restarting the config versions counter from V1 again.

- All files optimized and configured for APB 1.30 (64-bit).

- Renamed "Graphics" to "Visuals".

- Updated all graphics presets by lazer.

- Updated all localization.

- Added "FPS Unlocker" to Features with options for 500fps or unlimited fps.

- Added "Bloom Menu Transparency" to Visuals.

- Added the actual files for "No Fog" and "RTW Vegas Sound" instead of download links.

- Redone and added features to "Extended Engine Font".


Removed the following items as they are now either redundant or no longer working as of APB 1.30:

- Removed the "144hz+ Slide Fix" as it is now integrated into the "FPS Unlocker". If you prefer 128fps you don't need the FPS Unlocker as the game's default max fps value is currently 128 anyway.

- Removed  "Remove Bullet Holes & Effects Particles" from Particles as it no longer works and will give a client mismatch.



## 07.11.2022

- Further optimized the graphics file - credit to lazer.

- Added new feature to all localization variants: The kill feed will now display not only the orange stun lightning icon but also the weapon that was used to stun the player next to it so it is clearer how a stun happened -Full credit goes to Leefekyn.

- Other minor updates to all localization variants.

- Added "White Mission Timer" under Interface - Unfortunately very broken and not recommended. Still included for anyone who wants to try it. Make sure to read the text file for it first. Credit to lazer.

- Added "Remove Bullet Holes & Effects Particles" under Particles.



## 15.10.2022

- Rebuilt the entire archive.

- Added a couple new features and moved things around. Extended Engine Font is now separate and will require additional text file editing if used at the same time as some of the other configs due to conflicting files.

- Fixed a few bugs from V21. Faster Loadout UI won't change the game's font and chatbox fade speed anymore.

- Updated all localization - "Item Not Ready Yet" message when attempting to use a mod that is on cooldown is now gone. Credit to Esurient.

- Updated most readme files.



## 28.09.2022

- Added "Faster Loadout UI" - Makes the Loadout Menu quicker and less laggy by replacing a texture. Read the readme in the folder for details. Credit to Esurient and lazer.

- Updated the "Maximum" video settings preset in the graphics file to be speee's graphics config (with full permission from speee). This is probably the best performance and FPS you can get out of APB but at the cost of all designs and symbols. It is a low poly config.

- Minor updates to all Localization presets.

- Minor changes to some of the readme files.



## 04.07.2022

- Updated "Engine Font" completely with new variants depending on how far you want to push the font stuff and whether you want Cyrillic/Russian support with it. Credit goes to Esurient and lazer for their work on this.



## 04.06.2022

- Updated Vanilla localization preset.

- Added "Engine Font" in the "Engine Font" localization folder - a new config by Esurient which replaces almost the entire UI's font with the engine font and not just parts of it accessible by localization alone. Read the text file for more info.



## 21.02.2022

- Added "Remove Nutcracker Skin Muzzle Flash" - Separate file if you want to get rid of the blue muzzle flash on the Nutcracker skin which is the only one that remains in the game if you apply the main files.

- Added "Remove Spray Objective Particles" - This removes the spray can objective particles so you can look around while doing them. This is still being tested so if you run into any issues, make sure to report them to me.

- Added "Remove Blood Particles"

- Updated graphics file - Updated all presets. Massive thanks to lazer for the help.

- Updates to all localization.

- New localization color scheme - Dark Blue and Dark Red.



## 24.01.2022

- Added "Remove Muzzle Flash Particles" - You're welcome. And no it won't get you banned, I've made sure of it. I wouldn't include it in this archive otherwise.

- Minor updates to all localization.



## 27.10.2021

- Updated all Localization presets for the Halloween Infection game mode.



## 12.10.2021

- Updated all Localization presets (including the Experimental Font one). Relatively small changes but they're neat.

- Fixed the Auto Sprint & Hold Crouch folder structure.

- Updated contacts descriptions to also show Wilson LeBoyce and Double-B's missions (thanks to lazer).



## 14.06.2021

- Fixed the graphics file having some incorrect values and messing everything up with environment textures. It should be back to working correctly again. Oops.

- Fixed the "Auto Sprint & Hold Crouch" having an APBCompat.ini file in it. Not sure how that happened but it has surely messed around with some things. Oops.

- Updated the "Experimental Font" Localization variant slightly. More will probably come to this in the future.

- Added the "For Localization Makers" folder in the Localization folder which includes all color tags and custom fonts info for those who want to make their own localization for APB.

- Sorted out the folders in the Loading + Login Screen folders so that the vanilla file is more easily found.



## 12.06.2021

- Added "Experimental Font" Localization variant which includes swapped out fonts in some places in the in-game UI. This is still work in progress and will receive multiple updates in the future.



## 14.05.2021

- Added 4th color scheme for localization due to several requests - Vanilla Green and Red (colors same as original game). Haven't actually tested it myself so feel free to report bugs.



## 21.03.2021

- Updated localization - minor mission stage description corrections.

- Updated graphics - mission-related graffiti should now be back to lowest quality.



## 06.03.2021

- Removed "Lower Shoulder Switch Delay". After some testing I've concluded that it makes things worse. While your camera might seem faster/smoother, it still does not show you where exactly your character is accurately and will often cause you to die behind corners when you shouldn't. It is better that you don't use it. In case you still have it and you want to get rid of it simply open: "APBGame\Config\DefaultGame.ini". in it find "m_bCalculateOnServer=" and set it to "true" like so: "m_bCalculateOnServer=true" then save the file.

- Updated graphics file:

a) Optimized it further for more FPS thanks to lazer.

b) Maximum preset has been replaced with the maximum preset provided by the Advanced APB Launcher for designing/filming/screenshotting purposes (higher than vanilla game maximum settings).

- Updated localization, added preview screenshots for all 3 color variants and renamed folder to just "Localization".

- Removed old graphics and old mission names as those are now obsolete. "Graphics" and "Localization" are the better variants respectively.

- Added separate variants for Auto Sprint & Hold Crouch if you only want to use one and renamed the folder to "Auto Sprint & Hold Crouch".

- Added "144hz+ Slide Fix" which is a workaround for the sliding that occurs in-game when you go over 128fps on 144hz+ refresh rate monitors.



## 26.01.2021

- Updated localization.



## 25.01.2021

- Updated localization.



## 15.12.2020

- Changed the "ParticleMaxWorldSpaceArea" value in APBCompat.ini to 10000.0 for all 5 graphics presets. This should help increase performance slightly while retaining all needed particles for bullet holes, effects, grenade smoke etc. Previous value was set to 0.0 which meant there could be infinite amount of particles at any given time which could cause fps drops on some hardware.



## 31.10.2020

- Fixed crash when using "Remove Notifications" upon opening contact menus.



## 19.10.2020

- Added "Rainbow Concs + Glowing OPGL Nades" due to popular request.

- Added "Remove Notifications"

- Added "Lower Shoulder Switch Delay"

Make sure to read the text files in each of those folders for more info.



## 12.10.2020

- Updated localization (Mainly mission stuff so its kind of important).



## 23.09.2020

- Updated localization.

- Added "Alternative (Turquoise & Magenta)" due to some people requesting it.



## 21.09.2020

- Updated localization with newest mission timers after the 16th Sept. Update.



## 30.08.2020

- Updated localization:

Apparently I put the wrong set of files in the Blue and Orange preset folder and they were both Greyscale. I never realised that and no one told me about it until now so I've now fixed it. Another update coming eventually when APBDB gets updated and I can generate a new mission descriptions file for any changed mission timers that came with the patch that came AFTER the Mission Impossible patch.

- Removed "Remove Themes + Songs" - LO updated APB to have an in-game toggle option to disable death themes as well as MVP themes so we don't need this config anymore.



## 08.08.2020

- Updated localization:

1. Fixed mission description stage timers to align with all mission changes after the "Mission Impossible" patch for both Normal and Greyscale variants.

2. Changed Greyscale variant to a slightly darker grey.



## 18.07.2020

- Updated localization.

- Localization now has a Greyscale option as seen on my stream due to popular request. Check the Flaws Localization (UI) text file for more info.



## 08.07.2020

- Added a 4th disclaimer to the readme. I recommend that you all read it.

- Added "Remove Ragdolls" with all possible variants included.

- Added "Remove Themes + Songs" and vanilla files if you want to revert it.

- Updated localization.



## 21.04.2020

- Changed method of low-poly graphics presets (see text file in the NEW graphics folder).
 
- Added transparent mission description and spawn screen to all graphics presets.

- Updated localization.

- Removed "Mission Stages (Description)" folder as it was a direct downgrade of my localization and lots of people used it without realising that.



## 18.02.2020

- Archive dubbed "Flaws Config V2" (no more years).

- Added "Flaws Localization" - My personal localization is now included with my config. Check the separate text file for it for more details.



## 11.02.2020

- Archive dubbed "Flaws Config 2020 V1".

- Added a new, more optimized graphics config but kept the old one as an option (new one highly recommended).

- Added visible grenade/OPGL/rocket smoke to all low-poly presets across the old and new graphic configs.

- Updated lazer's "Mission Stages (Description)" to the newest version as of 11.02.2020.

- Updated Advanced APB Launcher download link to the official Little Orbit one from the GamersFirst website in the Readme file.

- Updated Readme file.



## 23.11.2019

- Archive dubbed "Flaws Config 2019 V3".

- Added "Mission Stages (Description)" - Read text file inside the folder.

- Fixed the Shadows graphics preset and added 2 more low poly presets for low end PC's.

- Added info text files for each config separately for easier understanding and installing.



## 24.09.2019

- I will dub this archive Flaws Config 2019 V2 so that I can now change the version number everytime I update it, due to a lot of confusion on whether people have the newest one or an older one and that might be hard to keep track of when they are all classed as 2019.

- Swapped out the Login Screen file for a better one from Tobii's config.



## 17.06.2019

- Added "Remove VivoxVoiceService" - Details about this further down.

- Updated the Mission Names Config and it should now work flawlessly with the RIOT update. (Haven't tested it myself so report any issues with it to me on Twitch, Discord or Steam).

- Updated the Mission Names Config README file.

- Updated INSTRUCTIONS text file.

NOTE: The optional second graphics preset with shadows enabled does NOT currently work. I am not sure why that is but I likely won't update it further as the Engine Upgrade is coming relatively soon and we won't need configs to setup those things. You are however more than welcome to pick up where I left of with my config and enable shadows for yourself while using the rest of my graphics options.



## 15.05.2019

- Added a second (optional) graphics preset to the graphics APBCompat.ini with enabled shadows. Everything else is the same. Select the "Low" preset to enable shadows.



## 14.03.2019

- Changed Archive File Type to .zip for easier access even if you do not have WinRAR / 7Zip installed.

- Removed "No Fog Shader" - As a security measure to make sure no one gets banned/suspended accidentally, these files have been stripped from the archive and will not re-appear in later versions. (It was also later found out that removing fog in APB lowers FPS and causes deeper FPS drops.)

- Removed "Remove Muzzle Flash" - Removing any particles like this from the game is classed as cheating, therefore I will no longer distribute any particle removal files in my config. As well as, again, to prevent anyone from getting banned accidentally.



## 09.11.2018

- Removed "Mousefix" - It was discovered a couple months back by an LO/G1 employee that the mousefix doesn't actually do anything other than speed up your in-game sensitivity (forcing you to halve it). As such, I've removed it from the archive as it's useless.

- Removed "Remove Bullet Holes + Effects" - Due to recent patches to the game, editing anything in the "APB Reloaded\APBGame\Content\Release\Packages\VFX\Common" directory actually gives you an Unreal Engine error in-game and does not allow you to even login and as such has been removed from the archive.

- Removed "Input Lag Fix" - Like with the Mousefix, it is obsolete so it has been removed from the archive.
