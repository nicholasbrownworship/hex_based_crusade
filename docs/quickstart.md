# Hex Crusade (v1) Quickstart

This is the “how to run it at the table” guide for the planet-scale hex campaign.

## What you need
- A printed or digital hex map (or a shared image)
- One Army Token per player
- A way to mark controlled hexes (colored dots, highlighter, digital layers)
- The rules: `/rules/hex_crusade_rules_v1.md`
- Installations: `/installations/installations_v1.md`

## Setup (10 minutes)
1. Choose factions/teams.
2. Place each faction’s **Spawn Hex** (see map folder `spawns_v1.json`).
3. Place Army Tokens on their faction Spawn Hex.
4. Confirm which Installation Hexes exist on the map (see `map_layout_v1.json`).

## Playing a campaign round
1. **Reinforcement Phase**  
   Return defeated tokens to Spawn Hex (or eligible Void Port, if your rules allow it).
2. **Movement Phase**  
   Each Army Token rolls 1D6 and moves hex-by-hex.
3. **Collision Phase**  
   If a token enters an enemy-occupied hex, a battle is triggered.
4. **Control Resolution**  
   Winner controls the contested hex. Loser token goes to Reinforcement Status.
5. **Recovery Phase**  
   Do Crusade post-game. Apply Medicae/Hospital installation effects if controlled.

## Battle selection
- Battles only happen on collisions. If there are multiple collisions, resolve them in any order.
- If you can’t play a collision battle that week, mark that hex as **Contested** and resolve next session.

## Victory (pick one)
- First team to control a majority of Installation Hexes at the end of a round
- Time limit (e.g., 6 rounds), then count installations controlled
- Narrative objective (GM-defined)

## Recommended “first test” (fast)
- Use a small map (10–20 hexes)
- Place 1 Spawn per faction
- Place 5–7 installations total
- Run 2 rounds and see if:
  - movement feels fun
  - collisions are frequent enough
  - any installation dominates
