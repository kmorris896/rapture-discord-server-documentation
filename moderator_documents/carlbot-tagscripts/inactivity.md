---
TagScript: true
---

# Tag: inactivity
- Command: `!inactivity`
- Arguments: 
  - **REQUIRED** reason shortcut; one of:
    - "rule": For not accepting the rules
    - "intro": For not posting an acceptable intro
    - "inactive": For not being active
  - **REQUIRED** User ID
- Requirements:
  - Can only be run as Moderator


## Description

Kicks the named user off the server with the reason stated.

## Script

{% raw %}
```
{=(validReasons):rule rules intro inactive}
{=():Invalid Reason "{1}"; must me one of: {validReasons}}

{=(l1):{lower:{1}}}
{=(rule):Thank you very much for checking us out.  I know life can get busy but since you haven't accepted the rules within 48 hours, I'm giving you a polite nudge out of the server.}
{=(rules):{rule}}
{=(intro):Thank you very much for checking us out.  I know life can get busy but since you haven't posted an acceptable intro within 48 hours, I'm giving you a polite nudge out of the server.}
{=(inactive):Thank you very much for checking us out.  I know life can get busy and it can be hard finding a way in a server.  I promise we are a warm and inviting bunch.  However, we want you to participate in our conversations.  Since you haven't done so in over a week, I'm giving you a polite nudge out of the server.  But don't worry: you're welcome back at anytime.  You're roles and intro will stay up.}

{=(reason):{{l1}}

You are welcome anytime by accepting this invite: https://discord.gg/hRSHvBd}

{{if({in({1}):{validReasons}}==true):c:kick {2} {reason}}}

```
{% endraw %}
