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

## mouse unlocked from game window

In `options.cfg`:

```
[ClientGraphics]
  constrainMouseCursorToWindow=0
```

## in game features

You can spin the camera around your character by pressing `ctrl` + `shift` + `s`, this option does not show up in the in-game keybindings.

## crossover

To stop the gamma being set by the game when using [crossover](https://www.codeweavers.com/crossover/) on MacOS use the following command in the terminal:

```
defaults write com.codeweavers.CrossOver AllowGamma never
```

Use `always` in place of `never` if you prefer the game to change the brightness.

## references

* [SWGEmuEdu - Ep.99 - Changing the Maximum Zoom Range (Mobyus1)](https://www.youtube.com/watch?v=-gZpskSlXhs)
* [Adjust brightness/contrast in game under Mac CX 11 and 12](https://www.codeweavers.com/compatibility/crossover/tips/deus-ex/adjust-brightness-contrast-in-game-under-mac-cx-11-and-12)
