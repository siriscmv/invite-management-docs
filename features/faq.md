# Frequently asked questions

## Basic setup
Learn how to setup the join channel, and how to customize the template
* Use the `/config set` slash command to setup join and leave channels by providing the channel

![setting up join channel](https://i.imgur.com/kWe5qjX.gif)  
* Use the `Set as template` context menu to setup templates easily!  
* Look at [#variables](commands/config.md#variables "mention") for a list of available variables that you can use in your template.  
* You can use an embed builder like [discord.club](https://discord.club/dashboard) for making the template

![setting up join message](https://i.imgur.com/NydLETl.gif)  

## Context Menus
Learn to use context menus
* User context menus: Right click an user to view the list of commands
* Message context menus: Right click a message to view the list of commands

## Accounts command
Learn to use the accounts command to filter accounts and perform certain actions
* Provide a date for the `start-date` option, this can be a snowflake id, date in dd-mm-yyyy format or a data in human form like "10 minutes ago"  
* Set the type to either filter by creation/join date  
* You can also optionally provide an `end-date` & a `target` to filter accounts that are invited by that target  

![The accounts command](https://i.imgur.com/AV6ygSE.gif)  

## Stealing stickers
Learn how to view and steal multiple emojis & stickers at once
* Use the `emojis` command (available as a normal command & context menu command) on stickers/emojis to view & steal them!  
* Normal command: You can either provide the emoji/sticker while using the command or reply to an existing message  
* Context Menu command: Right click the message that conttains the stickers/emojis -> Apps -> Emojis  

![The emojis command](https://i.imgur.com/ZGbHMS2.gif)

## Resetting invites
Learn how to reset invites
* To reset invites for everyone leave the argument empty  
* To reset invites for a specific user, mention that user as argument 

![The reset command](https://i.imgur.com/g9Eom1k.gif)

## Blacklisting channels
Prevent members from using bot commands in specific channels
* Use the `/config blacklist channel` slash command to blacklist a specific channel  
* To unblacklist a channel, run the same slash command again  
* Note: Members with `MANAGE_GUILD` perms can still use commands in blacklisted channels  

![Blacklisting a channel](https://i.imgur.com/BJu2VOB.gif)