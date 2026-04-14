NPC/boss traits.

# `BITS_BLOCK_MYCHAR`

Player bounces off of this NPC/boss.

# `BITS_THROW_EBLOCK`

Ignores collision with tiles with attribute `ATRB_EBLOCK`.

# `BITS_BLOCK_BULLET`

Blocks bullets, using their `blockXL` and `blockYL` radii.

# `BITS_THROW_BLOCK`

Ignore map collision entirely.

# `BITS_BOUND_MYCHAR`

When combined with `BITS_BLOCK_MYCHAR`, this makes the player only bounce
vertically when landing on top of this NPC/boss.

# `BITS_BANISH_DAMAGE`

Can be damaged by bullets, using their `enemyXL` and `enemyYL` radii.

# `BITS_BLOCK_MYCHAR2`

Player collides with this NPC/boss, similarly to `BITS_BLOCK_MYCHAR` except the
player does not bounce.

# `BITS_DAMAGE_SIDE`

Hurt the player only when touching the left and right sides of this NPC/boss.

# `BITS_EVENT_HIT`

Trigger an event upon colliding with the player.

Event is specified by `code_event` member variable.

# `BITS_EVENT_BREAK`

Trigger an event upon being destroyed.

Event is specified by `code_event` member variable.

# `BITS_EVENT_ALIVE`

Would have triggered an event so long as the NPC/boss is alive, but no
functionality for this exists, rendering this bit unused.

It has been repurposed for the horizontal/vertical trigger NPC (ID 46), to make
it move slower, just like in Cave Story's freeware version (this can also be
achieved by setting its `code_flag` member variable to 9999).

# `BITS_FLAG_ALIVE`

Causes the NPC/boss to be spawned only if a certain flag is set.

# `BITS_DIRECT_RIGHT`

Spawn with the `direct` member variable set to `DIR_RIGHT`.

# `BITS_EVENT_CHECK`

Triggers the event specified by member variable `code_event` when the player
examines it (presses the down key whilst stood in front of the NPC/boss).

# `BITS_FLAG_DEAD`

Causes the NPC/boss to be spawned only if a certain flag is clear.

# `BITS_VIEWDAMAGE`

Show a number (a so-called 'value-view') when damaged.

# `BITS_ACTION`

A bitmask for extracting "action-related bits". Particularly...
- `BITS_BLOCK_MYCHAR`
- `BITS_THROW_EBLOCK`
- `BITS_BLOCK_BULLET`
- `BITS_THROW_BLOCK`
- `BITS_BOUND_MYCHAR`
- `BITS_BANISH_DAMAGE`
- `BITS_BLOCK_MYCHAR2`
- `BITS_DAMAGE_SIDE`
- `BITS_VIEWDAMAGE`
