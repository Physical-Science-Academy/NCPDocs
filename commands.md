---
title: Commands
description: The Usages of Commands in NCP
published: true
date: 2023-05-07T10:07:09.172Z
tags: 
editor: markdown
dateCreated: 2023-05-06T23:53:55.834Z
---

Overall, NCP has the following commands.
**Arguments in [ ] are considered optional.**
- `/ncp` Shows the available commands and their arguments.

- `/ncp version` Shows the version info of the plugin.

- `/ncp reload` Reloads the current config file.

- `/ncp debug` Toggles the Debug mode.

- `/ncp ban (playername) (days) [hours] [minutes]` Bans a player by his name

- `/ncp unban (playername)` Unbans a player by his name

- `/ncp kick` Kicks an online player

- `/ncp toggle (checkTypeName)` Enables/Disables a given Check

- `/ncp permission (create/remove) (checkTypeName) (permissionName)` Creates or removes a permission that allows bypassing the provided check.


### root command
When you enter the main command `/ncp` in the console, the plugin will output all commands owned by the current NCP. Of course, if there is a command that is not explained by NCP, it may be because you have installed an extension or an additional command added by a component.

### version command
execute `/ncp version`
This command is used to output the current NCP version information.

### reload command
excute `/ncp reload`

Use this command to hot reload some parameters in your NCP configuration. Of course, it can't reload all the data, so you'd better restart your Nukkit server.

### debug command
excute `/ncp debug`

This is the developer debugging command of NCP. Enter it to switch the debug mode. In debug mode, NCP will output some detection information. So, please don't turn on this function for the server in your production environment!

### ban command
excute:
- `/ncp ban (playername) (days)`
- `/ncp ban (playername) (days) (hours)`
- `/ncp ban (playername) (days) (hours) (minutes)`

Use this command to ban players temporarily from your server. You can customize the Banning Module in the `config`.

### unban command
excute `/ncp unban (playername)`

Unbans a player that was banned by `/ncp ban`.

### kick command
excute `/ncp kick (playername)`

Allows to kick a currently online player from your server.

### toggle command
execute `/ncp toggle (checkTypeName)`

Allows to disable or enable a Check registered in NCP. A list of Checks is displayed on server startup. The `checkTypeName` is the uppercase name of the Check Module (for example `MOVING_CREATIVE_FLY`).
```
[INFO ] [NoCheatPlus] Loading module: MOVING_CREATIVE_FLY 1.0.0
[INFO ] [NoCheatPlus] Loading module: MOVING_NO_FALL 1.0.0
[INFO ] [NoCheatPlus] Loading module: MOVING_VEHICLE 1.0.0
[INFO ] [NoCheatPlus] Loading module: MOVING_SPEED 1.0.0
[INFO ] [NoCheatPlus] Loading module: FIGHT_SPEED 1.0.0
...
```

### permission command
execute `/ncp permission (create/remove) (checkTypeName) (permissionName)`

Allows to create / remove a permission which, if assigned to a player, enables the player to bypass the provided Check (provided by argument `checkTypeName`). To assign the created permission, you will need a Permission Manager like [LuckPerms](https://cloudburstmc.org/resources/luckperms.51/).
