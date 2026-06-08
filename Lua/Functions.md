# `div`

## Description

Integer division. Lua's default integer division rounds towards negative
infinity, but this rounds towards zero. This is necessary for compatibility
with code which was converted from C++, as C++'s integer division also rounds
towards zero. An instance of code which depends on C++'s rounding behaviour is
the Mimiga Village boss Balrog, whom fails to come to a complete stop and
remains stuck in place indefinitely.

## Parameters

| Type    | Name       | Description                  |
|---------|------------|------------------------------|
| Integer | `dividend` | The number to be divided.    |
| Integer | `divisor`  | The number to be divided by. |

## Return Value

(Integer) `dividend` divided by `divisor`.

## See Also

- `mod`



# `mod`

## Description

Similar to `div`, except it computes the remainder of a division.

## Parameters

| Type    | Name       | Description                  |
|---------|------------|------------------------------|
| Integer | `dividend` | The number to be divided.    |
| Integer | `divisor`  | The number to be divided by. |

## Return Value

(Integer) The remainder of `dividend` divided by `divisor`.

## See Also

- `div`




# `AddExpMyChar`

## Description

Gives EXP to a player.

## Parameters

| Type    | Name    | Description                          |
|---------|---------|--------------------------------------|
| Integer | `mc_no` | The ID of the player to give EXP to. |
| Integer | `x`     | How much EXP to give the player.     |

## Return Value

None.



# `AddWaterCollision`

## Description

Collides player with physical water.

Only matters when physical water is enabled in `Settings.json`.

## Parameters

| Type   | Name | Description                 |
|--------|------|-----------------------------|
| MYCHAR | `mc` | The player to collide with. |

## Return Value

None.



# `AdjustMyCharRect`

## Description

Adjusts player's sprite RECT to account for the selected costume.

## Parameters

| Type    | Name    | Description                                        |
|---------|---------|----------------------------------------------------|
| Integer | `mc_no` | The ID of the player whose RECT is being adjusted. |
| RECT    | `rect`  | The player's sprite RECT.                          |

## Return Value

None.



# `bossHPMultiply`

## Description

Scales a boss's health value to account for the number of players. With
multiple players, boss health is 1.5x higher.

## Parameters

| Type    | Name    | Description        |
|---------|---------|--------------------|
| Integer | `value` | Boss health value. |

## Return Value

(Integer) `value` scaled to account for the number of players.



# `BackgroundBlowsItemsLeft`

Indicates whether things like EXP, health, and ammunition should gravitate to
the left, as they do in the Outer Wall and the Ironhead boss battle.

## Parameters

None.

## Return Value

(Boolean) `true` if items should gravitate to the left, `false` otherwise.



# `ChangeMapParts`

## Description

Changes the map tile at the position specified by `x` and `y` to the tile
specified by `no`.

## Parameters

| Type    | Name | Description        |
|---------|------|--------------------|
| Integer | `x`  | Tile X coordinate. |
| Integer | `y`  | Tile Y coordinate. |
| Integer | `no` | Tile index.        |

## Return Value

(Boolean) `false` if the coordinates were out-of-bounds, `true` otherwise.

## See Also

- `DeleteMapParts`



# `ChangeToFirstArms`

## Description

Makes the player switch to their first weapon. This was presumably used in the
fabled 'Cave Story Beta', back when weapons like the Fireball had limited ammo.

## Parameters

| Type    | Name    | Description                            |
|---------|---------|----------------------------------------|
| Integer | `mc_no` | The ID of the player to switch weapon. |

## Return Value

None.



# `ChargeArmsEnergy`

## Description

Adds ammunition to the player's current weapon.

## Parameters

| Type    | Name    | Description                      |
|---------|---------|----------------------------------|
| Integer | `mc_no` | The ID of the player.            |
| Integer | `num`   | The amount of ammunition to add. |

## Return Value

None.

## See Also

- `ChargeUnequippedEnergy`
- `UseArmsEnergy`



# `ChargeUnequippedEnergy`

## Description

Adds ammunition to one of the player's weapons.

## Parameters

