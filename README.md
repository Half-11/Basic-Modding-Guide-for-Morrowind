![alt text](https://s1.qwant.com/thumbr/0x380/3/8/d7f5496f0150df0e1393821d5717583648166b6b339654fc7fdab94b9fd658/1384957911_m50.jpg?u=http%3A%2F%2Felder-scrolls.com%2Fuploads%2Fposts%2F2013-11%2F1384957911_m50.jpg&q=0&b=1&p=0&a=1)


# Morrowind: Basic Modding Guide

## About this guide
This guide aims to help (new) players to improve the game of Morrowind by giving step-by-step instructions on how to install the most essential mods.

Although the amount of information might be intimidating at first glance, the modlist itself is pretty basic. The information is there so you know exactly what to do in each scenario.

This guide is made up of three parts. The first part deals with the most essential mods (8 total). The second optional part are some more mods (10) that bring the game to a vanilla+ experience. The third and last part covers how to set up third party tool MGE XE.

*Full disclosure: I'm the author of both Patch for Purists and Expansion Delay which are recommended in this guide.*

# §1 Essential Mods 

## Step 1.1: Before we begin
Before we start installing mods we need to create an account and install some required software.

* [Register on Nexus](https://www.nexusmods.com/signup) - Most mods in this guide will be downloaded from Nexus. Nexus Mods is a site which allows users to upload and download "mods" (modifications) for computer games like Morrowind. In order to do this you have to create account. Click on the *REGISTER NOW* button to start your registration. The next screen will ask you to select a paid membership. **DON'T BE FOOLED BY THIS!** Just go to the bottom and select *Create Account* without selecting any membership. The rest is self-explanatory. [Here is a short video guide](https://youtu.be/ZoS87E5_rn0?t=15).

* [7-Zip](https://www.7-zip.org/download.html) - If you have no file archiver installed on your computer I would recommened installing one. All mods on Nexus will be downloaded as one archive file (.7z/.rar/.zip files). 7-Zip is one of the best-known utilities for unpacking such archives into their orginal state.
     - *Note: If you have never used 7-Zip before I would recommend to watch [this short tutorial](https://www.youtube.com/watch?v=WCxbEQo3Zhg) on how to extract files with it.*

* [DirectX 9.0c June 2010](http://www.microsoft.com/download/en/details.aspx?id=35) - This is a required update for third-party software we are going to use. This won't conflict with exisiting installations of DirectX (10+).
     - *Note: Uncheck the **Install Bing Bar** thingy during installation. It's just bloatware.*

* [Microsoft Visual C++ 2015 Redistributable (x86)](https://www.microsoft.com/en-us/download/details.aspx?id=48145) - This is another requirement for third-party software later in this guide.
     - *Instructions: Select your language on the Microsoft website. Click the **Download** button. Check the box before **vc_redist.x86.exe**. Click the **Next** button (or use this [direct link](https://aka.ms/vs/16/release/vc_redist.x86.exe)).*
    - *Note: For Morrowind you'll need the *vc_redist.x86.exe* file, regardless of your computers architecture.*

## Step 1.2: Propper Game Installation
- Don't install the game in its default folder (C:\Program Files). This folder is monitored by the security system, which was unknown at the time of Morrowinds design. The default installation location can lead to crashes, error messages and mods not appearing. Instead, it is strongly recommended to create a new folder on your hard drive, such as: C:\Games\Morrowind.
     - *Steam users can follow [this short tutorial](https://www.youtube.com/watch?v=hV1UbXLTsy0) to change the games installation path to a non-Program Files location. edit libraryfolders.vdf if want add second library on same partition
current steam client limited to 1 library per partition 
"2" "C:\\Games"*
     - *GOG users need to remove the default Meshes, Textures, Icons and Bookart folders found in Morrowind\Data Files after a fresh install. The original Construction Set disc (a separate disc) came with uncompressed assets. GOG thought it was a good idea to put those in the games Data Files folder, but the game can't handle these files well. This is causing the load times to slow down without any visual improvements. Don't worry about deleting these folders; all files are already present in the BSA.*
     - *In addition, I would recommended GOG users to remove the "official plugins" that come with this version of the game. Remove the following files from your Morrowind\Data Files folder:*
```
adamantiumarmor.esp
AreaEffectArrows.esp
bcsounds.esp
EBQ_Artifact.esp
entertainers.esp
LeFemmArmor.esp
master_index.esp
Siege at Firemoth.esp
```
 
   - I'm giving you fair warning that [the official plugins](https://en.uesp.net/wiki/Morrowind:Plugins) are pretty shitty. They are buggy; have balance issues; and don't fit the vanilla game. If you ask me, only two are worth playing really (Bitter Coast Sounds & Master Index). If you want to play with these mods, you could take a look at the [fixed versions in UMOPP 3.0.4](https://www.nexusmods.com/morrowind/mods/43931) (I would ignore the Merged and Compatibility Versions and go with the UMOPP 3.0.4 file).

- Make sure you are running the latest official patch (v1.6.1820). Digital versions (Steam, GOG, Bethesda Launcher) of the game are up to date. If you are running the CD version, the correct installation order is: Morrowind CD / Tribunal CD / Bloodmoon CD / [Bloodmoon Patch v1.6.1820](https://cdn.bethsoft.com/elderscrolls/morrowind/patches/Bloodmoon_v1.6.1820.exe) (skip Morrowind Patch v1.2.0722 and Tribunal Patch v1.4.1313).
     - *Note: When you are in doubt about the version of your game; this can be found at the bottom left of the main menu in-game.*

## Step 1.3: Morrowind Code Patch
The Morrowind Code Patch (MCP) fixes bugs and problems that aren't possible to do with scripting alone. MCP reduces crash and save corruption problems. In addition there are many more smaller optional fixes that cover all sorts of areas of the game.

1. [Download Morrowind Code Patch](https://www.nexusmods.com/morrowind/mods/19510)
     - *Note: Get the Standard exe version (ignore the Python version).*

2. Extract the zip to your ***/Morrowind*** root directory, the one with the Morrowind.exe program in it (not Data Files).

3. Start MCP by running the *Morrowind Code Patch.exe* executable. You will see categories and patches listed on the left. The program will explain what each patch does, click on the patch name to display the explanation on the right. Each patch can be turned on and off by clicking the checkbox to the left of the name.
The defealt selection is pretty good and recommended for new players. We need to add two patches however to ensure functionality for Patch for Purists. Under the *Mod specific* tab select the following:
- `Separate axe inventory sounds`
- `Creature voiceover enable`

4. Click *Apply the chosen patches*. Your Morrowind.exe will now be updated (You can do this at any time and it doesn't matter if you patched your Morrowind.exe before).

## Step 1.4: Patch for Purists
Patch for Purists is an unofficial fan patch for Morrowind. It  takes a more conservative approach about what it considers a "bug" than the Morrowind Patch Project you might know from the past. PfP covers pretty much every aspect of the game within the limitations of the Construction Set (e.g broken quests, floating objects, lots of broken dialogue etc).

1. [Download Patch for Purists](https://www.nexusmods.com/morrowind/mods/45096)

2. Extract the zip to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click *Yes*.

## Step 1.5: Morrowind Optimization Patch
Morrowind Optimization Patch (MOP) does two things: it noticeably improves performance and fixes mesh errors. 

1. [Download Correct UV Rocks](http://mw.modhistory.com/download-56-12003)
     - *Note: Every now and then the servers of Morrowind Modding History are down. If that is the case, then a mirror can be found [here](https://web.archive.org/web/20161103112615/mw.modhistory.com/download-56-12003).*

2. Extract the *Meshes* folder to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click *Yes*.

3. [Download Morrowind Optimization Patch](https://www.nexusmods.com/morrowind/mods/45384)

4. Extract the *Meshes* and *Textures* folders and *Lake Fjalding Anti-Suck.esp* to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click *Yes*.
     - *Note: When looking at the contents of the zip you might notice unfamiliar folder names (00 Core, 01 Clean Alpha Textures, 02 Lake Fjalding Anti-Suck). This is because MOP has a archive folder structure intended for mod managers (called "BAIN installer"). For a simple setup like ours a mod manager is not needed. The only thing we want here are the Meshes and Textures subfolders.*
     - *Copy and paste the two Meshes and the Textures folders and the Lake Fjalding Anti-Suck.ESP file into your Morrowind\Data Files folder. In other words; treat each folder as if you were installing a separate mod.*
     - *Regarding BAIN installers: these are often used to deliver optional patches for other mods. A mistake that is often made by people who are new to modding Morrowind, is installing these patches for mods that they have not actually installed. This will result in error messages because the game is missing the files from the mod for which the patch in question was intended. When you are not sure whether the optional modules are patches or extras for the mod itself, please read the ReadMe carefully.*

## Step 1.6 MGE XE
MGE XE is an utility that allows the game to render distant land, shadows, shaders, atmospheric effects and much more.

1. Run the game once into the main menu and exit, before installing MGE XE.

2. [Download MGE XE](https://www.nexusmods.com/morrowind/mods/41102)
     - *Note: Download the ***MGE XE Manual Install*** (skip on the MGE XE Installer).*

3. Extract the zip to your ```Morrowind``` root folder (the folder with Morrowind.exe in it; NOT Morrowind\Data Files). When asked to overwrite files, click *Yes*.

4. We now want to run the ***MWSE-Update.exe*** we just copied inside the Morrowind root folder.
     - *Note: Doing this will ensure we are running the latest nightly build of MWSE 2.1 (Morrowind Script Extender Lua) which we need for some of the mods later on in this guide. MWSE adds new functionality to the scripting language of Morrowind, allowing for new features to be implemented into the game. MWSE 2.1 is actively maintained, so it is recommended to do this now and then, especially when you use other MWSE mods.*

## Step 1.7 Some minor essential mods
Finally, there are a few minor mods that I consider essential. Again, extract these zips to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click Yes.

1. [Better Dialogue Font](https://www.nexusmods.com/morrowind/mods/36873)

2. [Expeditious Exit](https://www.nexusmods.com/morrowind/mods/45634)

3. [Expansion Delay](https://www.nexusmods.com/morrowind/mods/47588)

4. [Fix Those Bastard Rope Fences](https://www.nexusmods.com/morrowind/mods/45741)


# §2 Optional mods for a Vanilla+ installation
The following mods are all optional. If all you want are bug fixes and performance improvements, you can skip to **§3 Setting up MGE XE** below. However, if you want to enhance the games aesthetics and gameplay with a few more mods in a vanilla friendly way; read on.

All of the following mods are optional. Each can be skipped based on personal preference.

## Step 2.1: Properly Smoothed Meshes
Here, you have to make a choice whenever you care about smoother models. If you don't, you can skip this step. Properly Smoothed Meshes offers more detailed models in a vanilla fashion.

1. [Download Properly Smoothed Meshes](https://www.nexusmods.com/morrowind/mods/46747)

2. In the zip file we just downloaded you'll find multiple BAIN archive folders. We are only interested in ***00 Core***. Extract the content of this folder to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click *Yes*.

## Step 2.2: Glow in the Dahrk
Glow in the Dahrk makes windows glow at night.

1. [Download Glow in the Dahrk](https://www.nexusmods.com/morrowind/mods/45886)

2. Yet again, we're dealing with BAIN archive folder structures. Extract the contents of the following folders to your ***Morrowind/Data Files*** directory:
- `00 Core`
- `01 Hi Res Window Texture Replacer (skip if you decided not to use Intelligent Textures above)`
- `02 Interior Sunrays`
- `03 Nord Glass Windows`
- `03 Nord Glass Windows Interior Sunrays`
     - *Note: Don't install the **Hi Res Window Texture Replacer** folder right away.* because we want it to overwrite the Intelligent Textures (Step 2.4) later on in the guide.

## Step 2.3: Project Atlas
Project Atlas improves performance even further by using different techniques than MOP. Using them together will get you quite the FPS gain.

1. [Download Project Atlas](https://www.nexusmods.com/morrowind/mods/45399)
     - *Warning: This mod is not recommended if you play the game on a very old GPU. The so-called texture atlases are quite large and might actually hurt your performance in this case. Semi-modern onboard Intel/AMD GPUs should be okay though.*

2. Yet again, we're dealing with BAIN archive folder structures. Extract the *Meshes* and *Textures* folders inside the *00 Core* folder to your ***Morrowind/Data Files*** directory.

3. You'll find some more optional modules in the archive:
     - ***30 Redware - Smoothed** and **40 Urns - Smoothed** can be installed if you chose to install Properly Smoothed Meshes earlier.*
     - *The **Glow in the Dahrk (- Interior Sunrays)** and **[Glowing Bitter Coast](http://mw.modhistory.com/download-44-14321)** folders should only be used when the corresponding mods are installed. If you want to use these mods, make sure to install them BEFORE installing Project Atlas.*

## Step 2.4: Intelligent Textures
Intelligent Textures replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.

1. [Download Intelligent Textures](https://www.nexusmods.com/morrowind/mods/47469)

2. Extract the contents of both the ***00 Core*** and the ***01 Atlas Textures*** folders to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click *Yes*.
     - *Note: If you chose to install Glow in the Dahrk (Step 2.2) you can now install its ***Hi Res Window Texture Replacer*** folder in the same manner.*

## Step 2.5: Remiros' Groundcover
Remiros' Groundcover is one of the best (if not the best) grass and groundcover mod for Morrowind.

1. [Download Remiros' Groundcover](https://www.nexusmods.com/morrowind/mods/46733)
     - *Note: We want the non-OpenMW file on top of the download page (not ***Remiros' Groundcover - OpenMW***).*

2. In the download you'll find a big BAIN archive with all kinds of options. We are only interessed in the contents of the ***00 Core*** folder. Extract its contents to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click *Yes*.
     - *Note: If for some reason you don't like the small mushrooms this mod adds, you can install the contents of the ***04a No Mushrooms*** folder in the same manner.*

## Step 2.6: Graphic Herbalism - MWSE and OpenMW Edition
This mod makes it so that you pick plants just by activating them instead of opening them like a container. When harvesting, part of the plant you pick disappears.

1. [Download Graphic Herbalism MWSE - OpenMW](https://www.nexusmods.com/morrowind/mods/46599)
     - *Note: We will only need the Main File.*
     - *Note: [Happy Harvesting](https://www.nexusmods.com/morrowind/mods/45627) does the same thing without the visual part. Purist players might prefer this mod instead.*

2. In the zip file we just downloaded you'll find two folders ***00 Core + Vanilla Meshes*** and ***01 Optional - Smoothed Meshes***. Start with extracting the content of the ***00 Core + Vanilla Meshes*** folder to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click *Yes*.

3. The second folder, ***01 Optional - Smoothed Meshes***, is optional. Personally, I don't like the looks of the smoother models for flora and ignore this folder. If you  like them then you can repeat the process from the previous step for this folder.

## Step 2.7: Weapon Sheathing
Weapon Sheathing makes unreadied weapons and shields appear on the character's hip or back (incl. quivers).

1. [Download Weapon Sheathing](https://www.nexusmods.com/morrowind/mods/46069)
     - *Note: We want the ***WeaponSheathing1.6-MWSE*** file (not ***WeaponSheathing1.6-OpenMW***).*

2. In the zip file we just downloaded you'll find two folders ***Data Files*** and ***Extras***. Ignore the ***Extras*** folder. Extract the contents of the ***Data Files*** folder to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click *Yes*.

## Step 2.8 Some minor mods
Finally, here are a few more minor graphical mods that are a nice  addition to the game. Again, extract these zips to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click Yes.

1. [Better Waterfalls](https://www.nexusmods.com/morrowind/mods/45424)

2. [Mist Retexture](https://www.nexusmods.com/morrowind/mods/44322?tab=files)


# §3 Setting up MGE XE
Now it's time to set up MGE XE; the tool responsible for shaders and increased draw distance. Open ***MGEXEgui.exe*** found inside your Morrowind folder. You will see a tabbed interface. We will use default settings unless otherwise indicated. Make sure to use the following settings in the first tab from the left:
>**Display**
>
>Resolution: set this to your monitor resolution (after this is don't want to touch the resolution in the Morrowind Launcher ever again)
>
>Windowed mode: checked
>
>Borderless window: checked (helps alt-tabbing the game)
>
>Antialiasing: 8x
>
>VSync: On
>
>Enable shaders: checked
>
>FPS limiter: 60 (more frames can cause issues with animations)
>
>Menu UI scaling (I would leave this 1,00 but if you have vision problems or the ingame letters are simply to small for your taste; you can increase this to e.g. 1,20)

6. Click **Shader setup...** in the first MGE XE tab. Then click **Modding >>>**. Now double click available shaders in the following order:
```
SSAO HQ
Underwater Effects
Underwater Interior Effects
Sunshafts
Bloom Soft (people who don't like bloom can skip this one)
```
   Hit *Save*.

8. Now we are going to the second tab from the left. Run the **Distant land generator wizard** (the square button at the top left in the Distant Land tab). Hit **Select all** and then **Continue**. You're asked to set resultions but we just want to use the default settings here; click **Create Land Textures**. When asked for *World mesh detail* leave this at the default *High* (or set it to *Ultra High* when you feel confident about your hardware). Click **Create Land Meshes**. In the *Statics* tab we want to leave most stetting default though we want to set *Minimum static size* to 130.  Click **Create Statics** and wait for the program to finish. Click **Finish** when its done.

Make sure to use the following settings:

>**Distant Land**
>
>Use Distant Land: checked
>
>Draw Distance: 3,7 cells (this is what I personaly use but anything beteen 3.0 and 5.0 seems reasonable to aim for)
>
>Auto set other distances: checked (By Draw Distance)
>
>Water Reflections: check all but Blur Reflections
>
>Use Distant Statics: checked (Near: 130, Far: 600, Very Far: 780)
>
>Dynamic ripples: checked (50 Height of waves)
>
>Caustic: 50% brightness
>
>Use high quality (exponential) fog: checked
>
>High quality atmosphere & distance colouring: checked
>
>Dynamic solar shadows: checked
>
>Per-pixel lightning shader: uncheck (it's extremely heavy on performance especially on a weak CPU)
>
>Exponential distance multiplier 4.0
>
>Use high quality (exponential) fog: checked (can be unchecked in favour of performance)
>
>High quality atmosphere & distance colouring: checked

9. The third *In-Game* tab is self-explanatory. I like to check to following (in addition to the default settings):

>**Config**
>
>Skip opening movie
>
>Allow yes to all load errors
>
>Allow screenshots

We can now close MGE XE as we don't need to change anything in the other tabs.

# §4 Final steps
Now there are a few things left to do.

1. Open **Morrowind Launcher** trough shortcut or *Morrowind\Morrowind Launcher.exe*. Click on the *Data Files* button. Here we want to activate the mods we want to play with. To activate mods you'll have to double click them so they get a check mark.
- Don't activate the .esps that start with **Rem_**; these are our grass mods and only need to be active durning Distant Land generation within MGE XE.
- **XE Sky Variations.esp** comes with MGE XE. It affects the colours of clear and cloudy skies and makes it so that you will have a different sky scattering colours every day. Highly recommended to use.

2. The last thing set to do is adjusting the Gamma Correction option ingame (Options > Video). This affects the overall brightness of the game. If you like how the game looks, you might want to skip this step, but since every monitor is different it might be worth to tweak this setting a little.




From here on you can decide to install your own selection of mods on top of this guide, though one could argue that a slightly modded vanilla setup is the best way of playing Morrowind (especially for people how experience the game for the first time).


Almost twenty years of modding gave us lots of great mods but even more crappy ones. Don't expect to improve the game by installing dozens of mods that just sound good on paper. Chances are they don't meet the quality of the orignal game or cause (compatibility) issues. Other mods that were looked up to in the past didn't exactly age well (LGNPC, Morrowind Comes Alive, etc).



When it comes to modding Morrowind; more is not always better.
I would urge you not to install dozens of mods and hope you get it right.





As fun as it can be to browse trough modding guides, forums and pages, it can also be can be a headache; especially to people new to the game.

tes3cmd
https://storage.googleapis.com/google-code-archive-downloads/v2/code.google.com/mlox/tes3cmd-0.37v-2013.10.06.7z

resetdates.bat



MGE/MWSE Mods List
https://github.com/Lucevar/mw-immersion-mods/blob/master/mwse.md

Tamriel Rebuilt Recommended mods
https://www.tamriel-rebuilt.org/recommended-mods

Merlord's Immersive Modlist
https://docs.google.com/spreadsheets/d/1euy-S5Y8SFHG6lLzgbo2_ck5KvslFL92bHUjaCJz7_c/edit?usp=sharing
