# Tiny Stove 0.2.0

*by Dixiecapt*

A small cast iron ship's stove for small boats: the classic kind with a
flat top for one pot, a glass door with the fire burning behind it, a rail
round the top so the pot stays put at sea, and a capped stovepipe. A new
item for sale beside the Aestrin stoves at the Fort. It replaces nothing:
every stock stove is left as it is.

## Requirements

- Sailwind, BepInEx 5 (installed by Thunderstore Mod Manager / r2modman)

Optional: **Configuration Manager** (F1) to change settings in the game.

## Install

Unzip into `BepInEx\plugins\`. You should get:

    BepInEx\plugins\TinyStove\TinyStove.dll
    BepInEx\plugins\TinyStove\tinystove

Both files must sit together: `tinystove` is the stove's model. With a mod
manager, just install the package.

## The stove

- **Where to buy it:** the Fort (island 15), beside the two stock Aestrin
  stoves, at the Aestrin stove's price in the local coin.
- **How it works:** just like the Aestrin stove. It cooks at the same
  strength and holds three pieces of firewood. Set it on a deck and nail it
  down with the hammer like any stove.
- **One pot on top.** The soup pot or the kettle sits on the flat top,
  handles across, inside the rail.
- **Fire behind glass.** The firewood lies in the firebox and burns behind
  the door's window, with a warm glow on the deck in front of it and smoke
  from the chimney cap.
- **Size:** about 71 cm tall, 58 cm deep counting the door handle, and 44 cm
  wide. That is half the floor space of the Emerald stove, so it fits
  small boats.

## Settings

All of these are in F1, or in
`BepInEx\config\com.dixiecapt.sailwind.tinystove.cfg`.

- **Stove > Chimney length (m):** how tall the pipe stands above the stove,
  from 0.2 to 2.5 m. It changes every cast iron stove at once, so you can
  raise it to clear a cabin roof or lower it under a boom.
- **Shop > Sell at the Fort:** switches the Fort's stove spot on or off.
- **Shop > Spot along the stove row (m)** and **Spot sideways (m):** move
  where the stove stands for sale, if another mod has put something there.

## Taking it out

**A save with a cast iron stove in it needs this mod to load**, the same as
any mod that adds new items. Before you remove the mod, sell or throw away
every cast iron stove, then save.

If only the `tinystove` model file goes missing, your stoves come back as
plain Aestrin stoves so the save still loads. Put the file back and they
are cast iron again.

## Credits

- Stove model: a free cast iron stove model from TurboSquid, cut down for
  the game (window opened, top cleared, rail and chimney added).
- Cooking, fire, smoke and sound: the game's own Aestrin stove.

## Version history

- **0.2.0:** first shared release.