| Type    | Name       | Description                      |
|---------|------------|----------------------------------|
| Integer | `mc_no`    | The ID of the player.            |
| Integer | `WeaponNo` | The ID of the weapon.            |
| Integer | `Energy`   | The amount of ammunition to add. |

## Return Value

None.

## See Also

- `ChargeArmsEnergy`
- `UseArmsEnergy`



# `CountArmsBullet`

## Description

Counts how many instances of a weapon's bullets there currently are, from a
specific player.

## Parameters

| Type    | Name        | Description                                  |
|---------|-------------|----------------------------------------------|
| Integer | `mc_no`     | The ID of the player.                        |
| Integer | `arms_code` | The ID of the weapon whose bullets to count. |

## Return Value

(Integer) The number of bullets that currently exists which were created by the
player.

## See Also

- `CountArmsBulletAll`
- `CountBulletNum`



# `CountArmsBulletAll`

## Description

Counts how many instances of a weapon's bullets there currently are, from all
players.

## Parameters

| Type    | Name        | Description                                  |
|---------|-------------|----------------------------------------------|
| Integer | `arms_code` | The ID of the weapon whose bullets to count. |

## Return Value

(Integer) The number of bullets that currently exists which were created by all
players.

## See Also

- `CountArmsBullet`
- `CountBulletNum`



# `CountBulletNum`

## Description

Counts how many instances of a bullet there currently are, for a specific
player.

This differs from `CountArmsBullet` in that a weapon can have multiple
different types of bullet associated with it, whereas this only counts one
specific type of bullet.

## Parameters

| Type    | Name          | Description                    |
|---------|---------------|--------------------------------|
| Integer | `mc_no`       | The ID of the player.          |
| Integer | `bullet_code` | The ID of the bullet to count. |

## Return Value

(Integer) The number of bullets that currently exists which were created by the
player.

## See Also

- `CountArmsBullet`
- `CountArmsBulletAll`



# `CreateFullScreenWaterVolume`

## Description

Creates a large layer of physical water which covers the screen.

Only matters when physical water is enabled in `Settings.json`.

## Parameters

None.

## Return Value

None.



# `CutNoise`

## Description

Ends river/helicopter background noises.

## Parameters

None.

## Return Value

None.

## See Also

- `SetNoise`



# `DamageMyChar`

## Description

Damages a player. Damages is halved in easy mode.

## Parameters

| Type    | Name     | Description                         |
|---------|----------|-------------------------------------|
| Integer | `mc_no`  | The ID of the player.               |
| Integer | `damage` | The amount to damage the player by. |

## Return Value

None.



# `DeleteBullet`

## Description

Deletes every instance of a particular weapon's bullets.

## Parameters

| Type    | Name   | Description                                   |
|---------|--------|-----------------------------------------------|
| Integer | `code` | The ID of the weapon whose bullets to delete. |

## Return Value

None.



# `DeleteMapParts`

## Description

Sets the map tile at the given coordinates to tile 0 (blank).

## Parameters

| Type    | Name | Description                             |
|---------|------|-----------------------------------------|
| Integer | `x`  | The X coordinate of the tile to delete. |
| Integer | `y`  | The Y coordinate of the tile to delete. |

## Return Value

None.

## See Also

- `ChangeMapParts`



# `DeleteNpCharCode`

## Description

Deletes all NPCs with a particular ID.

## Parameters

| Type    | Name     | Description                                |
|---------|----------|--------------------------------------------|
| Integer | `code`   | The ID of the NPCs to be deleted.          |
| Boolean | `bSmoke` | Make deleted NPCs create a cloud of smoke. |

## Return Value

None.



# `FindNpCharByEvent`

## Description

Find the first NPC with a particular event code.

## Parameters

| Type    | Name          | Description                                          |
|---------|---------------|------------------------------------------------------|
| Integer | `code_event`  | The event code of the NPC to be found.               |
| Boolean | `start_index` | Where in the NPC array to begin searching (0-based). |

## Return Value

(Integer) The index of the found NPC within `gNPC` (0-based).

## See Also

- `gNPC`



