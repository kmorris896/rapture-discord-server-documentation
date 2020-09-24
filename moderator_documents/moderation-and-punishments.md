---
sort: 2
---

# Moderation and Punishments

Moderating the server is relatively straight-forward.  I won't go through the entire [carl-bot documentation](https://docs.carl.gg/moderation/moderation/) here but I will go over some of the specific commands we'll be using.

## Message/Chat Management

Chat management is fairly straight forward.  You can mass-delete messages (with or without options).  This might be necessary to clean up any drama or inappropriate messages.

### Purge or delete messages

```
!purge x
```

Where `x` is the number of messages to purge.  Keep in mind that purges do not show up in the delete logs.

### Purge or delete messages from a specific person

```
!purge user @someuser 100
```

Where `@someuser` is mentioning the username in question and `100` is the number of messages to delete.


## User Management

### Jail (or Mute)

Jailing or muting a member will remove all roles from their profile and add the "Jailed" role.  Jailed members can:

- See the Welcome, Rules and Policies, and Support Ticket channels
- All other chat channels are hidden except for the "Jail" chat channel

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

On the surface, mute and bans accomplish the same action: preventing the offending member from interacting with the rest of the server.  So why do one over the other?

A mute may be more appropriate for someone who is new to the server or someone who has been on the server a long time and needs "a time out".  If they are being a bit of an ass, isolating them so that they have to interact with the mod so they understand what they did wrong, with the ultimate goal being mutual understanding.  If the member understands, feel free to lift the mute early.

Bans, on the other hand, should be employed for cases involving egregious rule breaks, such as spamming, repeated harassment, etc.  Temp bans should lead to a full ban if the admin agrees.

A short cut to deciding between the two: if you want to talk to the offending user, mute.  If you just want them out of here, ban.

Both are reversable so don't feel bad if you choose incorrectly.  At the end of the day, remember it's about protecting members and both actions do just that.

