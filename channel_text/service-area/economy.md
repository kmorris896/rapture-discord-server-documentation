---
sort: 3
cSpell: ignore waifu
---

# Economy

<@763577946211745814> is a self-hosted version of the NadekoBot (<https://gitlab.com/Kwoth/nadekobot>).  Full commands can be found on their website (<https://nadeko.bot/commands>) but keep in mind that the server only has the following modules enabled:

- **gambling**
-- "WaifuClaimCommands" disabled
-- "FlowerShopCommands" disabled
-- all other gambling games can be played in <#758133041213210635>
- **games**
-- only the `.pick` and `.plant` commands are available in the chat channels
-- all other games can be played in <#758133041213210635>

The currency of the server is called "Banana Peels".  Peels are earned in one of three ways:
- :banana: 5 by typing `.timely` in <#758133041213210635> every 2 hours
- various amounts for participating in server events such as picture themes, etc.
- :banana: 2 randomly (2% chance) while chatting in the following enabled channels:

-- message break --

```
# provide a list of all channels where .gc is enabled
.gclist
```

-- message break -- 

All members, including mods and admins, may purchase items listed in the Store below.  And although admins are in the unique position to give away currency, they won't because it will **RUIN THE ECONOMY**.  :rofl:

All items are sold by "the server" and banana peels return to the pool for further distribution.  At this time, you may not buy things from other users.  If there is interest in this, I'll consider it.  

Please note that this is very experimental.  I'll try to keep settings relatively stable but data loss (and thus accumulated peels) is possible.  Don't go *too* wild claiming peels.

-- message break --

+++

**__The Store__**

To purchase an item, you may tell me within the server, DM me, or create a <#752172092426027108>.


**__Picture Themes__**
Only one theme can be active at one time

- :banana: 100 - 1-Day SFW Picture Theme
- :banana: 200 - 1-Day NSFW Picture Theme
- :banana: 300 - 1-Day SFW/NSFW Picture Theme (yes, just add the two together)

**__Server__**
- :banana: 1000 - Change <@725742965661761588>'s server nickname once, lasts one day
- :banana: 1500 - Custom server role with a custom color and role break-out that lasts 1 week

**__Requires Consent__**
You must receive the member's permission before purchasing any of these roles.

- :banana: 500 - Change a member's nickname once, lasts for one day.
- :banana: 1500 - Custom server role with a custom color and role break-out that lasts 1 week

*More items may be added over time.  Feel free to make your suggestions over in <#754995041117798480>.*

+++

```
# cspell:disable

# disable all modules
.asm disable

# enable economy by enabling gambling and games in Bots Commands channel
.cm gambling enable <#758133041213210635>
.cm games enable <#758133041213210635>

# enable .pick server-wide
.sc .pick enable
.sc .plant enable

# disable waifus
.sc .claim disable
.sc .gift disable
.sc .waifureset disable
.sc .waifutransfer disable
.sc .divorce disable
.sc .affinity disable
.sc .waifustats disable
.sc .shop disable

# disable .give command so that users can't give each other currency
.sc .give disable

# Set Currency
.bce CurrencyName Banana Peel
.bce CurrencyPluralName Banana Peels
.bce CurrencySign :banana:

# Set Timely
# 5 peels every 2 hours, total of 60 daily
.timelyset 5 2

# Currency Generation: drop 2 peels
.bce CurrencyDropAmount 2

# Daily Currency Decay to control inflation, currently disabled
# .bce DailyCurrencyDecay 0.05
```
