# Data Schemas (Notes)

This repo uses:
- **Markdown** for human-readable rules/docs
- **JSON** for machine-readable campaign data (maps, installations, spawns, tokens)

## Maps (`/maps/<map_name>/map_layout_v1.json`)
Minimum recommended fields:
- `map_id` (string)
- `name` (string)
- `version` (string)
- `hexes` (array of hex objects)

Hex object:
- `q`, `r` axial coords (integers)
- `terrain` (string) e.g., normal, urban, industrial, wasteland
- `installation_id` (string|null) if a special installation exists on that hex
- `notes` (string, optional)

## Installations (`/data/installations_v1.json`)
Installation object:
- `id` (string)
- `name` (string)
- `effect_text` (string)  # keep as a single block at first
- `timing` (string)       # pre_battle, in_battle, post_battle, campaign_round
- `limits` (string)       # once per battle, once per round, etc.

## Spawns (`/maps/<map_name>/spawns_v1.json`)
- One or more spawn points per faction/team.
Spawn object:
- `faction_id` (string)
- `label` (string)
- `q`, `r` (integers)

## Tokens (`/maps/<map_name>/tokens_v1.json`)
Token object:
- `token_id` (string)
- `player_name` (string)
- `faction_id` (string)
- `q`, `r` starting coords (integers)
- `status` (active|reinforcing)

Keep v1 schemas intentionally simple. Tighten later after playtests.
