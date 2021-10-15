---
description: List of utility commands
---

# `accounts`

{% tabs %}
{% tab title="Slash" %}

* `/accounts <start-date> <type> <end-date> <target>` - Filter accounts that either joined / were created (depending on `type`) after `start-date`, before `end-date` and were invited by `target.`
* `<end-date>` is optional and defaults to current date
* `<target>` is optional and defaults to everyone (ie) all accounts
* The dates can be in any format, example: "10 minutes ago", "10 days ago", "02-09-2021". It also accepts a discord snowflake ID (message / user ids for example)

![This command will filter accounts that joined b/w 5-10 days ago and were invited by liamm.](https://cdn.discordapp.com/attachments/889530273618886686/898208628857765989/unknown.png)

{% endtab %}
{% endtabs %}

# `avatar`

{% tabs %}
{% tab title="Slash" %}

* `/avatar <target> <hide-reply>` - Shows the **avatar, server avatar and banner** of the target user, if `hide-reply` is `true` the response will be ephemeral (can be seen only by you)

![Getting the avatar with hide-reply set to true](https://cdn.discordapp.com/attachments/889530273618886686/898614232172625960/unknown.png)

{% endtab %}

{% tab title="Normal" %}

* **Aliases**: `av`, `pfp`, `banner`
* **Usage**: `avatar <target>` - Shows the **avatar, server avatar and banner** of the target user

{% endtab %}

{% tab title="Context Menu" %}

* Go to the profile of the target user
* Right click them, then `Apps`, then `Avatar`

{% endtab %}

{% endtabs %}

# `emojis`

{% tabs %}
{% tab title="Normal" %}

* **Aliases**: `stickers`, `steal`
* **Usage**: `emojis <emojis...>` - Get a list of all emojis & stickers that are provided, along with a steal button! 
* You can also use the command while replying to an existing message to extract emojis & stickers from that message too

![Using the emojs command while replying to another message](https://cdn.discordapp.com/attachments/889530273618886686/898232104301764639/unknown.png)

{% endtab %}

{% tab title="Context Menu" %}

* Go to the target message (that contains the emojis/stickers)
* Right click it, then `Apps`, then `Emojis`

{% endtab %}
{% endtabs %}

# `membercount`

{% tabs %}
{% tab title="Slash" %}

* `/membercount` - Shows the member count of the server along with more statistics and a beautiful graph

![The membercount command](https://cdn.discordapp.com/attachments/889530273618886686/898614853093179504/unknown.png)

{% endtab %}

{% tab title="Normal" %}

* **Aliases**: `mc`
* **Usage**: `membercount` - Shows the member count of the server along with more statistics and a beautiful graph

{% endtab %}
{% endtabs %}

# `userinfo`

{% tabs %}
{% tab title="Slash" %}

* `/userinfo <target>` - Shows detailed information about any user, such as tag, avatar, roles, invites count, inviter, account age, badges, etc.

![The userinfo command](https://cdn.discordapp.com/attachments/889530273618886686/898615537414864896/unknown.png)

{% endtab %}

{% tab title="Normal" %}

* **Aliases**: `ui`, `whois`
* **Usage**: `userinfo <target>` - Shows detailed information about any user, such as tag, avatar, roles, invites count, inviter, account age, badges, etc.

{% endtab %}

{% tab title="Context Menu" %}

* Go to the profile of the target user
* Right click them, then `Apps`, then `Userinfo`

{% endtab %}
{% endtabs %}

{% hint style="success" %}
Normal commands are supposed to be used with a prefix. The default prefix for normal commands is the bot's mention ( **`@Invite Management#6068`** ) and **`+`**
{% endhint %}