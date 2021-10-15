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

