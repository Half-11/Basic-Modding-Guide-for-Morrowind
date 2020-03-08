# Morrowind Basic Modding Guide

## About this guide
This guide aims to help (new) players to improve the game of Morrowind by giving step-by-step instructions on how to install the most essential mods.

Although the amount of information might be intimidating at first glance, the modlist itself is pretty basic (9 mods for the essential part, and another 9 for vanilla+). The information is there so you know exactly what to do in each scenario.

This guide is made up of three parts. The first part deals with the most essential mods. The second part are some mods that bring the game to a vanilla+ experience. The third and last part covers how to set up third party tool MGE XE.

# §1 Essential Mods 

## Step 1.1: Before we begin
Before we start installing mods we need to create an account and install some required software.

* [Register on Nexus](https://www.nexusmods.com/signup) - Most mods in this guide will be downloaded from Nexus. Nexus Mods is a site which allows users to upload and download "mods" (modifications) for computer games like Morrowind. In order to do this you have to create account. Click on the *REGISTER NOW* button to start your registration. The next screen will ask you to select a paid membership. **DON'T BE FOOLED BY THIS!** Just go to the bottom and select *Create Account* without selecting any membership. The rest is self-explanatory.

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

- Make sure you are running the latest official patch (v1.6.1820). Digital versions (Steam, GOG, Bethesda Launcher) of the game are up to date. If you are running the CD version, the correct installation order is: Morrowind / Tribunal / Bloodmoon / [Bloodmoon Patch v1.6.1820](https://cdn.bethsoft.com/elderscrolls/morrowind/patches/Bloodmoon_v1.6.1820.exe) (so skip Morrowind Patch v1.2.0722 and Tribunal Patch v1.4.1313).
     - *Note: When you are in doubt about the version of your game; this can be found at the bottom left of the main menu in-game.*

## Step 1.3: Morrowind Code Patch
The Morrowind Code Patch (MCP) fixes bugs and problems that aren't possible to do with scripting alone. MCP reduces crash and save corruption problems. In addition there are many more smaller optional fixes that cover all sorts of areas of the game.

1. [Download Morrowind Code Patch](https://www.nexusmods.com/morrowind/mods/19510)
     - *Note: Get the Standard exe version (ignore the Python version).*

2. Extract the zip to your ***/Morrowind*** root directory, the one with the Morrowind.exe program in it (not Data Files).

3. Set the Morrowind Code Patch program and Morrowind.exe as run as an administrator.
     - *Instructions: When you put to the Morrowind Code Patch.exe executable in the root of your Morrowind folder, right-click on it to view the contextual menu. Then, click or tap on Properties. In the Properties window, go to the Compatibility tab. At the bottom of the window, check the box that says "Run this program as an administrator" and then click or tap on Apply or OK.*
     - *Repeat this process for Morrowind.exe (also located in the root of your Morrowind folder).*

4. Start MCP by running the *Morrowind Code Patch.exe* executable. You will see categories and patches listed on the left. The program will explain what each patch does, click on the patch name to display the explanation on the right. Each patch can be turned on and off by clicking the checkbox to the left of the name.
The defealt selection is pretty good and recommended for new players. We need to add two patches however to ensure functionality for Patch for Purists. Under the *Mod specific* tab select the following:
- `Separate axe inventory sounds`
- `Creature voiceover enable`

5. Click *Apply the chosen patches*. Your Morrowind.exe will now be updated (You can do this at any time and it doesn't matter if you patched your Morrowind.exe before).

## Step 1.4: Patch for Purists
Patch for Purists is an unofficial fan patch for Morrowind. It  takes a more conservative approach about what it considers a "bug" than the Morrowind Patch Project you might know from the past. PfP covers pretty much every aspect of the game within the limitations of the Construction Set (e.g broken quests, floating objects, lots of broken dialogue etc).

1. [Download Patch for Purists](https://www.nexusmods.com/morrowind/mods/45096)

2. Extract the zip to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click *Yes*.

## Step 1.5: Morrowind Optimization Patch
Morrowind Optimization Patch (MOP) does two things: it noticeably improves performance and fixes mesh errors. 

1. [Download Morrowind Optimization Patch](https://www.nexusmods.com/morrowind/mods/45384)

2. Extract the *Meshes* and *Textures* folders and *Lake Fjalding Anti-Suck.esp* to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click *Yes*.
     - *Note: When looking at the contents of the zip you might notice unfamiliar folder names (00 Core, 01 Clean Alpha Textures, 02 Lake Fjalding Anti-Suck). This is because MOP has a archive folder structure intended for mod managers (called "BAIN installer"). For a simple setup like ours a manager is not needed. The only thing we want here are the contents of the subfolders.*
     - *Copy and paste the two Meshes and the Textures folders and the Lake Fjalding Anti-Suck.ESP file into your Morrowind\Data Files folder. In other words; treat each folder as if you were installing a separate mod.*
     - *Regarding BAIN installers: these are often used to deliver optional patches for other mods. An mistake that is often made by people who are new to modding Morrowind, is installing these patches for mods that they have not actually installed. This will result in error messages because the game is missing the files from the mod for which the patch in question was intended. When you are not sure whether the optional modules are patches or extras for the mod itself, please read the ReadMe carefully.*

## Step 1.6: Project Atlas
Project Atlas improves performance even further by using different techniques than MOP. Using them together will get you quite the FPS gain.

1. [Download Project Atlas](https://www.nexusmods.com/morrowind/mods/45399)
     - *Warning: This mod is not recommended if you play the game on a very old GPU. The so-called texture atlases are quite large and might actually hurt your performance in this case. Semi-modern onboard Intel/AMD GPUs should be okay though.*

2. Yet again, we're dealing with BAIN archive folder structures. Extract the *Meshes* and *Textures* folders to your ***Morrowind/Data Files*** directory.
     - *Some of the modules come with ***Smoothed Meshes*** and ***Optional Hi-Res Texture*** folders. It's totally up to you whenever you want to install these or not.*
     - *The [Glow in the Dahrk (GitD)](https://www.nexusmods.com/morrowind/mods/45886) and [Glowing Bitter Coast](http://mw.modhistory.com/download-44-14321) folders should only be used when the corresponding mods are installed. If you want to use these mods, make sure to install them before installing Project Atlas.*

When looking at the contents of the zip you might notice unfamiliar folder names (00 Core, 01 Clean Alpha Textures, 02 Lake Fjalding Anti-Suck). This is because MOP has a BAIN archive folder structure intended for mod managers. For a simple setup like ours a manager is not needed. The only thing we want here are the contents of the subfolders.

## Step 1.6 MGE XE
MGE XE is an utility that allows the game to render distant land, shadows, shaders, atmospheric effects and much more.

1. Run the game at least once before you installing.

2. [Download MGE XE](https://www.nexusmods.com/morrowind/mods/41102)
     - *Note: Download the MGE XE Manual Install (skip on the MGE XE Installer).*

3. Extract the zip to your ```Morrowind``` root folder (the folder with Morrowind.exe in it). When asked to overwrite the file, click *Yes*.

4. Before we are going to set up MGE XE, we want to run the ***MWSE-Update.exe*** we just copied.
     - *Note: Doing this will ensure we are running the latest nightly build of MWSE 2.1 (Morrowind Script Extender Lua) which we need for some of the mods later on in this guide. MWSE 2.1 is actively maintained so it is recommended to do this now and then.*

## Step 1.7 Some minor essential mods

1. [Better Dialogue Font](https://www.nexusmods.com/morrowind/mods/36873)

2. [Expeditious Exit](https://www.nexusmods.com/morrowind/mods/45634)

3. [Expansion Delay](https://www.nexusmods.com/morrowind/mods/47588)

4. [Fix Those Bastard Rope Fences](https://www.nexusmods.com/morrowind/mods/45741)


# §2 Optional mods for a Vanilla+ installation
The following mods are all optional and can be skipped. If all you wanted were bug fixes and performance improvements, you can skip to **§3 Setting up MGE XE** below. However, if you want to enhance the games aesthetics with a few more mods in a vanilla friendly way; read on.

## Step 2.1: Intelligent Textures
Intelligent Textures replaces almost all textures in the vanilla game and its expansions with high resolution AI upscales.

1. [Download Intelligent Textures](https://www.nexusmods.com/morrowind/mods/47469)

2. We want to copy just one folder from the zip we just downloaed. Extract the *Meshes* folder found inside *00 Core* to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click *Yes*.

## Step 2.1: Properly Smoothed Meshes
Here, you have to make a choice whenever you care about smoother models. If you don't, you can skip this step. Properly Smoothed Meshes offers more detailed models in a vanilla fashion. This mod is optional. If you're fine with the vanilla models, you can skip on this one.

1. [Download Properly Smoothed Meshes](https://www.nexusmods.com/morrowind/mods/46747)

2. In the zip file we just downloaded you'll find two folders ***00 Core + 01 Atlas Textures***. Extract the content of both folders to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click *Yes*.

## Step 2.2: Graphic Herbalism - MWSE and OpenMW Edition
This mod makes it so that you pick plants just by activating them instead of opening them like a container. When harvesting part of the plant you pick disappears.

1. [Download Graphic Herbalism MWSE - OpenMW](https://www.nexusmods.com/morrowind/mods/46599)
     - *Note: We will only need the Main File.*

2. In the zip file we just downloaded you'll find two folders ***00 Core + Vanilla Meshes*** and ***01 Optional - Smoothed Meshes***. Start with extracting the content of the ***00 Core + Vanilla Meshes*** folder to your ***Morrowind/Data Files*** directory. When asked to overwrite the file, click *Yes*.

3. The second folder, ***01 Optional - Smoothed Meshes***, is optional. If you care about smoother models for the flora, you can repeat the process from the previous step for this folder. If you don't care about this, you can just ignore this folder.

## Step 2.3: Glow in the Dahrk
Glow in the Dahrk makes windows glow at night. Again, this mod is optional.

1. [Download Glow in the Dahrk](https://www.nexusmods.com/morrowind/mods/45886)

2. Yet again, we're dealing with BAIN archive folder structures. Extract the contents of the following folders to your ***Morrowind/Data Files*** directory:
- `00 Core`
- `01 Hi Res Window Texture Replacer (skip if you decided not to use Intelligent Textures above)`
- `02 Interior Sunrays`
- `03 Nord Glass Windows`
- `03 Nord Glass Windows Interior Sunrays`
- `05 Raven Rock Glass Windows`
- `05 Raven Rock Glass Windows Interior Sunrays`






# §3 Setting up MGE XE

5. Now open ***MGEXEgui.exe***. You will see a tabbed interface. We will start setting up the first tab from the left. Make sure to use the following settings:

>**Display**
>
>Resolution: your monitor resolution
>
>Windowed mode: checked
>
>Borderless window: checked
>
>Antialiasing: 8x (or 4x if you are worried about performance)
>
>Anisotropic filtering: 8x
>
>VSync: On
>
>Enable shaders: checked
>
>Auto FOV: checked
>
>FPS limiter: 60 (more frames will cause issues with animations)

6. Click **Shader setup...** in the first MGE XE tab. Then click **Modding >>>**. Now double click available shaders in the following order:
```
SSAO
Underwater Effects
Underwater Interior Effects
Sunshafts
Bloom Soft (you can also use Bloom Fine here for a more subtle bloom)
```
7. **Optional step (can be skipped)**: *deband_fogaware* is a shader that blurs the fog in addition to fixing banding. This shader does not come with MGE XE out of the box but can be [downloaded here](https://cdn.discordapp.com/attachments/381217735306248192/587447644876439572/deband_fogaware.fx). Put the *deband_fogaware.fx* file inside your ```Morrowind\Data Files\shaders\XEshaders``` folder. Close and restart ***MGEXEgui.exe*** and put the new shader at the end of your *Active Shaders* list (like we did in the previous step). It should now look like this:
```
SSAO HQ
Underwater Effects
Underwater Interior Effects
Sunshafts
Bloom Soft (you can also use Bloom Fine here for a more subtle bloom)
deband_fogaware
```
8. Now we are going to the second tab from the left. Make sure to use the following settings:

>**Distant Land**
>
>Use Distant Land: checked
>
>Draw Distance: 3,7 cells (this is what I personaly use but anything beteen 3.0 and 5.0 seems reasonable to aim for)
>
>Auto set other distances: checked (By Draw Distance)
>
>Water Reflections: check all (Nearby Statics can be skipped in favour of performance)
>
>Use Distant Statics: checked (Near: 130, Far: 600, Very Far: 780)
>
>Dynamic ripples: checked (30 Height of waves)
>
>Caustic: 35% brightness
>
>Use high quality (exponential) fog: checked
>
>High quality atmosphere & distance colouring: checked
>
>Dynamic solar shadows: checked
>
>Per-pixel lightning shader: uncheck (it's extremely heavy on performance especially on a weak CPU)
>
>Exponential distance multiplier 4.4
>
>Use high quality (exponential) fog: checked (can be unchecked in favour of performance)
>
>High quality atmosphere & distance colouring: checked

9. Now we are going to run the **Distant land generator wizard** (the square button at the top left in the Distant Land tab). Hit **Select all** and then **Continue**.




Weapon Sheathing

Remiros' Groundcover
https://www.nexusmods.com/morrowind/mods/46733

WIP Detailed Correct UV Rocks
https://www.nexusmods.com/morrowind/mods/44321?tab=files


Better Waterfalls
https://www.nexusmods.com/morrowind/mods/45424

Mist Retexture
https://www.nexusmods.com/morrowind/mods/44322

RopeFenceFix


Krokantor's Enhanced Water Shader for MGE XE updated to work with latest MGE XE version.
https://cdn.discordapp.com/attachments/381217735306248192/579434115720413184/Enhanced_Water_Shader_for_MGE_XE_2.1_wip.7z



Morrowind Essentials is a project aimed at the distribution of a single updated package for mods that are considered essential.

As fun as it can be to browse trough modding guides, forums and pages, it can also be can be a headache; especially to people new to the game.

tes3cmd
https://storage.googleapis.com/google-code-archive-downloads/v2/code.google.com/mlox/tes3cmd-0.37v-2013.10.06.7z

resetdates.bat
