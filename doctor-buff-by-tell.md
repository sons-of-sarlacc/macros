# Doctor: Buff by tell

## Introduction
Built on the shoulders of wookies. This macro will doctor buff on tell. Needs improvement for pulling droid, eating bivoli and havla. 

## Alias
You only need to run the alias once per session. Change all instances of `<name>` to your character's name.

```
/alias :a /alias <name> /ui action toolbarPane04;/pause 4;/ui action toolbarPane05

/alias :b /alias <name> /setmood

/alias ll /target
```

## Macro
Create the following macros exactly as written. Change all instances of `<name>` to your character's name.

### docStart
Starts macros running.
``` 
/:a;
/pause 1;
/macro docAdvertise;
/pause 1;
/tell <name> Clearing target.;
/pause 1;
/tar Bacta;
/macro docResponse;
```

### docAdvertise
Respect the server spam rules and don't advertise more often than every 3 minutes. 

 ```
/Recite Now buffing. Please see my bio for buffing instructions.;
/pause 180;
/macro docAdvertise;
```

### docResponse
Checks to see if someone sent a tell.

```
/ui action startChatReply;
/ui action chatCursorHome;
/ui action chatCursorRight;
/ui action chatDelete;
/ui action chatDelete;
/ui action chatDelete;
/ui action chatDelete;
/ui action chatDelete;
/ui action chatEnter;
/pause .5;
/ui action toolbarSlot11;
/pause 1;
/tell <name> Clearing target.;
/pause 10;
/macro docResponse;
```

### docBuff
Runs buff cycle.
* If you put a Medical Droid on `toolbarPane05` > `toolbarSlot09` it will be called and dismissed when there is a valid buff customer
* Put Bivoli and Havla on `toolbarPane05` > `toolbarSlot08` & `toolbarSlot07` they will be used when there is a valid buff customer. 

```
/:b;
/afk;
/pause .5;
/ui action startChatReply;
/ui action chatCursorHome;
/ui action chatCursorRight;
/ui action chatDelete;
/ui action chatDelete;
/ui action chatEnter;
/pause 1;
/say Beginning buffs now.;
/ui action toolbarSlot10;
/pause .5;
/ui action toolbarSlot09;
/pause .5;
/ui action toolbarSlot08;
/pause .5;
/ui action toolbarPane04;
/pause 1;
/healEnhance Health;
/pause 13;
/healEnhance Action;
/pause 13;
/healEnhance Strength;
/pause 13;
/healEnhance Stamina;
/pause 13;
/healEnhance Constitution;
/pause 13;
/healEnhance Quickness;
/pause 1;
/tellpet store;
/pause 1;
/say Your buffs are complete. Enjoy your day, and good luck out there.;  
/tar Bacta;  
/pause 1;  
/afk;  
/:a;
```

## UI settings

### Toolbar

* Set sixth pane, toolbarSlot11 to the docBUFF macro.
* Set fifth pane, toolbarSlot11 to Empty.
* Set sixth pane, toolbarSlot10 to your Medical Droid.
* Set sixth pane, toolbarSlot09 to your Bivoli. 
* Set sixth pane, toolbarSlot08 to your Havla.


### Bio
In `Community > Character > Biography` set an appropriate message.

```
Send me a tell for buffs. No need to drop group!

If I fail to buff you, please soft-log and try again.

Doc buffs require a significant up-front investment. If you appreciate the service, please tip.
```

### AFK
Ensure `Options > AFK > Auto AFK enabled` is not checked.

In `Options > AFK > Auto-Response Message` set an appropriate response.

```
I am currently in the middle of a buff session. Please send a tell when this session is over.  
  
Thank you for your support!
```

### Cantina & compulsory item placement (Bacta)
I have crafted a Healthpack and named it "Bacta" as my no-buff target. 

### Droid
You want a droid deployed with battery power and a Medical Module Rating: 110. 

Drag your droid to `toolbarPane05` > `toolbarSlot09`

## Food
Food is critical to a doctor maximizing the application of their buffs. 

### Bivoli
Bivoli increses your Wound Treatment Skill Mod. Drag your Bivoli to `toolbarPane05` > `toolbarSlot08`. You do not need to adjust your macro to benefit from Bivoli as it increases the potency of the buffs.

### Havla
Havla increases your Wound Treatment Speed Skill Mod. The above macro does not yet have optimised timings for Havla consumption. Drag your Havla to `toolbarPane05` > `toolbarSlot07` and you will need to adjust the timings in docBuff between all the `healEnhance` calls. 

### References

* [Mistress Aerea Buff by tell macro](https://www.swgemu.com/forums/showthread.php?t=128123)
* [nunzio99 Who are your tippers](https://www.swgemu.com/forums/showthread.php?t=205263)
* [Astin Larry's Doctor Macro](https://www.swgemu.com/forums/showthread.php?t=214152)
* [Xtura Seska's Doctor Guide: Buffing for Free (for tips)](https://www.swgemu.com/forums/showthread.php?t=47785)
* [NaTaS Buff by Tell Macro](https://revelationonline.net/forums/viewtopic.php?t=126)
