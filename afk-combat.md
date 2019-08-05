# AFK Combat

## Introduction
Built on the shoulders of wookies. 

## Macro
This macro will find a target every 15 seconds and throw an intimidate at it. It is not intended for at keyboard combat automation. It's intended use is afk farming static spawns outside of majour NPC cities. No buffs required, but reasonable armour minisuit probably mandatory. 

### afk
```
/tar self;
/pause 1;
/ui action cycleTargetOutward;
/pause 1;
/intimidate;
/pause 1;
/attack;
/pause 12;
/macro afk;
```