# `GetArktan`

## Description

Compute arctangent.

## Parameters

| Type    | Name | Description                               |
|---------|------|-------------------------------------------|
| Integer | `x`  | X coordinate, to express the input angle. |
| Integer | `y`  | Y coordinate, to express the input angle. |

## Return Value

(Integer) The arctangent, expressed as a number between 0 and 255 (inclusive).

## See Also

- `GetCos`
- `GetSin`



# `GetAttributeRaw`

## Description

Get raw attribute data of the map tile at the given coordinate. This data
combines the tile's type with its sand attribute property. The sand attribute
can be extracted with `IsSandAttribute` and the `ATRB_SAND_MASK` constant.

## Parameters

| Type    | Name | Description                                               |
|---------|------|-----------------------------------------------------------|
| Integer | `x`  | The X coordinate of the tile to obtain attribute data of. |
| Integer | `y`  | The Y coordinate of the tile to obtain attribute data of. |

## Return Value

(Integer) The tile's raw attribute data.

## See Also

- `ATRB` constants.
- `IsSandAttribute`



# `GetCos`

## Description

Compute cosine.

## Parameters

| Type    | Name     | Description                                                       |
|---------|----------|-------------------------------------------------------------------|
| Integer | `degree` | Input angle, expressed as a number between 0 and 255 (inclusive). |

## Return Value

(Integer) The cosine, expressed as a number between -511 and 511 (inclusive).

## See Also

- `GetArktan`
- `GetSin`



# `GetDifficulty`

## Description

Gets the game's current difficulty.

## Parameters

None.

## Return Value

(Integer) The difficulty level (see `Constants/DIFFICULTY.md`).



# `GetFramePositionX`

## Description

Get X coordinate of the camera's position within the level.

## Parameters

None.

## Return Value

(Integer) The X coordinate of the camera's position within the level.

## See Also

- `GetFramePositionY`



# `GetFramePositionY`

## Description

Get Y coordinate of the camera's position within the level.

## Parameters

None.

## Return Value

(Integer) The Y coordinate of the camera's position within the level.

## See Also

- `GetFramePositionX`



# `GetMapHeight`

## Description

Get height of the level, measured in tiles.

## Parameters

None.

## Return Value

(Integer) The height of the level, measured in tiles.

## See Also

- `GetMapWidth`



# `GetMapWidth`

## Description

Get width of the level, measured in tiles.

## Parameters

None.

## Return Value

(Integer) The width of the level, measured in tiles.

## See Also

- `GetMapHeight`



# `GetNPCFlag`

## Description

Get the specified NPC flag.

## Parameters

| Type    | Name | Description                         |
|---------|------|-------------------------------------|
| Integer | `a`  | ID of the NPC flag to be retrieved. |

## Return Value

(Boolean) The requested NPC flag.



# `GetNpCharIndex`

## Description

Gets the index of the NPC within the `gNPC` array (0-based).

## Parameters

| Type   | Name  | Description                       |
|--------|-------|-----------------------------------|
| NPCHAR | `npc` | The NPC to retrieve the index of. |

## Return Value

(Integer) The index of the NPC within the `gNPC` array (0-based).

## See Also

- `gNPC`



# `GetSin`

## Description

Compute sine.

## Parameters

| Type    | Name     | Description                                                       |
|---------|----------|-------------------------------------------------------------------|
| Integer | `degree` | Input angle, expressed as a number between 0 and 255 (inclusive). |

## Return Value

(Integer) The sine, expressed as a number between -511 and 511 (inclusive).

## See Also

- `GetArktan`
- `GetCos`



# `HitNpCharMap`

## Description

Perform collision of the NPC with the level. Normally, this is done
automatically by the game engine, but it can be called manually to perform
multiple collision checks within a single frame, like the H/V triggers (NPC 46)
do.

This modifies the NPC's `flag` variable to indicate collision, and sets the
`ym` variable to 0 when a top or bottom collision occurs.

## Parameters

| Type   | Name  | Description                        |
|--------|-------|------------------------------------|
| NPCHAR | `npc` | The NPC to perform collision with. |

