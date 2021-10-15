---
description: List of configuration commands
---

# `bonus-invites`

{% tabs %}
{% tab title="Slash" %}

* `/bonus-invites add <target> <invites>` - Add invites to the target user
* `/bonus-invites remove <target> <invites>` - Remove invites from the target user

![Adding bonus invites](https://cdn.discordapp.com/attachments/889530273618886686/898193226832412702/unknown.png) ![Removing bonus invites](https://cdn.discordapp.com/attachments/889530273618886686/898193447494770718/unknown.png)

{% endtab %}
{% endtabs %}

# `config`

{% tabs %}
{% tab title="Slash" %}

* `/config view setting <setting>` - View the specified setting
* `/config set join-channel <channel>` - Set the channel where join message are sent
* `/config set leave-channel <channel>` - Set the channel where leave messages are sent
* `/config set join-msg <template>` - Set the template for join messages
* `/config set leave-msg <template>` - Set the template for leave messages
* `/config reset setting <setting>` - Reset the specified setting
* `/config blacklist channel <channel>` - Blacklist/Unblacklist a specific channel such that commands can/cannot be used in the specified channel
* `/config test message <type>` - Send a test join/leave message

![Setting up the join channel](https://cdn.discordapp.com/attachments/889530273618886686/898137361412657152/unknown.png) ![Setting up the leave channel](https://media.discordapp.net/attachments/889530273618886686/898137443440685056/unknown.png) 
![Setting up the join message template](https://cdn.discordapp.com/attachments/889530273618886686/898196313391398912/unknown.png) ![Setting up the leave message template](https://cdn.discordapp.com/attachments/889530273618886686/898196571559174195/unknown.png) 
![Resetting the join-channel setting](https://media.discordapp.net/attachments/889530273618886686/898197130798301264/unknown.png?width=1440\&height=141) 
![Blacklisting a specific channel](https://cdn.discordapp.com/attachments/889530273618886686/898197527671758848/unknown.png) 
![Sending a test join message](https://cdn.discordapp.com/attachments/889530273618886686/898197584865267712/unknown.png)

{% endtab %}
{% endtabs %}

{% hint style="warning" %}
Please use the [#set-as-template](context-menu-commands.md#set-as-template "mention") command for setting up join / leave message templates. It is much easier to use and also supports multi-line input.^
{% endhint %}

# `reset`

{% tabs %}
{% tab title="Slash" %}

* `/reset <target>` - Resets invites of the specified target user
* `/reset` - Reset invites for everyone (when \<target> is not specified)

![Resetting invites for everyone](https://cdn.discordapp.com/attachments/889530273618886686/898200612422942720/unknown.png) ![Resetting invites for a specific user ](https://cdn.discordapp.com/attachments/889530273618886686/898200657239097364/unknown.png)

{% endtab %}

{% tab title="Normal" %}

* **Aliases**: `resetinvites`
* **Usage**: `reset <target>` - if target is an userID / mention, only that specific user's invites will be reset, if it is left empty or "all" it will reset everyone's invites

{% endtab %}
{% endtabs %}

# `Set as template`

{% tabs %}
{% tab title="Context Menu" %}

* Send the template using variables (from the `/variables` slash command) as a normal message
* Right click the message that you just sent, click on `Apps` then `Set as template` 
* Choose the type of template that you are trying to set

![Setting up join messages using the Set as template context menu command](https://cdn.discordapp.com/attachments/889530273618886686/894923573788024903/joinmsg.gif)

{% endtab %}
{% endtabs %}

# `setprefix`

{% tabs %}
{% tab title="Normal" %}

* **Usage**: `setprefix <new-prefix>` - Sets the bot's prefix to `new-prefix`

![Setting the bot prefix to ;](https://cdn.discordapp.com/attachments/889530273618886686/898223916257009684/unknown.png)

{% endtab %}
{% endtabs %}

# `variables`

{% tabs %}
{% tab title="Slash" %}

* `/variables` - View a list of all available variables that you can use to customise join / leave message templates 

![Viewing a list of variables](https://cdn.discordapp.com/attachments/889530273618886686/898201384934051860/unknown.png)

{% endtab %}
{% endtabs %}