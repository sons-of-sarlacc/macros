# configuration options

## enable user.cfg
Find the `swgemu.cfg` file in the SWGEmu client installation folder and find the following line and uncomment it (remove the leading #), the line once modified should look like this:

```
.include "user.cfg"
```

## increase maxiumum zoom

Find the `user.cfg` file in the SWGEmu client installation folder (or create it if it doesn't exist) and add the following lines:

```
[ClientGame]
freeChaseCameraMaximumZoom=6
```
