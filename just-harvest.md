# Just Harvest

## Introduction
Built on the shoulders of wookies. 

## Macro
This macro will harvest the corpse you currently have selected, followed by any corpse around you. If you get the message `target is out of range for this action` there is likely another person killing mobs nearby. In this case just click the nearest corpse to you and it should continue harvesting.

### justHarvest
```
/harvest;
/harvest corpse;
/pause 1;
/macro justHarvest;
```

## Variants

You can replace `harvest` and `harvest corpse` with `harvest <resource type>` and `harvest corpse <resource type>` where `<resource type` can be `meat`, `bone` or `hide` if you want to gather a specific resource.

### justHarvestMeat
```
/harvest meat;
/harvest corpse meat;
/pause 1;
/macro justHarvestMeat;
```

### harvest

The old style macro, will only harvets what's clicked. Replace `<resource type` with `meat`, `bone` or `hide` as required. The following `/harvest` is a catchall in case the mob you are harvesting does not contain `<resource type>`.

```
/harvest <resource type>;
/harvest;
/pause 1;
/macro harvest;
```
