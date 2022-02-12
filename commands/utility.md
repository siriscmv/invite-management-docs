---
description: List of utility commands
cover: ../.gitbook/assets/Summer Dog.jpg
coverY: 0
---

# Utility

## `accounts`

{% tabs %}
{% tab title="Slash" %}
* `/accounts <start-date> <type> <end-date> <verified> <target>` - Filter [verified / unverified] accounts that either joined / were created (depending on `type`) after `start-date`, before `end-date` and were invited by `target.`
* `<end-date>` is optional and defaults to current date
* `<verified>` filters accounts that are either verified or unverified. If empty, verification status is ignored.
* `<target>` is optional and defaults to everyone (ie) all accounts
* The dates can be in any format, example: "10 minutes ago", "10 days ago", "02-09-2021". It also accepts a discord snowflake ID (message / user ids for example)

![This command will filter unverified accounts that joined b/w 3-5 days ago and were invited by Siris](https://i.imgur.com/7Ydp5Wr.png)
{% endtab %}
{% endtabs %}

## `avatar`

{% tabs %}
{% tab title="Slash" %}
* `/avatar <target> <hide-reply>` - Shows the **avatar, server avatar and banner** of the target user, if `hide-reply` is `true` the response will be ephemeral (can be seen only by you)

![Getting the avatar with hide-reply set to true](https://i.imgur.com/YOJZMz2.png)
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

## `embed`

{% tabs %}
{% tab title="Slash" %}
* `/embed send <channel> <json>` - Sends an embed message constructed using the json file provided to the specified channel
* `/embed build <json>` - Opens an interactive interface that allows you to design embeds. A json file can also be provided to edit that embed instead of starting from scratch
* `/embed source <id>` - Gets the raw json of a message from the current channel with the specified id

![The embed commands](https://i.imgur.com/H7fCo7D.png)
{% endtab %}
{% endtabs %}

## `emojis`

{% tabs %}
{% tab title="Normal" %}
* **Aliases**: `stickers`, `steal`
* **Usage**: `emojis <emojis...>` - Get a list of all emojis & stickers that are provided, along with a steal button!
* You can also use the command while replying to an existing message to extract emojis & stickers from that message too

![Using the emojs command while replying to another message](https://i.imgur.com/QiT6Urp.png)
{% endtab %}

{% tab title="Context Menu" %}
* Go to the target message (that contains the emojis/stickers)
* Right click it, then `Apps`, then `Emojis`
{% endtab %}
{% endtabs %}

### `info`

{% tabs %}
{% tab title="Slash" %}
* `/info channel <target>` - Get information about the target channel like type, position, etc
* `/info colour <target>` - Get information about the target colour like hex String, int value, complementary colours, etc
* `/info invite <link>` - Get information about the target link like server name, created at, etc
* `/info role <target>` - Get information about the target role like name, colour, members, permissions, etc
* `/info server` - Get information about the server like members, boosts, roles, emojis, etc
* `/info user <target>` - Get information about the target user like created at, pfp, banner, etc

![The info role command](https://i.imgur.com/NLeCrvc.png) ![The info user command](https://i.imgur.com/JI150MQ.png)
{% endtab %}
{% endtabs %}

## `membercount`

{% tabs %}
{% tab title="Slash" %}
* `/membercount` - Shows the member count of the server along with more statistics and a beautiful graph

![The membercount command](https://i.imgur.com/UXPFf7T.png)
{% endtab %}

{% tab title="Normal" %}
* **Aliases**: `mc`
* **Usage**: `membercount` - Shows the member count of the server along with more statistics and a beautiful graph
{% endtab %}
{% endtabs %}

## `purge-invites`

{% tabs %}
{% tab title="Slash" %}
* `/purge-invites <uses> <targetUsers> <usersType> <targetChannels> <channelsType>` - Mass delete invite links 
* `<uses>` invite links with uses less than or equal to this number will be deleted
* `<targetUsers>` is optional and defaults to all users
* `<usersType>` whether to inlucde or exclude the users mentioned in `<targetUsers>`. If empty, it defaults to include.
* `<targetChannels>` is optional and defaults to  all channels
* `<channelsType>` whether to inlucde or exclude the channels mentioned in `<targetChannels>`. If empty, it defaults to include.

![The purge-invite command](https://i.imgur.com/rWHYjOI.png)
{% endtab %}
{% endtabs %}

{% hint style="success" %}
Normal commands are supposed to be used with a prefix. The default prefix for normal commands is the bot's mention ( **`@Invite Management#6068`** ) and **`+`**
{% endhint %}
