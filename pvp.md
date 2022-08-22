# PVP 

## Introduction
Built on the shoulders of wookies. 

All the macros that start with `clearCombatQueue` will dump all pending attacks in your combat queue, effectively interrupting whatever you were doing previously. This is mostly applied to heals and state debuffing, it's worth noting that by specifying `self` we don't need to change target, which would otherwise futz with our pvp. 

These macro's assume you have the standard Doctor `4x3x` as part of your template, otherwise some of these will not be available to you, and the bleed is from Fencer. 

## Doctor

### pvpCureDisease
```
/ui action clearCombatQueue;
/curedisease self;
```

### pvpCurePoison 
```
/ui action clearCombatQueue;
/curepoison self;
```

### pvpExtinguishFire
```
/ui action clearCombatQueue;
/extinguishFire self;
```

### pvpFirstAid
```
/ui action clearCombatQueue;
/firstAid self;
```

### pvpHealDamage
```
/ui action clearCombatQueue;
/healdamage self;
```

### pvpHealState
```
/ui action clearCombatQueue;
/healState self;
```

## Combat

### pvpDeathblow
```
/deathblow;
/pause 1;
/macro pvpDeathblow;
```

### pvpIntimidate
```
/ui action clearCombatQueue;
/intimidate;
```

### pvpWarcry
```
/ui action clearCombatQueue;
/warcry1;
/peace;
```

### pvpCOB
```
/center;
/pause 31;
/macro pvpCOB;
```

### pvpBleed
```
/melee1hhealthhit2;
/melee1hhealthhit1;
```

## Force Healing

### Heal Health Self

```
/ui action clearCombatQueue;
/healHealthSelf;
```

### Heal Action Self

```
/ui action clearCombatQueue;
/healActionSelf;
```

### Heal Mind Self

```
/ui action clearCombatQueue;
/healMindSelf;
```

### Heal All Self

```
/ui action clearCombatQueue;
/healAllSelf;
```

### Total Heal Self

```
/ui action clearCombatQueue;
/totalHealSelf;
```

### Stop Bleeding

```
/ui action clearCombatQueue;
/stopBleeding self;
```

### Force Cure Disease

```
/ui action clearCombatQueue;
/forceCureDisease self;
```

### Force Cure Poison

```
/ui action clearCombatQueue;
/forceCurePoison self;
```

### Heal States Self

```
/ui action clearCombatQueue;
/healStatesSelf;
```

### Purge

```
/ui action clearCombatQueue;
/healStatesSelf;
/forceCurePoison self;
/forceCureDisease self;
/stopBleeding self;
```
