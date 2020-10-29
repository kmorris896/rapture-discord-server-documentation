---
TagScript: true
---

# Tag: initiate
- Command: `!initiate`
- Arguments: 
  - **REQUIRED** User mention
- Requirements:
  - Can only be run as Moderator


## Description

Removes the "Awaiting Initiation" role and adds the "Member" and "Initiate" Roles.

## Script

```
{require(message):<@&752090357025734756>}

{=(error):You must ping a valid Discord user}
{{if({user(id)}!={target(id)}):c:role custom {target(id)} +752090540371345488 +752090174737088583 -752090021967953991}}
```
