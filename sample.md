This is the sampling macro I used (two variants, the first will ignore surveying mini game the second won't - the 2nd is more useful when crafting whilst surveying as it won't `/ui action defaultButton;` which can sometimes close your crafting window)

In order to use either of these macros you will need to manually survey for the material  you want to sample. Once you have located the resource and are happy with your position, run either depending on whether you are going to be afk, or crafting.

name: afkSample

```
/stand; 
/pause 1; 
/sample; 
/pause 5; 
/stand; 
/pause 1; 
/sit; 
/pause 25; 
/ui action defaultButton; 
/macro afkSample;
```

name: sample

```
/stand; 
/pause 1; 
/sample; 
/pause 5; 
/stand; 
/pause 1; 
/sit; 
/pause 25; 
/macro sample;
```

If your action secondaries are 400+ you won't need to sit, which can stop your character wondering the landscape:

```
/sample;
/pause 1;
/sample;
/pause 13.5;
/macro sampleTime;
```

Add the `/ui action defaultButton;` if you are afk and want to auto click away the minigame.

Mobyus version:

name: surveymacro

```
/stand;
/pause 2;
/sample;
/pause 6;
/stand;
/pause 2;
/sit;
/pause 17;
/macro surveymacro
```

