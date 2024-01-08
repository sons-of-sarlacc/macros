# Introduction

Place 5 general crafting tools in the first 5 slots of your current toolbar. the macro will craft mineral survey devices with a 5 second pause to input materials.

The schematic number is correct if artisan is the only prof you have that grants crafting recipies, otherwise you will need to adjust for your character. 

### craftMSD
```
/ui action toolbarSlot00;
/selectDraftSchematic 22;
/pause 5;
/nextcraftingstage;
/nextcraftingstage;
/createprototype practice no item;
/createprototype practice no item;
/pause 2.1;
/ui action toolbarSlot01;
/selectDraftSchematic 22;
/pause 5;
/nextcraftingstage;
/nextcraftingstage;
/createprototype practice no item;
/createprototype practice no item;
/pause 2.1;
/ui action toolbarSlot02;
/selectDraftSchematic 22;
/pause 5;
/nextcraftingstage;
/nextcraftingstage;
/createprototype practice no item;
/createprototype practice no item;
/pause 2.1;
/ui action toolbarSlot03;
/selectDraftSchematic 22;
/pause 5;
/nextcraftingstage;
/nextcraftingstage;
/createprototype practice no item;
/createprototype practice no item;
/pause 2.1;
/ui action toolbarSlot04;
/selectDraftSchematic 22;
/pause 5;
/nextcraftingstage;
/nextcraftingstage;
/createprototype practice no item;
/createprototype practice no item;
/pause 2.1;
/macro craftMSD;
```