## Return Value

None.



# `IsActiveSomeBullet`

## Description

Checks if any instances of 'special' bullets exist.

A bullet's 'special' property is defined in its `Metadata.json` file.

By default, the 'special' bullet IDs are 13, 14, 15, 16, 17, 18, 23, 25, 26,
27, 28, 29, 30, 31, 32, and 33.

## Parameters

None.

## Return Value

(Boolean) `true` if any instances of 'special' bullets exist, `false` otherwise.



# `IsMaxExpMyChar`

## Description

Checks if the player's current weapon is at its maximum EXP.

## Parameters

| Type    | Name     | Description           |
|---------|----------|-----------------------|
| Integer | `mc_no`  | The ID of the player. |

## Return Value

(Boolean) `true` if the player's current weapon is at its maximum EXP, `false`
otherwise.



# `IsSandAttribute`

## Description

Checks if the given tile attribute has its sand flag set.

Map tiles with the sand attribute flag set cause the sand caret to appear when
a player walks on it.

## Parameters

| Type    | Name   | Description         |
|---------|--------|---------------------|
| Integer | `atrb` | The tile attribute. |

## Return Value

(Boolean) `true` if the tile attribute's sand flag is set, `false` otherwise.

## See Also

- `ATRB` constants.
- `GetAttributeRaw`



# `LoseNpChar`

## Description

Destroy an NPC, randomly dropping EXP or health.

If the NPC's `BITS_VIEWDAMAGE` flag is set, then the NPC is not actually
destroyed unless the `bVanish` parameter is `true`.

## Parameters

| Type    | Name      | Description                        |
|---------|-----------|------------------------------------|
| NPCHAR  | `npc`     | The NPC to destroy.                |
| Boolean | `bVanish` | Replace destroyed NPC with NPC 3.  |

## Return Value

None.



# `moveNPCrelative`

## Description

Move NPCs with the specified event by the specified amount.

## Parameters

| Type    | Name         | Description                               |
|---------|--------------|-------------------------------------------|
| Integer | `code_event` | Event code of the NPCs to move.           |
| Integer | `xm`         | Amount to move the NPCs by on the X axis. |
| Integer | `ym`         | Amount to move the NPCs by on the Y axis. |

## Return Value

None.



# `NpCharSetNearestXYTargetMC`

## Description

Set NPC's 'tgt_mc' variable to the player that is closest on the X and Y axis.

## Parameters

| Type   | Name  | Description                               |
|--------|-------|-------------------------------------------|
| NPCHAR | `npc` | The NPC to set the 'tgt_mc' variable of.  |

## Return Value

None.

## See Also

- `NpCharSetNearestXTargetMC`
- `NpCharSetNearestYTargetMC`



# `NpCharSetNearestXTargetMC`

## Description

Set NPC's 'tgt_mc' variable to the player that is closest on the X axis.

## Parameters

| Type   | Name  | Description                               |
|--------|-------|-------------------------------------------|
| NPCHAR | `npc` | The NPC to set the 'tgt_mc' variable of.  |

## Return Value

None.

## See Also

- `NpCharSetNearestXYTargetMC`
- `NpCharSetNearestYTargetMC`



# `NpCharSetNearestYTargetMC`

## Description

Set NPC's 'tgt_mc' variable to the player that is closest on the Y axis.

## Parameters

| Type   | Name  | Description                              |
|--------|-------|------------------------------------------|
| NPCHAR | `npc` | The NPC to set the 'tgt_mc' variable of. |

## Return Value

None.

## See Also

- `NpCharSetNearestXYTargetMC`
- `NpCharSetNearestXTargetMC`



# `PlaySoundObject`

## Description

Play or stop a sound.

A `mode` of 0 means to stop the sound.
A `mode` of 1 means to play the sound once.
A `mode` of -1 means to play the sound in an indefinite loop.

Sound `WAVE_SPLASH2` (ID 56) is hardcoded to play with a volume ramp and a
cooldown of 100ms.

## Parameters

