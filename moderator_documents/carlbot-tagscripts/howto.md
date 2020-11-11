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
{=(validCommands):verify rules policies}

{=():Invalid shortcut "{1}"; must me one of: {validCommands}}

{=(L1):{lower:{1}}}
{=(policies):NCKkQKWP}
{=(rules):NCKkQKWP}
{=(verify):gvwGFW90}

{=(embedBin):{{L1}}}

{{and({in({L1}):{validCommands}}==true):c:cembed https://pastebin.com/{embedBin}}}

```
{% endraw %}

## Embed

### rules

{% raw %}
```
{"description":"• [Rapture Principles](https://kmorris896.github.io/rapture-discord-server-documentation/channel_text/landing-zone/welcome-message.html)\n• [Server Rules and Policies](https://kmorris896.github.io/rapture-discord-server-documentation/channel_text/landing-zone/rules-and-policies.html)\n• [Moderation Guide](https://kmorris896.github.io/rapture-discord-server-documentation/moderator_documents/why.html)\n\nRule changes/diffs can be found in [the server repository](https://github.com/kmorris896/rapture-discord-server-documentation/pulls?q=is%3Apr).","thumbnail":{"url":"https://github.com/kmorris896/rapture-discord-server-documentation/raw/228f19504580d0283b5415464bc184adb055acff/channel_text/landing-zone/images/github.png"},"color":8311585}
```
{% endraw %}

### Verify

{% raw %}
```
{"title":"💬 How To Verify","description":"[Verification Instructions](https://discord.com/channels/752074304224755752/752104497538400306/763876523517542461)","color":8311585}
```
{% endraw %}