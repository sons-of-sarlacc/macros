# AFK Combat

## Introduction
Built on the shoulders of wookies. 

## Macro
This macro will find a target every 15 seconds and throw an intimidate at it. You can use this to grind marksman, but you need to spend the 100 credits on novice brawler for Intimidate1. If for whatever reason you do not want to take novice brawler you can remove the intimidate and the following pause.

It is not intended for at keyboard combat automation. It's intended use is afk farming static spawns outside of majour NPC cities. No buffs required, but reasonable armour minisuit probably mandatory. 

Because the macro always targets you first at the start of the loop, the cycleTargetOutward will always land on the nearest enemy. 

### afk
```
/stand;
/ui action targetSelf;
/ui action cycleTargetOutward;
/attack;
/pause 2;
/macro afk;
```
