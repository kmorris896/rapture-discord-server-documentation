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


### Role Workflow:

- New Arrival
- Awaiting Initiation
- Initiate + Member

When brand new members enter the server, they are given the "New Arrival" role, which will grant them permission to the "Welcome" and "Rules and Policies" channel.  "New Arrivals" must react to the message in "Welcome", which will grant them the "Awaiting Initiation" role.

Members with the "Awaiting Initiation" role have one week to post an acceptable Introduction at which point they will be politely kicked from the server.


### Initiating New Members

New members need to complete an introduction as well as select roles for their profile.  Introductions should not be low-effort and should reflect that they have put thought and consideration to their words.  Of course, this is subjective but it's good to look for the following things:

- All of the required information is filled out
- Appropriate Server roles have been selected
- They aren't doing the bare minimum

If their introduction and profile are missing things, ping them in "Initiate Chat".  If they make the corrections as needed and are ready to be initiated, issue the following command:

```
!role custom USER_ID +@Initiate +@Member -@Awaiting Initiation
```

This will add the "Initiate" and "Member" roles to the user and remove the "Awaiting Initiation" role.


### Jail (or Mute)

Jailing or muting a member will remove all roles from their profile and add the "Jailed" role.  Jailed members can only see the Landing Zone and can only chat in the "Jail" chat channel.

The Jail chat channel is unique in that this is the only channel where moderators have "Manage Channel" permissions.  This is to allow mods to chat without being stopped by the Slowdown mode.

To jail a member, issue the following command:

```
!hardmute USER_ID <duration> <mute reason>
```

Duration should be set to an appropriate timeframe and should not exceed 10 days.  Most mutes should be for a day or two, using discretion as needed.

Some examples:

```
!hardmute 1234567890 1d You're being a bit of an ass right now.  Take a break for a day.  Come back fresh tomorrow
!hardmute 1234567890 48h We suspect you are underage.  In order to continue being a member on our server, you will need to verify.
!hardmute 1234567890 8h30m You probably shouldn't Discord while at work.
```

Mutes will show in #mod-actions **BUT** will not warn the user.  It's recommended that you issue both a warning and a mute at the same time.


### Bans

Moderators have the delegated authority to ban users.  While carlbot lacks the granularity to ensure that only tempbans are used, it's my personal belief that mods should have the power to ban indefinitely.

From a policy standpoint, indefinite bans should only be issued if there is a repeated offense by a member or if user is causing some sort of issue (i.e. raiding).  As a moderator, you are trusted to perform these actions judiciously and without malace.

Do not be afraid to use this power but know that you are wielding it.

To tempban a member, issue the following command:

```
!tempban USER_ID <duration> <reason>
```

Duration should be set to an appropriate timeframe.  

Some examples:

```
!tempban 1234567890 1d You're a bit thirsty.  Come back after you've rehydrated.
!tempban 1234567890 365d We suspect you are underage and did not verify.  We're banning you for one year.
!tempban 1234567890 7d You are a staff member of a server and cannot allow membership unless you either step down as staff on that server or you leave it.
```


### Mute vs. Ban

