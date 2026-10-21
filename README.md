# Galley Range 0.1.0

*by Dixiecapt*

A man-of-war's galley stove for the largest ships: the Brodie stove of the
1780s. A riveted iron range with two copper boilers set into the top at the
back, two stove eyes in front of them, an open fire at the front with a
spit turned by a chain and a gridiron over the coals, a hanging bar under
the hood where the smoke rises, and a tall flue with a cowl that turns away
from the wind. Two new items, the range and the copper boiler. Nothing of
the game's is replaced.

## Requirements

- Sailwind, BepInEx 5 (installed by Thunderstore Mod Manager / r2modman)

Optional: **Configuration Manager** (F1) to change settings in the game.

## Install

Unzip into `BepInEx\plugins\`. You should get:

    BepInEx\plugins\GalleyRange\GalleyRange.dll
    BepInEx\plugins\GalleyRange\galleyrange

Both files must sit together: `galleyrange` is the model. With a mod
manager, just install the package.

## Where to buy it

At the **Fort** (island 15), along the row from the two stock Aestrin
stoves: the range, then two copper boilers beside it.

| Item | Price (before the local rate) | Weight | Size |
|---|---|---|---|
| Galley range | 7,500 | 400 kg | 1.8 m wide, 2.0 m deep, 1.8 m tall, flue above that |
| Copper boiler | 600 | 8 kg empty | 48 cm across, 49 cm tall |

For comparison the Aestrin stove is 2,600 and the big pot 250.

## Setting it up

1. **Have your ship at the Fort before you buy.** Carry the range aboard
   and set it down; it is big and heavy, carried in both arms like the
   stock stoves. Do not leave it on the quay and sail off for a ship: the
   game throws away anything bought and left ashore once you are 600 m
   away. That is the game's own rule for every item, not the mod's.
2. **Nail it down** with the hammer, like any stove.
3. **The fire lights only on a large ship.** With the range nailed down,
   put firewood in the firebox at the front. If the ship is too small, or
   the range is loose, the firewood will not go in and the range's name
   says why when you look at it: *nail it down first*, *needs a ship*, or
   *needs a larger ship* with that ship's name and weight.
   - Allowed ships: any whose name holds one of the words in F1 **Ships >
     Only on these ships** (to start: Chronian, Leopard, Clipper, Gloriana),
     or any ship whose hull weighs more than F1 **Or any ship heavier than
     (kg)** (10,000 to start; the game's medium hulls weigh 5 to 11 tonnes,
     its large ones 12 to 14; cargo does not count).
   - The log (`BepInEx\LogOutput.log`) names every ship that was refused,
     so you can add a name to the list.
4. Set the two copper boilers into the two copper rims on the top at the
   back. They snap in.

## Cooking

The range is one stove with seven cook places. Each place does its own job:

| Place | Where | What goes there | How it cooks |
|---|---|---|---|
| Two boiler wells | the copper rims at the back | copper boilers | like the Aestrin stove (cooking 0.5) |
| Two stove eyes | the flat top in front of the wells | the game's pot, big pot or kettle | like the Aestrin stove |
| The spit | the rod across the front | fish, meat, any loose food | like the Aestrin stove; it turns while the fire burns, and the food turns with it |
| The gridiron | over the coals behind the front bars | loose food | like the Aestrin stove |
| The smoke bar | the hooks under the hood lip | loose food | gently, and it smokes it, like the game's smoking racks |

- **Firewood:** the firebox holds 6 pieces (3 to 12 in F1). One fire heats
  every place.
- **Putting things on:** hold the item and click the range. A boiler goes
  to a well, a pot or kettle to an eye, loose food to the spit, the
  gridiron or the smoke bar: whichever free place is nearest where you are
  looking. You can also just set a thing down on its place.
- **The copper boiler** holds 60 units of water (20 to 120 in F1); the
  game's big pot holds 20. Fill it from water bottles and put food in, as
  with any pot. **To serve:** hold an ordinary pot or kettle and click the
  boiler; it fills from the boiler, soup and all, as much as it takes. You
  cannot drink straight from the boiler: it is too big to tip up.
- Smoked food is made on the smoke bar the same way the game's smoking
  racks make it. There is no new "grilled" state: the spit and gridiron
  cook food, which is what grilling is in this game.

## The flue and cowl

- **Range > Chimney length (m):** how tall the flue stands above the hood,
  0.3 to 3.5 m, on every galley range at once, so it can clear a deck above
  or be lowered under a beam.
- **Range > Cowl turns from the wind:** on, the cowl's mouth turns away
  from the wind by itself. Off, it points where **Cowl facing (degrees)**
  says (0 = the front of the range).
- Smoke comes out of the cowl's mouth.

## Settings (F1)

All in F1, or in `BepInEx\config\com.dixiecapt.sailwind.galleyrange.cfg`.

- **Range:** chimney length, cowl turning and facing, spit turns, firewood
  it holds, price.
- **Ships:** the ship name list, the weight rule, and *Also ashore* to let
  the fire light in a house or on a quay too.
- **Boiler:** capacity, price.
- **Shop:** sell at the Fort, how many boilers, where the spot is along the
  stove row and sideways. The mod looks further along the row by itself
  if the first spot lands outside the shop.

Firewood, price and boiler capacity are read when the game starts.

## Taking it out

**A save with a galley range or a copper boiler in it needs this mod to
load**, the same as any mod that adds new items. Before you remove the mod,
sell or throw away every range and boiler, then save.

If only the `galleyrange` model file goes missing, your range comes back as
a plain Aestrin stove and your boilers as big pots, so the save still
loads. Put the file back and they are themselves again.

## Credits

- Stove model: *Brodie Stove* by **Uhlan**, licensed under Creative
  Commons Attribution-NonCommercial 4.0
  (https://creativecommons.org/licenses/by-nc/4.0/). Changed for the
  game: the lids taken off for the lift-out boilers, copper rims, a
  gridiron and a smoke bar added, the cowl set on the flue, the mesh
  thinned.
- Cooking, fire, smoke and sounds: the game's own Aestrin stove and big
  pot.

## Version history

- **0.1.0:** first build.
