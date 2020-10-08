---
sort: 3
cSpell: ignore waifu
---

# Economy

<@763577946211745814> (Name may change) is a self-hosted version of the NadekoBot (<https://gitlab.com/Kwoth/nadekobot>).  Full commands can be found on their website (<https://nadeko.bot/commands>) but keep in mind that the server only has the following modules enabled:

- **gambling**
-- "WaifuClaimCommands" disabled
-- "FlowerShopCommands" disabled
-- all other gambling games can be played in <#758133041213210635>
- **games**
-- only the `.pick` and `.plant` commands are available in the chat channels
-- all other games can be played in <#758133041213210635>

Please note that this is very experimental.  I'll try to keep settings relatively stable but data loss (and thus accumulated peels) is possible.  Don't go *too* wild claiming peels.

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
