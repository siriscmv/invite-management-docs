---
description: List of slash commands
---

# Slash Commands

{% tabs %}
{% tab title="Config" %}
## Config commands



### `/bonus-invites`

* `/bonus-invites add <target> <invites>` - Add invites to the target user
* `/bonus-invites remove <target> <invites>` - Remove invites from the target user

![Adding bonus invites](https://cdn.discordapp.com/attachments/889530273618886686/898193226832412702/unknown.png) ![Removing bonus invites](https://cdn.discordapp.com/attachments/889530273618886686/898193447494770718/unknown.png)

### `/reset`

* `/reset <target>` - Resets invites of the specified target user
* `/reset` - Reset invites for everyone (when \<target> is not specified)

![Resetting invites for everyone](https://cdn.discordapp.com/attachments/889530273618886686/898200612422942720/unknown.png) ![Resetting invites for a specific user ](https://cdn.discordapp.com/attachments/889530273618886686/898200657239097364/unknown.png)

### `/variables`

* `/variables` - View a list of all available variables that you can use to customise join / leave message templates 

![Viewing a list of variables](https://cdn.discordapp.com/attachments/889530273618886686/898201384934051860/unknown.png)





### `/config`

* `/config view setting <setting>` - View the specified setting
* `/config set join-channel <channel>` - Set the channel where join message are sent
* `/config set leave-channel <channel>` - Set the channel where leave messages are sent
* `/config set join-msg <template>` - Set the template for join messages
* `/config set leave-msg <template>` - Set the template for leave messages
* `/config reset setting <setting>` - Reset the specified setting
* `/config blacklist channel <channel>` - Blacklist/Unblacklist a specific channel such that commands can/cannot be used in the specified channel
* `/config test message <type>` - Send a test join/leave message





{% hint style="warning" %}
Please use the [#set-as-template](context-menu-commands.md#set-as-template "mention") command for setting up join / leave message templates. It is much easier to use and also supports multi-line input.^
{% endhint %}





![Setting up the join channel](https://cdn.discordapp.com/attachments/889530273618886686/898137361412657152/unknown.png) ![Setting up the leave channel](https://media.discordapp.net/attachments/889530273618886686/898137443440685056/unknown.png) ![Setting up the join message template](https://cdn.discordapp.com/attachments/889530273618886686/898196313391398912/unknown.png) ![Setting up the leave message template](https://cdn.discordapp.com/attachments/889530273618886686/898196571559174195/unknown.png) ![Resetting the join-channel setting](https://media.discordapp.net/attachments/889530273618886686/898197130798301264/unknown.png?width=1440\&height=141) ![Blacklisting a specific channel](https://cdn.discordapp.com/attachments/889530273618886686/898197527671758848/unknown.png) ![Sending a test join message](https://cdn.discordapp.com/attachments/889530273618886686/898197584865267712/unknown.png)
{% endtab %}

{% tab title="General" %}
## General commands



* `/faq` - Get a list of frequently asked questions 
* `/help` - Shows a list of commands with their description, mentioning a specific command will show more information about that particular command
* `/invite` - Get the bot's invite link
* `/ping` - Shows the bot's ping (latency)
* `/prefix` - Shows the bot's current prefix 
* `/stats` - View some stats related to the bot

![The help command](https://cdn.discordapp.com/attachments/889530273618886686/898202869898027038/unknown.png) ![The stats command](https://cdn.discordapp.com/attachments/889530273618886686/898202960536952892/unknown.png)
{% endtab %}

{% tab title="Invites" %}
## Invites commands



* `/invitecodes <target>` - List of the target user's invite codes
* `/invited <target>` - Get a list of users invited by the target user
* `/inviteinfo <invite-link>` - Get information about an Invite link
* `/inviter <target>` - Find the person who invited the target user
* `/invites <target>` - Get the invite count of the target user 
* `/leaderboard` - List of top inviters in your server



![The inviter command](https://cdn.discordapp.com/attachments/889530273618886686/898207843960913990/unknown.png)

{% hint style="info" %}
`<target>` is optional. If not specified, it will default to the user who used the slash command
{% endhint %}
{% endtab %}

{% tab title="Utility" %}
## Utility commands



### `/accounts`

* `/accounts <start-date> <type> <end-date> <target>` - Filter accounts that either joined / were created (depending on `type`) after `start-date`, before `end-date` and were invited by `target.`
* `<end-date>` is optional and defaults to current date
* `<target>` is optional and defaults to everyone (ie) all accounts
* The dates can be in any format, example: "10 minutes ago", "10 days ago", "02-09-2021"

![This command will filter accounts that joined b/w 5-10 days ago and were invited by liamm.](https://cdn.discordapp.com/attachments/889530273618886686/898208628857765989/unknown.png)



### `/avatar`

* `/avatar <target> <hide-reply>` - Shows the **avatar, server avatar and banner** of the target user, if `hide-reply` is `true` the response will be ephemeral (can be seen only by you)



### `/membercount`

* `/membercount` - Shows the member count of the server along with more statistics and a beautiful graph



### `/userinfo`

* `/userinfo <target>` - Shows detailed information about any user, such as tag, avatar, roles, invites count, inviter, account age, badges, etc.
{% endtab %}
{% endtabs %}

{% hint style="info" %}
`<>` refers to user input. For example `<target>` refers to a user that is supposed to be entered while using the command. Most of these arguments are also optional
{% endhint %}

