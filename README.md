# Still

This directory is the home of the Still mods. They stay here, separated into `doom1/`, `doom2/`, and `brutal/`. Each folder is a file GZDoom loads.

Clearing the map loads that same map again, back at the start, with the weapons and health you were carrying. Dying restarts the same cycle. Quitting, or starting a new game, resets the count.

The wad is not included. Load `doom1` or `doom2` with GZDoom.

## Still E1M1

The hangar, Ultimate Doom. Each clear adds one extra copy of every monster on the map, up to three. Every two clears, those copies step up the chain: zombie, shotgunner, imp, demon, cacodemon, baron, cyberdemon. The chaingunner stays out, because Doom 1 has no sprite for it.

```sh
gzdoom -iwad /path/to/DOOM.WAD -file doom1 -skill 4 -warp 1 1
```

## Still MAP01

The entryway, Doom 2. You start with the shotgun and the super shotgun already in hand, and shell boxes are scattered on the floor. The map only has zombies and imps. Each clear adds a random 1 to 3 more copies of every monster, the same kind, with no cap. Copies spawn on open floor in sight of the monster they came from. A copy that does not fit is skipped.

Outside, a few steps past the shotgun, a soulsphere-shaped item raises shotgun damage by 5 per pellet, for both the pump and the super shotgun. The stack stays with you when the map reloads. One to three heavier monsters stand on it: demons at first, then cacodemons, revenants, hell knights, and barons as the copies pile up. The yard is off the way north. You can leave it.

```sh
gzdoom -iwad /path/to/DOOM2.WAD -file doom2 -skill 4 -warp 1
```

## Brutal, item lá fora

Same pickup, for Brutal v21 on Plutonia with Maps of Chaos. It starts on MAP01. Clearing the map loads MAP01 again, and each clear adds a random 1 to 3 more copies of every monster. Dying restarts the same cycle. The item sits under the nearest open sky to the shotgun, with 1 to 3 heavier monsters. Each pickup adds 1 to 3 stacks, and each stack adds 5 damage per pellet. Shell boxes are scattered on the floor. The shell reserve holds 400, and the pump magazine holds 20. You can leave the item.

```sh
gzdoom -iwad /path/to/Plutonia.wad -file DoomMetalVol5.wad brutalv21.pk3 mapsofchaos-hc.wad brutal
```
