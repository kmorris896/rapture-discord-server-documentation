---
TagScript: true
---

# Tag: bdsmtopic
- Command: `!howto`
- Requirements:
  - Can only be run as Moderator


## Description

BDSM Topics Script

## Script

{% raw %}
```
{=(topic):{random:
    What is one thing that's a no-no for you?~
    What is your favorite pet name?~
    What's a recent experience that felt like an affirmation of your kink role or identity?~
    What's the difference between BDSM and abuse and how can you tell the difference?~
    Is BDSM and kink appropriate when struggling with mental health?  Does it help, hinder, or neither?~
    What one part of BDSM/kink would you wish to be more socially acceptable right now, today?~
    Have you had a mentor, or someone important you learned from, in your journey into BDSM?  What's the most important thing you learned from them?~
    }
}

{embed(color): #51d3c0}
{embed(title): 💬 Random BDSM Topic #{uses}}
{embed(description):
{topic}
}

{=(comment): Make sure that the embed builder has something in it.
I recommend a period in the description.}
```
{% endraw %}