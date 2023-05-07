---
title: Commands
description: The Usages of Commands in NCP
published: true
date: 2023-05-07T09:55:20.672Z
tags: 
editor: markdown
dateCreated: 2023-05-06T23:53:55.834Z
---

# Command
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

Use this command to hot overload some parameters in your NCP configuration. Of course, it can't reload all the data, so you'd better restart your Nukkit server.

### debug command
excute `/ncp debug`

This is the developer debugging command of NCP. Enter it to switch the debug mode. In debug mode, NCP will output some detection information. So, please don't turn on this function for the server in your production environment!

### ban command
excute:
- `/ncp ban (player) (days)`
- `/ncp ban (player) (days) (hours)`
- `/ncp ban (player) (days) (hours) (minutes)`

Use this command to have NCP block some players on your server. Also, you can customize the ban.

### unban command
excute `/ncp unban (player)`

Lift the ban of a player banned by NCP.

### kick command
excute `/ncp kick (player)`

Kick out an online game through NCP.

### toggle command
