---
TagScript: true
---

# Tag: howto
- Command: `!howto`
- Requirements:
  - Can only be run as Moderator


## Description

Provides instructions on how to verify.

## Script

{% raw %}
```
{=(validCommands):verify rules policies inactive invite}

{=():Invalid shortcut "{1}"; must me one of: {validCommands}}

{=(L1):{lower:{1}}}
{=(policies):NCKkQKWP}
{=(rules):NCKkQKWP}
{=(verify):gvwGFW90}
{=(inactive):5fQrhBgT}
{=(invite):85nB1sMz}

{=(embedBin):{{L1}}}

{{and({in({L1}):{validCommands}}==true):c:cembed https://pastebin.com/{embedBin}}}

```
{% endraw %}

## Embed

### rules

{% raw %}
```
{"description":"• [Rapture Principles](https://kmorris896.github.io/rapture-discord-server-documentation/channel_text/landing-zone/welcome-message.html)\n• [Server Rules and Policies](https://kmorris896.github.io/rapture-discord-server-documentation/channel_text/landing-zone/rules-and-policies.html)\n• [Moderation Guide](https://kmorris896.github.io/rapture-discord-server-documentation/moderator_documents/why.html)\n\nRule changes/diffs can be found in [the server repository](https://github.com/kmorris896/rapture-discord-server-documentation/pulls?q=is%3Apr).","thumbnail":{"url":"https://github.com/kmorris896/rapture-discord-server-documentation/raw/228f19504580d0283b5415464bc184adb055acff/channel_text/images-and-assets/github.png"},"color":8311585}
```
{% endraw %}


### verify

{% raw %}
```
{"title":"💬 How To Verify","description":"Verification is a great way to let members know that you are, indeed, a legal adult as well as the selected gender.  It also grants you access to the verified channels where members post their own pictures.\n\n- [Verification Guidelines](https://kmorris896.github.io/rapture-discord-server-documentation/moderator_documents/verification.html)\n\nTL;DR: Create a <#752172092426027108> and be prepared to upload a picture of your license (with personal information optionally covered).  Then choose to verify either with a selfie or other adult verification.","color":8311585}
```
{% endraw %}


### inactive
{% raw %}
```
{"title":"⏰Inactivity Policy","description":"This server prides itself in having **active** membership.  We'd rather our membership numbers reflect the total number of people who participate than have a high count.\n\nDetails regarding our [Inactivity policy are available in our Rules and Policies](https://kmorris896.github.io/rapture-discord-server-documentation/channel_text/landing-zone/rules-and-policies.html).  If you want to tell us you won't be available, post in <#761402092107595797>","color":8311585}
```
{% endraw %}


### invite
{% raw %}
```
{"title":"📨 Server Invite","description":"Want to invite someone?  Here is the Invite link:\n\n`https://discord.com/invite/hRSHvBd`","color":8311585}
```
{% endraw %}
