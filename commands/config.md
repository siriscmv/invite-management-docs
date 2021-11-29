---
description: List of configuration commands
---

# Config

## `bonus-invites`

{% tabs %}
{% tab title="Slash" %}
* `/bonus-invites add <target> <invites>` - Add invites to the target user
* `/bonus-invites remove <target> <invites>` - Remove invites from the target user

![Adding bonus invites](https://i.imgur.com/MlrJa9L.png)
{% endtab %}
{% endtabs %}

## `config`

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

![Setting up the join channel](https://i.imgur.com/nmF3XTD.png) ![Setting up the leave channel](https://i.imgur.com/YHx8BcL.png) ![Resetting the join-channel setting](https://i.imgur.com/WJEdmjy.png) ![Blacklisting a specific channel](https://i.imgur.com/zEQz6Zf.png) ![Sending a test join message](https://i.imgur.com/3VNOccd.png)
{% endtab %}
{% endtabs %}

{% hint style="warning" %}
Please use the [#set-as-template](config.md#set-as-template "mention") command for setting up join / leave message templates. It is much easier to use and also supports multi-line input.
{% endhint %}

## `reset`

{% tabs %}
{% tab title="Slash" %}
* `/reset <target>` - Resets invites of the specified target user
* `/reset` - Reset invites for everyone (when \<target> is not specified)

![The reset command](https://i.imgur.com/g9Eom1k.gif)
{% endtab %}

{% tab title="Normal" %}
* **Aliases**: `resetinvites`
* **Usage**: `reset <target>` - if target is an userID / mention, only that specific user's invites will be reset, if it is left empty or "all" it will reset everyone's invites
{% endtab %}
{% endtabs %}

## `Set as template`

{% tabs %}
{% tab title="Context Menu" %}
* Send the template using variables (from the `/variables` slash command) as a normal message. Click on [#variables](config.md#variables "mention") for a list of variables
* Right click the message that you just sent, click on `Apps` then `Set as template`
* Choose the type of template that you are trying to set

![Setting up join messages using the Set as template context menu command](https://i.imgur.com/BOvkzue.gif)
{% endtab %}
{% endtabs %}

## `setprefix`

{% tabs %}
{% tab title="Normal" %}
* **Usage**: `setprefix <new-prefix>` - Sets the bot's prefix to `new-prefix`

![Setting the bot prefix to ;](https://i.imgur.com/WxWHM9L.png)
{% endtab %}
{% endtabs %}

## `variables`

{% tabs %}
{% tab title="Slash" %}
* `/variables` - View a list of all available variables that you can use to customise join / leave message templates  

**List of variables:** 
* `user_id` - The ID of the user who joined (example: `581451736305106985`)
* `user_tag` - The tag of the user who joined (example: `Siris#1337`)
* `user_mention` - The metion of the user who joined (example: `<@581451736305106985>`)
* `user_created_date` - The relative date when the user's account was created
* `user_joined_date` - The relative date when the user joined 
* `inviter_id` - The ID of the inviter
* `inviter_tag` - The tag of the inviter
* `inviter_mention` - The mention of the inviter
* `inviter_invites_total` - The Total invite count of the inviter
* `inviter_invites_joins` - The amount of joins the inviter has
* `inviter_invites_leaves` - The amount of leaves the inviter has
* `inviter_invites_bonus` - The amount of bonus invites the inviter has
* `invite_code` - The invite code that was used by the user to join
* `invite_channel` - The channel from which the invite code was created
* `invite_uses` - The number of uses the invite code has
* `guild_name` - The name of the server
* `guild_membercount` - The total number of members present in the server

**Note:** The variables are supposed to be include in `${}` (example: `${inviter_tag}`)
{% endtab %}
{% endtabs %}

{% hint style="success" %}
Normal commands are supposed to be used with a prefix. The default prefix for normal commands is the bot's mention ( **`@Invite Management#6068`** ) and **`+`**
{% endhint %}