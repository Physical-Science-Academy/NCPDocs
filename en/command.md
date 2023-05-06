---
title: Commands
description: The Usages of Commands in NCP
published: true
date: 2023-05-06T23:59:15.902Z
tags: 
editor: markdown
dateCreated: 2023-05-06T23:53:55.834Z
---

# Command
Overall, NCP has the following commands.
- `/ncp` get the version info

- `/ncp version` get the version info

- `/ncp reload` reload the config currently

- `/ncp debug` toggle the debug mode

- `/ncp ban` ban a player

- `/ncp unban` unban a player

- `/ncp kick` kick a player

- `/ncp toggle` Switch detection

- `/ncp permission` manage permissions.


### root command
When you enter the main command `/ncp` in the server, the plug-in will output all commands owned by the current NCP. Of course, if there is a command that is not explained by NCP, it may be because you have installed an extension or an additional command added by a component.

### version command
execute `/ncp version`

This command is used to query the current NCP version information.

### reload command
excute `/ncp reload`

Use this command to hot overload some parameters in your NCP configuration. Of course, it can't reload all the data, so you'd better restart your Nukkit server.

### debug command
excute `/ncp debug`

This is the developer debugging command of NCP. Enter it to switch the debug mode. In debug mode, NCP will output some detection information. So, please don't turn on this function for the server in your production environment!

### ban command
excuse:
- `/ncp ban player) days`