---
description: Some frequently asked questions about the bot
cover: .gitbook/assets/Quepal.jpg
coverY: 0
---

# FAQ

## Basic setup

Learn how to setup the join channel, and how to customize the template  

### Settings up join/leave channels:  
* Use the `/config set` slash command to setup join and leave channels by providing the channel

![setting up join channel](https://i.imgur.com/kWe5qjX.gif)  

### Setting up join/leave messages:  

{% hint style="info" %}
The bot has a default template which will be used as soon as you set the join or leave channel. Follow the below steps if you wish to customize the default templates
{% endhint %}  

* Look at [#variables](commands/config.md#variables "mention") for a list of available variables that you can use in your template.
* You can use the `/embed build` command for designing the template, or download premade json templates from this [repo](https://github.com/Siris01/invite-management-templates) and use the `/embed send <channel> <json>` command to send the template to the channel. 
* Once you are done designing the template, send it in any channel and then use the [#set-as-template](commands/config.md#set-as-template "mention") command on the message that you just sent (Right click -> Apps -> Set as template)

![setting up join message](https://i.imgur.com/UkT1EYv.gif)

## Context Menus

Learn to use context menus

* User context menus: Right click an user to view the list of commands
* Message context menus: Right click a message to view the list of commands

## Accounts command

Learn to use the accounts command to filter accounts and perform certain actions

* Provide a date for the `start-date` option, this can be a discord snowflake id, date in dd-mm-yyyy format or a data in human form like "10 minutes ago"
* Set the type to either filter by creation/join date
* Additionally you can filter out only the users that are not verified by setting the verified option to False
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

## Auto-refresh leaderboard

Setup an invites lb that refreshes itself automatically. It also has a handy "check invites" button.

* Use the `/config auto-refresh-leaderboard set <channel>` slash command to set the channel where the lb is to be sent
* To disabled it, run the `/config auto-refresh-leaderboard reset` command
* Note: You can have only 1 auto-refresh lb per server

![Auto-refresh lb](https://i.imgur.com/ufCR3O7.gif)

## Verification System

There are currently 3 types of verification:

* **Simple**: Members will have to press a button to get verified This type is effective against automated user accounts.
* **Password**: Set a pre-defined password which the user has to enter (using buttons) to get verified. Useful if you own a super exclusive server or you just want to hide the password in your rules, ensuring that all new members will actually read your server's rules :)
* **Randomised**: Make the bot randomise the password (of specified length) which the user has to enter (using buttons) to get verified.

Setting up the verification system:

![Simple verification](https://i.imgur.com/9UK9igo.png) ![Password verification: 12159](https://i.imgur.com/9OT6UKr.png) ![Randomised password of length 4](https://i.imgur.com/mRGJmt4.png)

Note:

* `role` is the role which will be given upon successful verification.
* `channel` is the channel where the verification embed will be sent.
* The embed can be customized by providing a json file in the `/config verification` command. This is restricted to premium tiers 2 and 3
