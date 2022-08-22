# AFK Combat

## Introduction
Built on the shoulders of wookies. 

## Macros

This macro will find a target every 15 seconds and throw an intimidate at it. It is not intended for at keyboard combat automation. It's intended use is afk farming static spawns outside of majour NPC cities. No buffs required, but reasonable armour minisuit probably mandatory. 

### afkstatic
```
/tar self;
/pause 1;
/ui action cycleTargetOutward;
/pause 1;
/intimidate;
/pause 1;
/attack;
/pause 12;
/macro afkstatic;
```

### afk

This macro will find the closest target every 2 seconds. 

Because the macro always targets you first at the start of the loop, the cycleTargetOutward will always land on the nearest enemy. 

```
/stand;
/ui action targetSelf;
/ui action cycleTargetOutward;
/attack;
/pause 2;
/macro afk;
```
