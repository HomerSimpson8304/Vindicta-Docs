---
layout: default
title: Alternative Save Game Storage
nav_order: 9
---

# Alternative Save Game Storage with FileXT addon

By default saved games are stored in your `.vars.arma3profile file`.

You can also save files into separate files if you install this addon:
[FileXT at Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=2162811561)
Currently it only supports x86 and x64 Windows Arma builds.

# Advantages

Advantages over `.vars.arma3profile` storage:
- Easy to manage and share saved games. Just move them between folders or send them to friends or anyone.
- Arma won't randomly damage these files, compared to `.vars.arma3profile`.
- Unlimited amount of saved games.
- Better performance for host, because Arma won't re-read these files for different reasons compared with `.vars.arma3profile`.
Reading `.vars.arma3profile` might freeze the game up to a few seconds when there are many saved games there.


# Setup

Setup is simple, just install this addon on the machine which hosts the mission:

- If you are using a dedicated server, this addon is required only on the server. Launch it with `-serverMod=` command line option.

- If you are hosting the game from your client, then only the host needs to install this addon.

- Same for singleplayer.

# Usage

When you open the `Savegame` tab, you will see a combobox which lets you choose the storage method.
The menu tab shows only saved games available through the selected storage method.
If FileXT is loaded, it will be selected by default. Just ensure that it is selected when you make a new save.

# Porting saved games from `.vars.arma3profile file` to FileXT
When you start your game, select `Profile` storage and load your old saved game. Then select `FileXT` and re-save it.