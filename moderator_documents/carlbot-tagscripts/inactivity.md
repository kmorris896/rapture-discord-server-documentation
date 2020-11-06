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
{=():}
{if({1} == "rule"):{=(reason):Thank you very much for checking us out.  I know life can get busy but since you haven't accepted the rules within 48 hours, I'm giving you a polite nudge out of the server.}}
{if({1} == "intro"):{=(reason):Thank you very much for checking us out.  I know life can get busy but since you haven't posted an acceptable intro within 48 hours, I'm giving you a polite nudge out of the server.}}
{if({1} == "inactive"):{=(reason):Thank you very much for checking us out.  I know life can get busy and it can be hard finding a way in a server.  I promise we are a warm and inviting bunch.  However, we want you to participate in our conversations.  Since you haven't done so in over a week, I'm giving you a polite nudge out of the server.  But don't worry: you're welcome back at anytime.  You're roles and intro will stay up.}}

{=(reason):{reason}

You are welcome anytime by accepting this invite: https://discord.gg/hRSHvBd}

{{c:kick {2} {reason}}}
```
{% endraw %}
