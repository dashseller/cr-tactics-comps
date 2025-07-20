# Troop IDs Reference

This document lists all troop IDs and their corresponding display names for the CR Tactics game.

> **Note:** Troop IDs are **kebab-case** (hyphen-separated). Underscore (`_`) forms are deprecated—update any legacy data or code using underscores.

## Troop ID → Name Mapping

| ID | Name |
|---|---|
| `archer` | Archers |
| `barbarian` | Barbarians |
| `bomber` | Bomber |
| `goblin` | Goblins |
| `knight` | Knight |
| `spear-goblin` | Spear Goblins |
| `dart-goblin` | Dart Goblin |
| `executioner` | Executioner |
| `giant-skeleton` | Giant Skeleton |
| `pekka` | P.E.K.K.A |
| `prince` | Prince |
| `valkyrie` | Valkyrie |
| `bandit` | Bandit |
| `goblin-machine` | Goblin Machine |
| `mega-knight` | Mega Knight |
| `princess` | Princess |
| `royal-ghost` | Royal Ghost |
| `archer-queen` | Archer Queen |
| `golden-knight` | Golden Knight |
| `skeleton-king` | Skeleton King |

## Usage

These IDs appear in:

- **Team Compositions**: (e.g. `team-comps.json`) inside each composition’s `troops` array.
- **Game State / Board Placement**: Used to reference troop data.
- **Filtering & Search**: UI components rely on these canonical IDs.
- **Ruler Field**: Each composition references the active ruler via `"ruler": "<ruler-id>"`. (Currently only one ruler: `royale-king` — adjust if/when more rulers become active.)

## Example Composition (JSON)

```json
{
  "tier": "S",
  "name": "Clan Avenger",
  "troops": [
    { "id": "barbarian", "stars": 2 },
    { "id": "archer", "stars": 2 },
    { "id": "valkyrie", "stars": 2 },
    { "id": "mega-knight", "stars": 2 },
    { "id": "bandit", "stars": 2 },
    { "id": "archer-queen", "stars": 2 }
  ],
  "ruler": "royale-king",
  "alts": {
    "groups": [
      {
        "replace": ["mega-knight"],
        "with": ["pekka"]
      }
    ]
  }
}
