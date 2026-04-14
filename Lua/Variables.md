C++ global variables which are exposed to the Lua environment.

| Type          | Name                | Description                                                                                             |
|---------------|---------------------|---------------------------------------------------------------------------------------------------------|
| Boolean       | `_b_boss_live`      | Indicates whether G-CLONE is alive. Used by some Wind Fortress NPCs.                                    |
| Boolean Array | `_b_my_held`        | Whether player has been grabbed by a Curly Clone (length is `MAX_MYCHAR`).                              |
| Integer Array | `_empty`            | Cooldown for player's 'EMPTY!' popup (length is `MAX_MYCHAR`).                                          |
| NPCHAR Array  | `gBoss`             | Boss NPC array (length is `MAX_BOSS_PARTS`).                                                            |
| BULLET Array  | `gBul`              | Bullet array (length is `MAX_BULLET`).                                                                  |
| CARET Array   | `gCrt`              | Caret array (length is `MAX_CARET`).                                                                    |
| Integer       | `gCurlyShoot_wait`  | Controls the timing of AI Curly's actions.                                                              |
| Integer       | `gCurlyShoot_x`     | X coordinate that AI Curly is targeting (measured in world coordinates).                                |
| Integer       | `gCurlyShoot_x`     | Y coordinate that AI Curly is targeting (measured in world coordinates).                                |
| Integer       | `g_GameFlags`       | `GAMEFLAG` bitfield (see the `GAMEFLAG` constants).                                                     |
| Integer       | `gKey`              | Held button inputs for all players (see the `gKey` constants).                                          |
| Integer       | `gKeyTrg`           | Recently-pressed button inputs for all players (see the `gKey` constants).                              |
| Integer Array | `gKeyMC`            | Held button inputs for a single player (length is `MAX_MYCHAR`) (see the `gKey` constants).             |
| Integer Array | `gKeyMCTrg`         | Recently-pressed button inputs for a single player (length is `MAX_MYCHAR`) (see the `gKey` constants). |
| MYCHAR Array  | `gMC`               | Player array (length is `MAX_MYCHAR`).                                                                  |
| NPCHAR Array  | `gNPC`              | NPC array (length is `MAX_NPCHAR`).                                                                     |
| Integer       | `gNumMyChar`        | How many players currently exist.                                                                       |
| Integer       | `gQuoteOutfitP2`    | Player 2's outfit (see `P2_OUTFIT` constants).                                                          |
| Integer       | `gStageNo`          | Numerical ID of the current stage. Matches folder structure of `data/Stage/Table`.                      |
| Integer       | `gSuperXpos`        | Generic X coordinate, used by NPCs to communicate with each other.                                      |
| Integer       | `gSuperYpos`        | Generic Y coordinate, used by NPCs to communicate with each other.                                      |
| Integer       | `gWaterY`           | Y coordinate of full-screen water's surface (measured in world coordinates).                            |
| Boolean       | `rapid_fire_weapon` | Whether rapid-fire mode has been activated by an `<RFW` TSC command.                                    |
