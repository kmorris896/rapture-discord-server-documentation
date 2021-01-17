---
TagScript: true
---

# Tag: howtoverify
- Command: `!howtoverify`
- Requirements:
  - Can only be run as Moderator


## Description

Provides instructions on how to verify.

## Script

{% raw %}
```
{require():<@&752090357025734756>}

{=(TZHours):-5}
{=(TZSeconds):{m:{TZHours}*60*60}}
{=(ETUnix):{m:trunc({unix}+{TZSeconds})}}


```
{% endraw %}

## Embed

{% raw %}
```
{"fields":[{"name":"Instructions for Moderators","value":"**__ID Verification__**\n\nMembers must be **18 years old or older** as of **US EASTERN TIME**, not member local time.  This is due to the fact that the server is located in US East.  \n\nDate of Birth in most other countries outside of the United States follow `yyyy-mm-dd` or `dd-mm-yyyy`.  If you're not sure, ask the member.\n\n\n","inline":false},{"name":"Birthday Cutoffs","value":"**Current Date (yyyy-mm-dd):** {strf({ETUnix}):%F}\n\n**18 years ago:** {m:trunc({strf({ETUnix}):%Y}-18)}-{strf({ETUnix}):%m-%d}\n**24 years ago:** {m:trunc({strf({ETUnix}):%Y}-24)}-{strf({ETUnix}):%m-%d}\n**30 years ago:** {m:trunc({strf({ETUnix}):%Y}-30)}-{strf({ETUnix}):%m-%d}\n**40 years ago:** {m:trunc({strf({ETUnix}):%Y}-40)}-{strf({ETUnix}):%m-%d}","inline":false}],"title":"How To Verify","description":"The full instructions are available in [rules-and-policies](https://discord.com/channels/752074304224755752/752104497538400306/763876523517542461) but here is the summary:\n\nTo start the verification process, you'll first submit picture of a government-issued photo identification.  In most places, this is a drivers license or identification card.  It can also be a passport or any other identification so long as it has your picture, your date of birth, and your gender.\n\nFor your privacy, you may black out any other personal information, such as your name, address, ID number, etc.  [Please see this image for an example](https://github.com/kmorris896/rapture-discord-server-documentation/raw/main/channel_text/landing-zone/images/MaskedPassport.jpg).\n\nYour identification is used to verify you are over 18.  Once this is done, tell the moderator how you would like to identify.  You can choose to verify in one of the following ways:\n- Video chat\n- Selfie\n- Verified third-party web-site (Pornhub, OnlyFans, etc) or partner server","color":8311585}
```
{% endraw %}