| Type    | Name   | Description                               |
|---------|--------|-------------------------------------------|
| Integer | `no`   | The ID of the sound to play.              |
| Integer | `mode` | Whether to play, stop, or loop the sound. |

## Return Value

None.



# `Random`

## Description

Computes a random number, between the specified bounds.

The number is generated using the Mersenne Twister algorithm. Note that this
differs from the algorithm used by the original Freeware version of Cave Story,
which was a linear congruential generator with a multiplier of 214013 and an
increment of 2531011.

## Parameters

| Type    | Name  | Description                          |
|---------|-------|--------------------------------------|
| Integer | `min` | Lower bound of the generated number. |
| Integer | `max` | Upper bound of the generated number. |

## Return Value

None.



# `SetBullet`

## Description

Spawns a bullet.

## Parameters

| Type    | Name    | Description                            |
|---------|---------|----------------------------------------|
| Integer | `mc_no` | ID of the player whose bullet this is. |
| Integer | `no`    | ID of the bullet to spawn.             |
| Integer | `x`     | X coordinate of the bullet.            |
| Integer | `y`     | Y coordinate of the bullet.            |
| Integer | `dir`   | `direct` variable of the bullet.       |

## Return Value

None.



# `SetCaret`

## Description

Spawns a "caret" (particle effect).

## Parameters

| Type    | Name   | Description                     |
|---------|--------|---------------------------------|
| Integer | `x`    | X coordinate of the caret.      |
| Integer | `y`    | Y coordinate of the caret.      |
| Integer | `code` | ID of the caret to spawn.       |
| Integer | `dir`  | `direct` variable of the caret. |

## Return Value

Index of created caret in the `gCaret` array (0-based).

## See Also

- `gCaret`
- `CARET` constants



# `SetDestroyNpChar`

## Description

Spawns smoke-cloud NPCs (ID 4) and a `CARET_BIGSMOKE` caret (ID 12).

Unlike `SetDestroyNpCharUp`, this spawns the cloud NPCs with `DIR_LEFT`.

## Parameters

| Type    | Name  | Description                                         |
|---------|-------|-----------------------------------------------------|
| Integer | `x`   | X coordinate to spawn at.                           |
| Integer | `y`   | Y coordinate to spawn at.                           |
| Integer | `w`   | Radius for the cloud NPCs to randomly spawn within. |
| Integer | `num` | Number of cloud NPCs to spawn.                      |

## Return Value

None.

## See Also

- `SetDestroyNpCharUp`



# `SetDestroyNpCharUp`

## Description

Spawns smoke-cloud NPCs (ID 4) and a `CARET_BIGSMOKE` caret (ID 12).

Unlike `SetDestroyNpChar`, this spawns the cloud NPCs with `DIR_UP`.

## Parameters

| Type    | Name  | Description                                         |
|---------|-------|-----------------------------------------------------|
| Integer | `x`   | X coordinate to spawn at.                           |
| Integer | `y`   | Y coordinate to spawn at.                           |
| Integer | `w`   | Radius for the cloud NPCs to randomly spawn within. |
| Integer | `num` | Number of cloud NPCs to spawn.                      |

## Return Value

None.

## See Also

- `SetDestroyNpChar`



# `SetExpObjects`

## Description

Spawns a random selection of EXP shard NPCs (ID 1).

## Parameters

| Type    | Name  | Description                                 |
|---------|-------|---------------------------------------------|
| Integer | `x`   | X coordinate to spawn at.                   |
| Integer | `y`   | Y coordinate to spawn at.                   |
| Integer | `exp` | The total value of the EXP shards to spawn. |

## Return Value

None.



# `SetFlash`

## Description

Triggers a screen-spanning flash effect.

## Parameters

| Type    | Name   | Description                          |
|---------|--------|--------------------------------------|
| Integer | `x`    | X coordinate of the effect's origin. |
| Integer | `y`    | Y coordinate of the effect's origin. |
| Integer | `mode` | The ID of the flash effect.          |

## Return Value

None.

## See Also

- `FLASHMODE` constants



# `SetNoise`

## Description

Starts river/helicopter background noises.

## Parameters

