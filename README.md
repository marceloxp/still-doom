# Still

This directory is the home of both Still mods. They stay here, separated into `doom1/` and `doom2/`. Each folder is the file GZDoom loads.

Clearing the map loads that same map again, back at the start, with the weapons and health you were carrying. Dying restarts the same cycle. Quitting, or starting a new game, resets the count.

The wad is not included. Load `doom1` or `doom2` with GZDoom.

## Still E1M1

The hangar, Ultimate Doom. Each clear adds one extra copy of every monster on the map, up to three. Every two clears, those copies step up the chain: zombie, shotgunner, imp, demon, cacodemon, baron, cyberdemon. The chaingunner stays out, because Doom 1 has no sprite for it.

```sh
gzdoom -iwad /path/to/DOOM.WAD -file doom1 -skill 4 -warp 1 1
```

## Still MAP01

The entryway, Doom 2. The map only has zombies and imps. Each clear adds one more copy of every monster, the same kind, with no cap. Copies spawn on open floor in sight of the monster they came from. A copy that does not fit is skipped.

```sh
gzdoom -iwad /path/to/DOOM2.WAD -file doom2 -skill 4 -warp 1
```
