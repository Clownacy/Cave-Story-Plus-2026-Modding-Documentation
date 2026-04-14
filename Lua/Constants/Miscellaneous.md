# `MAX_AIR`

How long a player can survive underwater (measured in frames).

Current value is 1000.

# `MAX_BOSS_PARTS`

Size of the `gBoss` array.

Current value is 20.

# `MAX_BULLET`

Size of the `gBullet` array.

Current value is 128.

# `MAX_CARET`

Size of the `gCrt` array.

Current value is 64.

# `MAX_MOVE`

Maximum amount that characters can move at in a single frame (measured in world
units).

Note that this is not universally enforced; characters opt-into having a speed
limit by manually capping their X and Y velocities (`xm` and `ym` variables) to
this constant.

Current value is `3 * VS - 1`.

# `MAX_MYCHAR`

Size of the `gMC` array.

Current value is 2.

# `MAX_NPCHAR`

Size of the `gNPC` array.

Current value is 1024.

# `MUZZLE_FLASH_DURATION`

How long a weapon's muzzle-flash lasts (measured in frames).

Current value is 4.

# `PARTSSIZE`

The width and height of all level tiles (measured in screen units).

Current value is 16.

# `SURFACE_WIDTH`

The width of the screen (measured in screen units).

Current value is 426.

# `SURFACE_HEIGHT`

The height of the screen (measured in screen units).

Current value is 240.

# `VS`

The ratio between screen units and world units.

Divide a world unit by this to get a screen unit.

Divide a screen unit by this to get a world unit.

Current value is 512.

# `WAIT_NPC_DAMAGE`

How long an NPC should be stunned after being damaged (measured in frames).

Current value is 16.
