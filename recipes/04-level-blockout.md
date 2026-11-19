# Build a level blockout

**Goal:** a greybox level to test gameplay before making real art.

## Prompt

```
In the current scene, block out a small arena level using primitives (or ProBuilder if it's
installed): a 40x40 floor, outer walls 4 units high, three platforms at different heights
reachable by jumping, two ramps and some cover boxes. Put everything under an empty parent
called Blockout, give each object a clear name, use one grey material for floors and a
darker one for walls, and save the scene.
```

## Check

- Everything is under `Blockout`, so you can move or delete it in one go.
- Play with your player controller and make sure every platform is reachable.

## If it goes wrong

- **Platforms too high to reach**: "Read the player's jump height from PlayerMovement and keep platform steps below it."
- **Objects overlapping**: "List each object's position and scale, then fix overlaps."