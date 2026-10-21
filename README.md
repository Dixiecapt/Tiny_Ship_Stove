# Tiny Stove 0.2.4

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
- **A closed stove makes its wood go further.** The three logs burn one
  after another, each slowly, so a full load lasts 8 game-hours (the
  night through) at a steady heat. The game's open stoves burn every log
  at once, 2 hours each.
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
- **Stove > Hours a full load burns** (8) and **Logs burning at once** (1).
- **Shop > Sell at the Fort:** switches the Fort's stove spot on or off.
- **Shop > Spot along the stove row (m)** and **Spot sideways (m):** move
  where the stove stands for sale. The mod walks along the row by itself
  until the stove's spot is inside the shop and on open ground.
- **Shop > Mark the spot where I stand:** stand in the Fort's shop where
  the stove should stand, facing the way its door should face, and switch
  this on. The stove moves there at once and stays there.

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

- **Log > Report each stove shape:** for bug reports. The first three
  stoves to appear write one line each to the log saying where their
  picture, pointing box and physics body are. Switch off once all is well.

## Version history

- **0.2.4:** fixes 0.2.3, which failed to build the stove on every machine
  and put a plain Aestrin stove in its place (Exocet): the new strip of
  inherited shapes was taking the stove's own cook place and fire with them.
  Do not run 0.2.3.
- **0.2.3:** works with Better Tables 0.1.0. That version hangs four leg
  shapes under the stock Aestrin stove; the tiny stove is a copy of that
  stove and was carrying the legs too, 26 cm through the deck, so it was
  red in the hand, would not set down and thrashed when it did (Mad). The
  stove now drops every collider it inherits from the stock stove except
  its own cook place and fire.
- **0.2.2:** the shop spot: 0.2.1 could walk the wrong way along the stove
  row and put the stove in a stall (Mad); the row's end is fixed again, the
  spot must be on open ground, and a Mark-the-spot switch in F1 puts it
  where you stand. The wood burns one log at a time and a load lasts 8
  hours. The log also reports a stove's shapes after it is put down.
- **0.2.1:** the stove's physics and pointing shape is now one plain box
  instead of a hull built on each PC (reports of the pointer landing beside
  the stove, a red outline in the hand, and the stove or ship thrashing);
  a switchable log line to help chase anything left.
- **0.2.0:** first shared release.
