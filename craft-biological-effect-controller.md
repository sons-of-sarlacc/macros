# Introduction

Place 5 food and chemical crafting tools in the first 5 slots of your current toolbar. the macro will craft biological effect controllers with a 5 second pause to input materials.

```
/ui action toolbarSlot00;
/selectDraftSchematic 00;
/pause 5;
/nextcraftingstage;
/nextcraftingstage;
/createprototype practice no item;
/createprototype practice no item;
/pause 2.1;
/ui action toolbarSlot01;
/selectDraftSchematic 00;
/pause 5;
/nextcraftingstage;
/nextcraftingstage;
/createprototype practice no item;
/createprototype practice no item;
/pause 2.1;
/ui action toolbarSlot02;
/selectDraftSchematic 00;
/pause 5;
/nextcraftingstage;
/nextcraftingstage;
/createprototype practice no item;
/createprototype practice no item;
/pause 2.1;
/ui action toolbarSlot03;
/selectDraftSchematic 00;
/pause 5;
/nextcraftingstage;
/nextcraftingstage;
/createprototype practice no item;
/createprototype practice no item;
/pause 2.1;
/ui action toolbarSlot04;
/selectDraftSchematic 00;
/pause 5;
/nextcraftingstage;
/nextcraftingstage;
/createprototype practice no item;
/createprototype practice no item;
/pause 2.1;
/macro craftBEC;
```
