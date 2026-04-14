Values of the `cond` member variable bitfield.

# `COND_CHECK`

NPC can be examined by the player.

# `COND_HIDE`

NPC will not be rendered.

# `COND_RUN`

Player will make running sounds.

# `COND_LOSE`

NPC will be destroyed.

# `COND_ZEROINDEXDAMAGE`

All damaged received by boss NPCs will be directed to the first boss NPC in the
`gBoss` array.

# `COND_FLOW`

Player will be blown to the left. Used during the Core boss battle.

# `COND_ALIVE`

Indicates that a slot in the `gBoss` or `gNPC` arrays is occupied, and that the
NPC exists. Clearing this will delete the NPC.

# `COND_DROWNED`

Player has drowned. Freezes the player in place and changes their sprite.
