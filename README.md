![version](https://img.shields.io/badge/Version-6.3-yellow?style=flat-square) ![last_modified](https://img.shields.io/github/last-commit/vel-san/kf-portable/master?style=flat-square) ![contributers](https://img.shields.io/github/contributors/vel-san/kf-portable?style=flat-square) ![size](https://img.shields.io/github/repo-size/vel-san/kf-portable?color=violet&style=flat-square) ![platforms](https://img.shields.io/badge/Platforms-Windows-blue?style=flat-square)

- [KF-PORTABLE](#kf-portable)
  - [What is included](#what-is-included)
    - [Vanilla Changes/Optmisations](#vanilla-changesoptmisations)
    - [Mutator Changes](#mutator-changes)
  - [Usage](#usage)
  - [FAQ](#faq)

# KF-PORTABLE

A pre-configured, Grey-listed *dedicated-server* **configuration** directory for Killing Floor 1

This guide assumes that you are already familiar with setting up a dedicated server via '**steamCMD**', if not, then you can simply contact me using the following:

- [Steam](https://steamcommunity.com/id/Vel-San/)
- Discord: **.Vel-San.#7468**
- [Twitter](https://twitter.com/Vel__San)
- [Other Guides](https://steamcommunity.com/id/Vel-San/myworkshopfiles/?section=guides&appid=1250)

## What is included

This directory is tailored according to my own taste of mutators.

### Vanilla Changes/Optmisations

- VAC Secured
- Edited parameters to allow downloading of Muts as compressed
- Changed the NAT value
- Changed default launch options of the server (Can be Changed to what you want)

### Mutator Changes

I currently have 2 lists of mutators in my Steam Collections:

- Grey-Listed, Minimal must-have muts that will improve player experience (Affects gameplay in several ways)
  - [Found Here](https://steamcommunity.com/sharedfiles/filedetails/?id=1913521033)
- White-listed, Minimal must-have muts that do not affect your gameplay, rather just imrpove Quality of the game
  - [Found Here](https://steamcommunity.com/sharedfiles/filedetails/?id=1490172785)

Below, you can see the currently installed (**And configured**) mods if you are using this repo:

>**WeaponPickupMessage** | Shows a message on weapon pickup, visible to all players
>
>**RgMsgMut** | Shows a message when someone rages a Scrake or a Fleshpound
>
>**MedicAlert** | Shows a message to the medic **ONLY** if someone needs healing
>
>**ESWWeightMut** | Customize the inventory weight so you can buy more weapons
>
>**CountryTags** | Shows country TAG next to names in ScoreBoard
>
>**KFARGChat** | Shows a small Chat-icon if someone is typing something
>
>**KFDamagePopup** | Shows damage popups when you hit a ZED
>
>**KFMutKillMessage** | Shows damage dealt to ZEDs
>
>**KFShareCash** | Shares the cash of disconnected or players who crashed
>
>**CleanAppIDmut** | DLC Unlocker; you can have all weapons!
>
>**ServerPerks** | A Mut that adds several optimisations to the gameplay, also, makes every Max Rank (6)
>
>**ReloadOptionsMut** | Enables you to interrupt a reload
>
>**CuteCustomes** | Adds custom OutFits in the Trader
>
>**EnhancedMusket** | A Modded version of the S. P. Musket
>
>**EnhancedSyringe** | A Modded version of the Medical Syringe, with sprint boost
>
>**WeaponStatConfig** | Configure default stats of any weapon on-the-fly from a config file
>
>**WhispColorChanger** | Change colors of the trader whisp
>
>**ZedVoiceChanger** | Adds custom ZED Sounds
>
>**ServerAdsKF** | Allows you to send Ad & Broadcast messages to all players in-game
>
>**AutoCallOut** | Show how many FPs & SCs are currently 'Spawned'
>
>**AreYouVIP** | Mark players as ViP or special in your server
>
>**ColorfulHUD** | Changes the game's HUD to a colorful fresh HUD
>
>**HardPatty** | Harder & Smarter Patty!
>
>**PattyHpBar** | Shows HP of Patty as a bar
>
>**KillStreakSounds** | Kill Streak Sounds for Comboes
>
>**FleshPoundSpinFix** | Fixes critical Fleshpound bugs
>
>**FakedPlayersPlus** | Simulates players for HoE GameDiff Modes
>
>**VisibleSpecX** | Spectators can shoot & heal enemies and players
>
>**ServerTools** | Empower your server with essential features
>
>**EnhancedScoreboard** | Adds more stats to the ServerPerks scoreboard

All of these mutators are pre-configured for the optimal experience. If you want to manually change the values and configuration of them, you can find the original files here:

- [MEGA - Default Mutators](https://mega.nz/folder/YDoEmKiC#s6FGAtgh40-TvB4bHsLaMQ)
  - If you want to upload these files to your own FTP host, you have to use **Compresser.bat** to convert them into .uz2 format - you can find the bat also in **\System**

## Usage

Alright. So, assuming you already downloaded the Repo and you have Killing Floor installed via **steamCMD** as a dedicated server.

- Navigate to your local KF-Dedicated Server directory
- Replace all files when prompted

Now we need to update the '*Vanilla*' Settings to what **YOU** want

- Open **Killingfloor.ini** with a file editor (Preferably *VSCode* or *NotePad++*)
- Press Cntrl+F (To Find a keyword)
- Search for '**Change_me**' (Without the quotes)
  - Whenever you find a Change_me keyword, replace it when what you want :)
- Now look for **KF_Server_Launcher.bat** in **\System**
  - Right click and create a desktop shortcut for it

You are done! Launch Killing Floor from steam, once it loads, go to Open the newly created KF_Server_Launcher shortcut from your desktop. You should be able to view the server once it starts inside the game (Multiplayer > Lan)

NOTE: The default config is the Modded, grey-listed mode. If you want to switch your config to Vanilla KF with no Mods at all, press ESC in-game and change the Game Mode in the Map Vote settings. You can find several pre-configured modes that i've made for you

You can join your own server, and if you have all ports properly forwarded in your router, anyone can join you!

## FAQ

- What are the ports that need forwarding?

>7707 UDP/IP (Game Port)
>
>7708 UDP/IP (Query Port)
>
>7717 UDP/IP (GameSpy Query Port)
>
>28852 TCP/IP and UDP (Allows your Server to Connect to the Master Server Browser)
>
>8075 TCP/IP (Port set via ListenPort that your WebAdmin will run on)
>
>20560 UDP/IP and TCP (Steam Port)

- How do I access WebAdmin UI?
  - In your browser, launch
    ><http://127.0.0.1:8075/ServerAdmin/>

    And enter your credentials

- How do I access ServerAdsKF UI?
  - In your browser, launch
    ><http://127.0.0.1:8075/ServerAdsKF/>

    And enter your credentials | **NOTE:** Don't forget to change my custom config in ServerAdsKF.ini!

- Will you add more mutators?
  - If the mut feels like it imrpoves the game quality and doesn't affect the gameplay then yes; Ping me on Steam with your request!

- How do I install KF in steamCMD as a dedicated server?
  - [Check this out](https://wiki.tripwireinteractive.com/index.php/Dedicated_Server_%28KillingFloor%29)

- Can I run AND play on the server?
  - Yep! Just launch Killing floor from steam first, then launch the Shortcut mentioned in the instructions above
