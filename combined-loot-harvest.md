# Combined Loot & Harvest

## Introduction
Built on the shoulders of wookies. 

## Macro
This macro will loot and harvest all corpses around you. It does not work well in groups, if you have harvested a corpse and a party member who has novice scout does not harvest it the macro goes awry. This is the main reason I split the loot and harvest macros. 

### combinedLootHarvest

```
/loot; 
/loot corpse all;
/pause .5;
/harvest;
/harvest corpse;
/pause .5;
/macro hoover;
```