| Type    | Name   | Description                                                     |
|---------|--------|-----------------------------------------------------------------|
| Integer | `no`   | ID of the background noise.                                     |
| Integer | `freq` | Frequency of the background noise (only affects `NOISE_RIVER`). |

## Return Value

None.

## See Also

- `CutNoise`
- `NOISE` constants



# `SetNpChar`

## Description

Spawns NPC.

The `start_index` parameter is useful for controlling NPC layering and ensuring
that NPCs update in a certain order. This is due to NPCs earlier in the array
both drawing and updating before NPCs later in the array. The latter is
particularly useful for parent and child NPCs, where one either controls, or
responds to, the other.

## Parameters

| Type    | Name          | Description                                                      |
|---------|---------------|------------------------------------------------------------------|
| Integer | `code_char`   | ID of the NPC to spawn.                                          |
| Integer | `x`           | NPC's X coordinate.                                              |
| Integer | `y`           | NPC's Y coordinate.                                              |
| Integer | `xm`          | NPC's X velocity.                                                |
| Integer | `ym`          | NPC's Y velocity.                                                |
| Integer | `dir`         | NPC's X direction.                                               |
| NPCHAR  | `npc`         | NPC's parent.                                                    |
| Integer | `start_index` | Earliest slot of the `gNPC` array to spawn the NPC in (0-based). |

## Return Value

Index of created NPC in the `gNPC` array (0-based).

## See Also

- `gNPC`



# `SetQuake`

## Description

Triggers minor screen-shaking effect, and rumbles controller.

## Parameters

| Type    | Name   | Description                                |
|---------|--------|--------------------------------------------|
| Integer | `time` | Duration of the quake, measured in frames. |

## Return Value

None.

## See Also

- `SetQuake2`
- `SetQuakeWithoutRumble`



# `SetQuake2`

## Description

Triggers major screen-shaking effect, and rumbles controller.

## Parameters

| Type    | Name   | Description                                |
|---------|--------|--------------------------------------------|
| Integer | `time` | Duration of the quake, measured in frames. |

## Return Value

None.

## See Also

- `SetQuake`
- `SetQuakeWithoutRumble`



# `SetQuakeWithoutRumble`

## Description

Triggers minor screen-shaking effect, without rumbling the controller.

## Parameters

| Type    | Name   | Description                                |
|---------|--------|--------------------------------------------|
| Integer | `time` | Duration of the quake, measured in frames. |

## Return Value

None.

## See Also

- `SetQuake`
- `SetQuake2`




# `StartTextScript`

## Description

Runs a TSC script.

If `mc_no` is less than 0, then the player associated with the script is left
unchanged.

## Parameters

| Type    | Name    | Description                                    |
|---------|---------|------------------------------------------------|
| Integer | `mc_no` | ID of the player to associate the script with. |
| Integer | `no`    | Event code of the script to run.               |

## Return Value

(Boolean) `true` if the event code could be found, `false` otherwise.




# `UseArmsEnergy`

## Description

Expends ammunition of the player's current weapon.

## Parameters

| Type    | Name    | Description                               |
|---------|---------|-------------------------------------------|
| Integer | `mc_no` | ID of the player whose ammunition to use. |
| Integer | `num`   | Amount of ammunition to use.              |

## Return Value

(Boolean) `true` if the player ID was valid, `false` otherwise.

## See Also

- `ChargeArmsEnergy`
- `ChargeUnequippedEnergy`



# `VanishNpChar`

## Description

Replaces NPC with NPC ID 3, which is invisible and despawns after 100 frames.
This NPC is used for anchoring the damage number ("value view") to the spot
where the NPC was destroyed.

## Parameters

| Type   | Name  | Description    |
|--------|-------|----------------|
| NPCHAR | `npc` | NPC to vanish. |

## Return Value

None.



# `ZeroExpMyChar`

## Description

Sets the player's current weapon to level 1 their EXP to 0.

## Parameters

| Type    | Name    | Description       |
|---------|---------|-------------------|
| Integer | `mc_no` | ID of the player. |

## Return Value

None.
