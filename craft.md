# Crafting Macro

## Useage

This will fire a crafting tool in the first slot on the toolbar `toolbarSlot00`. It will then load the schematic found in slot 3 (this will vary based on your professions, what type of crafting tool you are using, and whether you have set the UI to auto-sort your schematics).
```
/ui action toolbarSlot00;
/selectDraftSchematic 3;
/pause 5;
/nextC;
/nextC;
/nextC;
/createPrototype practice no item;
/createPrototype practice no item;
/pause 2;
```
