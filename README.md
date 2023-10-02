[![version](https://img.shields.io/github/v/release/Vel-San/killing-floor-portable?label=version&style=flat-square)](https://github.com/Vel-San/killing-floor-portable/releases) ![last_modified](https://img.shields.io/github/last-commit/vel-san/kf-portable/master?style=flat-square) ![contributers](https://img.shields.io/github/contributors/vel-san/kf-portable?style=flat-square) ![size](https://img.shields.io/github/repo-size/vel-san/kf-portable?color=violet&style=flat-square)


- [KF-PORTABLE](#kf-portable)
  - [IMPORTANT NOTE FOR CLONING](#important-note-for-cloning)
  - [What is included](#what-is-included)
    - [Vanilla Changes/Optmisations](#vanilla-changesoptmisations)
    - [Mutator Changes](#mutator-changes)
  - [Usage](#usage)
    - [Disabling/Enabling Mutators](#disablingenabling-mutators)
  - [FAQ](#faq)

# KF-PORTABLE

> A pre-configured, Grey-listed *dedicated-server* **configuration** directory for Killing Floor 1

This guide assumes that you are already familiar with setting up a dedicated server via '**steamCMD**', if not, then you can simply contact me using the following:

- [Steam](https://steamcommunity.com/id/Vel-San/)

## IMPORTANT NOTE FOR CLONING

Use the following command in case you want to clone the repo (to avoid cloning it's history, which is about ~600mbs)

```
git clone --depth 1 https://github.com/Vel-San/killing-floor-portable.git
```

## What is included

This directory is tailored according to my own taste of mutators.

### Vanilla Changes/Optmisations

- VAC Secured
- Edited parameters to allow downloading of Muts as compressed
- Changed the NAT value
- Changed default launch options of the server (Can be Changed to what you want)

### Mutator Changes

Below, you can see the currently installed (**And configured**) mods if you are using this setup:

>**WeaponPickupMessage** | Shows a message on weapon pickup, visible to all players
>
>**RgMsgMut** | Shows a message when someone rages a Scrake or a Fleshpound
>
>**MedicAlert** | Shows a message to the medic **ONLY** if someone needs healing
>
>**CountryTags** | Shows country TAG next to names in ScoreBoard
>
>**DamagePopup** | Shows damage popups when you hit a ZED
>
>**MutKillMessage** | Shows damage dealt to ZEDs
>
>**ShareCash** | Shares the cash of disconnected or players who crashed
>
>**CleanAppID** | DLC Unlocker; you can have all weapons!
>
>**ServerPerks** | A Mut that adds several optimisations to the gameplay, also, makes every Max Rank (6)
>
>**ReloadOptionsSP** | Enables you to interrupt a reload (Supports ServerPerks)
>
>**CuteCustomes** | Adds custom outfits in the Trader
>
>**WeaponStatConfig** | Configure default stats of any weapon on-the-fly from a config file
>
>**WhispColorChanger** | Change colors of the trader whisp
>
>**ServerAdsKF** | Allows you to send Ad & Broadcast messages to all players in-game
>
>**AutoCallOut** | Show how many FPs & SCs are currently 'Spawned'
>
>**AreYouVIP** | Mark players as ViP or special in your server
>
>**PattyHpBar** | Shows HP of Patty as a bar
>
>**FleshPoundSpinFix** | Fixes critical Fleshpound bugs
>
>**VisibleSpecX** | Spectators can shoot & heal enemies and players
>
>**ServerTools** | Empower your server with essential features
>
>**EnhancedScoreboard** | Adds more stats to the ServerPerks scoreboard
>
>**NFN** | Nanu Fucking Nanu GameType + Mut; Increased Difficulty
>
>**StartLoadout** | Change starting loadout for all perks
>
>**MutLoaderV2** | Load mutators without MapVote or Server Launch Command
>
>**HUDEffects** | Removes some annoying HUD Effects for all clients
>
>**ServerAcheivments** | Adds custom & vanilla achievments support
>
>**ColorfulHUD** | Pretty HUD ;D
>
>**Chat Icons** | Pretty, animated chat icons when a player is typing
>
>**MaxPlayers** | Increases server slots
>
>**SoundBoard** | Play various sound effects in-game, can be set as keybinds for inputs
>
>**KFPatcher** | Fix most gamebreaking bugs and ads some QoL tweaks

All of these mutators are pre-configured for the optimal experience. If you want to manually change the values and configuration of them, you can find the original files here:

## Usage

Alright. So, assuming you already cloned/downloaded the Repo and you have Killing Floor installed via **steamCMD** as a dedicated server.

- Navigate to your local KF-Dedicated Server directory
- Replace all files when prompted (Except `Killingfloor.ini`)

Now we need to update the '*Vanilla*' Settings to what **YOU** want

- Open **Killingfloor.ini** with a file editor (Preferably *VSCode* or *NotePad++*)
- Press Cntrl+F (To Find a keyword)
- Search for '**Change_me**' (Without the quotes)
  - Whenever you find a Change_me keyword, replace it with what you want :)
  - Replace *or* add all other values that are present in `Killingfloor.ini` from this repo, into the default `Killingfloor.ini`
- Now look for **KF_Server_Launcher.bat** in **\System**
  - Right click and create a desktop shortcut for it

### Disabling/Enabling Mutators

Navigate to `MutLoader.ini`:

- Change the configs to whatever you want. Each config works according to the GameDifficulty votes from your MapVotes
  - Here you can enable/disable mutators
  - Here you can change your ServerName with every MapVote you do. For more, check [MutLoader v2.1](https://steamcommunity.com/sharedfiles/filedetails/?id=2286683680)

You are done! Launch Killing Floor from steam, once it loads, launch the newly created **KF_Server_Launcher** shortcut from your desktop. You should be able to view the server once it starts inside the game.

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
  - Yep! Just launch Killing floor from steam first, then launch the Shortcut mentioned in the instructions above.

- Does this config work on Steam's Killingfloor (and not steamCMD)
  - Yep! Just do the same steps.

- Where can I get the compressed (.uz2) files from?
  - You can find everything (as long as it is hosted by me) in this [Redirect-URL](https://kf-server.000webhostapp.com/redirect/)
