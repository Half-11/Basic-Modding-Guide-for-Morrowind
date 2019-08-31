# Basic Modding Guide for Morrowind

## About this guide
This guide aims to help (new) players to improve the game of Morrowind by giving a step-by-step explanation on how to install the most essential mods.

## 1. Before we begin
Before we start installing mods we need to create an account and install some required software.

* [Register on Nexus](https://www.nexusmods.com/signup) - Most mods in this guide will be downloaded from Nexus. Nexus Mods is a site which allows users to upload and download "mods" (modifications) for computer games like Morrowind. In order to do this you have to create account. Click on the REGISTER NOW button to start your registration. The next screen will ask you to select a paid membership. DON'T BE FOOLED BY THIS! Just go to the bottom and select "create account" without selecting any membership. The rest is self-explanatory

* [7-Zip](https://www.7-zip.org/download.html) - If you haven't a file archiver installed on your computer I would recommened installing one. All mods on Nexus will be downloaded as one archive file (.7z/.rar/.zip files). 7-Zip is one of the best-known utilities for unpacking such archives into their orginal state.
     - *Note: If you have never used 7-Zip before I recommend to watch [this short tutorial](https://www.youtube.com/watch?v=WCxbEQo3Zhg) on how to extract files with it.*

* [DirectX 9.0c June 2010](https://www.microsoft.com/en-us/download/details.aspx?id=8109) - This is a required update for third-party software we are going to use and won't conflict with exisiting installations of DirectX (10+).

* [Microsoft Visual C++ 2010 Redistributable Package (x86)](https://www.microsoft.com/en-us/download/details.aspx?id=8109) - This is another requirement for third-party software later in this guide.

## 2. Propper Game Installation
- Don't install the game in its default folder (C:\Program Files). This folder is monitored by the security system, which was unknown at the time of Morrowinds design. The default installation location can lead to crashes, error messages and mods not appearing. Instead, it is strongly recommended to create a new folder on your hard drive, such as: C:\Games\Morrowind.
     - *Steam users should follow [this short tutorial](https://www.youtube.com/watch?v=hV1UbXLTsy0) to change the games installation path to a non-Program Files location.*
     - *GOG users need to remove the default Meshes, Textures, Icons and Bookart folders found in Morrowind\Data Files after a fresh install. The original Construction Set disc (a separate disc) came with uncompressed assets. GOG thought it was a good idea to put those in the games Data Files folder, but the game can't handle these files well. This is causing the load times to slow down without any visual improvements. Don't worry about deleting these folders; all files are already present in the BSA.*

- Make sure you are running the latest official patch (v1.6.1820). Digital versions (Steam, GOG, Bethesda Launcher) of the game are up to date. If you are running the CD version, the correct installation order is: Morrowind / Tribunal / Bloodmoon / [Bloodmoon Patch v1.6.1820](https://cdn.bethsoft.com/elderscrolls/morrowind/patches/Bloodmoon_v1.6.1820.exe) (so skip Morrowind Patch v1.2.0722 and Tribunal Patch v1.4.1313).
     - *When you are in doubt about the version of your game; this can be found at the bottom left of the main menu in-game.*


## 3. Morrowind Code Patch
The Morrowind Code Patch fixes bugs and problems that aren't possible to do with scripting alone. This patch reduces crash and save corruption problems. In addition there are many more smaller optional fixes that cover all sorts of areas of the game.

1. [Download Morrowind Code Patch](https://www.nexusmods.com/morrowind/mods/19510)
     - *Note: Get the Standard exe version (and ignore the Python version).*

2. Extract the zip to your Morrowind root directory, the one with the Morrowind.exe program in it (not Data Files).



3. Run the Morrowind Code Patch program as administrator.
     - *Instructions: When you get to the Morrowind Code Patch.exe executable, right-click on it to view the contextual menu. Then, click or tap on Properties. In the Properties window, go to the Compatibility tab. At the bottom of the window, check the box that says "Run this program as an administrator" and then click or tap on Apply or OK.*




MCP, MGE XE,  Enhanced textures, done

You forgot Atlas and MOP

the latest nightly build of MWSE 2.1.
