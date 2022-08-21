# AFK Combat

## Introduction
Built on the shoulders of wookies. 

## Macro
This macro will find the closest target every 2 seconds. 

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
