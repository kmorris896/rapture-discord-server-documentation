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
{=(validCommands):verify}

{=():Invalid shortcut "{1}"; must me one of: {validCommands}}

{=(L1):{lower:{1}}}
{=(verify):gvwGFW90}

{=(embedBin):{{L1}}}

{{and({in({L1}):{validCommands}}==true):c:cembed https://pastebin.com/{embedBin}}}


```
{% endraw %}

## Embed

### Verify

{% raw %}
```
{"title":"💬 How To Verify","description":"[Verification Instructions](https://discord.com/channels/752074304224755752/752104497538400306/763876523517542461)","color":8311585}
```
{% endraw %}