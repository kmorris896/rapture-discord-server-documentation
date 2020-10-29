---
sort: 2
---

# Roles and Permissions

Server Roles are broken up into the following categories:

* **Vanity Roles**: These roles don't provide any special rights/privileges except to make certain information easy to see when clicking on a user's profile.
* **Prescriptive Roles**:  These roles will provide special rights/privileges server-wide, category-wide, or channel specific.

The following Prescriptive Roles provide the basis of all privileges granted to members:

|Role Name|Role ID|Category|Unique|Server Permissions|Category Permissions|Channel Permissions|
|---|---|---|---|---|---|---|
|New Arrival|752089891621568563|Membership|One of Membership|Read Message History|none|Can only see "Welcome" and "Rules and Policies" channel|
|Awaiting Initiation|752090021967953991|Membership|One of Membership|Attach Files, Read Message History, Use External Emojis, Add Reactions, Connect, Speak, Video|Can see all "Landing Zone" channels|Read announcements, and create tickets.|
|Member|752090540371345488|Membership|One of Membership|Attach Files, Read Message History, Use External Emojis, Add Reactions, Connect, Speak, Video|Most categories opened|Can see majority of the server, sans administrative channels|
|Jailed|752151508237418506|Membership|One of Membership|Attach Files, Read Message History, Use External Emojis, Add Reactions, Connect, Speak, Video|none|Can only chat the "Jail" chat, read rules/policies, and create service tickets.|


# Role Workflow:

- New Arrival
- Awaiting Initiation
- Initiate + Member
- Member

When brand new members enter the server, they are given the "New Arrival" role, which will grant them permission to the "Welcome" and "Rules and Policies" channel.  "New Arrivals" must react to the message in "Welcome", which will grant them the "Awaiting Initiation" role.

Members with the "Awaiting Initiation" role have one week to post an acceptable Introduction at which point they will be politely kicked from the server.


# Initiating New Members

New members need to complete an introduction as well as select roles for their profile.  Introductions should not be low-effort and should reflect that they have put thought and consideration to their words.  Of course, this is subjective but it's good to look for the following things:

- All of the required information is filled out
- Appropriate Server roles have been selected
- They aren't doing the bare minimum

If their introduction and profile are missing things, ping them in "Initiate Chat".  If they make the corrections as needed and are ready to be initiated, issue the following command:

```
!initiate @username
```

This will add the "Initiate" and "Member" roles to the user and remove the "Awaiting Initiation" role.

Please note that the "Initiate" role is a **VANITY** role and does not grant any additional rights or permissions.
