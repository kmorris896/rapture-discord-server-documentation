---
sort: 4
---

# Verification

Verifying users is relatively straight forward.  All verification attempts require a government-issued ID that shows the following information:

- Picture
- Date of Birth
- Gender

The example that is posted on the server:

![Image of a Censored License](https://github.com/kmorris896/rapture-discord-server-documentation/raw/main/channel_text/images-and-assets/MaskedPassport.jpg)

Obviously, check to make sure that the person is 18 years old.  FYI: **Their birthday must be before or today 2003.**

The license is used to verify the person is over 18 and that their license picture reasonably matches their picture/video.

While I have a hard time believing this will happen, if you are concerned that an ID may be fake, please let the admin handle the verification.

Now let's go through each method.


## Picture Verification

The verification procedures instruct:

> Selfie with a **hand-written sign** that has the server name, your Discord Username and Discriminator (the four digit code that comes after the `#`), and the date and time.

Have the member post this picture first.  Make sure the picture looks clear and unfiltered.  Keep in mind that you are not verifying their age.  You are verifying that the person on the other end is who they say they are.  Note their gender, making appropriate allowances for trans and non-binary people.

The concern that we want to address is that someone who is trying to gain access to gender-specific channels.

If you are not satisfied, have the user take the picture again with a new sign.  Don't do this more than once.  If you are still not satisfied, pass it on to an admin.

The second selfie the user is to take must happen while in chat.  Have the user take another selfie with something else written on top of the sign.  Examples include a random word or number.  If they can't do this, have them take a selfie holding up a hand signal such as thumbs up, hang-loose, "Dr. Evil Pinky Thing", etc.  **Do not have hold up a number with their fingers.**  It's too easy for them to get all combinations from someone else.

Do not give the user more than a few minutes to take the picture.  If this picture takes longer than 5 minutes, they have failed verification and can try again the next day.

If they fail verification twice, members must verify using Video Chat immediately or face a 30-day ban.


## Adult Website Verification

```note
This is still experimental.  The process for this may change.
```

If the member is a **verified** member of one of the following sites, they may verify without posting a picture:

- pornhub.com
- onlyfans.com
- hutt.com

In order for the member to verify, they must post on their site a publicly accessible picture that shows their face.  If they do not show their face on their site, they cannot verify in this way.

Make sure that the member's license picture reasonably matches the picture they posted.


## Shared Discord Server Verification

```note
This is still experimental.  The process for this may change.
```

If the member is verified on another Discord Server that you share with them and they have a similar system of verification, you may verify them without further review.

# Final Steps

It is the **member's** responsibility to delete their pictures.  You may remind them of this prior to closing the ticket.  Close the ticket by issuing the following command:

`t!close Verified [user]`

# Forcing Verification

Any member, regardless of their verification status, may be forced to verify if a moderator believes that a member is misrepresenting their identity.  In order to do so, create a ticket like you normally would and then issue the following command within the channel:

`t!add USER_ID`

Once they are added, make sure you ping them so that you can see that a ticket was created for them.

**Do not DM users for verification.**  This is open to abuse by non-mods as they can change their Discord username to match a mods.

If you are forcing verification, you probably need to mute them as well.  To do so, issue the following command:

`!hardmute USER_ID There is a concern that you may be underage, catfishing, etc`

Doing so will open the jail channel for the user as well as the ticket you opened.  If the user fails to verify, ban the user for one year.

`!ban USER_ID 365d You failed to verify so we're banning you for one year.  Sorry.`

