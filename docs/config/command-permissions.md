# Managing commands

!!! info
    Please consider using the Dashboard at [https://discord.com/channels/1013018020899192892/1013058418971516939] it is much, much easier for this and allows for per-command customization *far* beyond what commands offer.

!!! info
    Restricted commands require a bot channel to be set up.

| Name | Example | Usage |
| :ava |:!warn | :warning someone |
| **ignore [channels...] [commands...]**  | !ignore #general #log #adminsonly "temp home" ping activity | If no channel is specified, the current channel is ignored. If a command is supplied, it will ignore that command in the specified channel. Manage server bypasses this. You can supply more than one channel and or command. |
| **ignore server** | !ignore server | This is essentially the same as making the entire bot mod-only |
| **ignore all [commands...]**  | !ignore all "pc top" ping | This is equal to typing !ignore channel command subcommand in all channels the bot can see, useful if you want to ignore a command in all channels except for one. This will not work for channels created in the future. If the command is already ignored in a channel, this will unignore it. |
| **unignore [channels...] [command...]** | !unignore \#general \#log temp ping | Reverses what !ignore does |
| **unignore all** | !unignore all | Unignores all channels \(this does not take ignored commands into account\) |
| **disable &lt;commands...&gt;** | !disable "pc top" rr temp | This really disables the command globally from the server, not even manage server bypasses this. |
| **enable &lt;commands...&gt;** | !enable "pc top" ping "tag info" | Enables one or more previously disabled commands. |
| **enable all** | !enable all | Sets all commands to enabled. |
| **disable all** | !disable all | Sets all commands to disabled. |
| **enable mod** | !enable mod | Enables all moderation commands |
| **disable mod** | !disable mod | Disables all moderation commands |
| enable list | !enable list | Shows all enabled/disabled commands. |
| **restrict &lt;command&gt;** | !restrict define | This requires a bot channel to utilize. Makes it so that if the command is used outside of the bot channel, the bot will ping the user in the botchannel and give the results there instead. |
| **unrestrict &lt;command&gt;** | !unrestrict d | Unrestricts it. Like all commands where you pass in a command, aliases work just as well. |
| **set bot &lt;channel&gt;** | !set bot \#botspam | Sets the channel used for restricted commands to be redirected to. |
| **modonly &lt;command&gt;** | !modonly echo | Makes a command usable by mods only |
| **unmodonly &lt;command&gt;** | !unmodonly dog | Removes a command from the modonly list |
| **modrole &lt;role&gt;** | !modrole bot commander | Makes it so that any member with the specified role is seen as a moderator by the bot. This does not allow members with this role to kick, ban, mute, warn or any variation of these commands. |
| **modrole clear** | !modrole clear | Removes the modrole |

