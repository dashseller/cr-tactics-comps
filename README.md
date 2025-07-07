# Troop IDs Reference

This document provides a reference table for all troop IDs and their corresponding names in the CR Tactics game.

## Troop ID to Name Mapping

| ID | Name |
|---|---|
| `archer` | Archers |
| `barbarian` | Barbarians |
| `bomber` | Bomber |
| `goblin` | Goblins |
| `knight` | Knight |
| `spear_goblin` | Spear Goblins |
| `dart_goblin` | Dart Goblin |
| `executioner` | Executioner |
| `giant_skeleton` | Giant Skeleton |
| `pekka` | P.E.K.K.A |
| `prince` | Prince |
| `valkyrie` | Valkyrie |
| `bandit` | Bandit |
| `goblin_machine` | Goblin Machine |
| `mega_knight` | Mega Knight |
| `princess` | Princess |
| `royal_ghost` | Royal Ghost |
| `archer_queen` | Archer Queen |
| `golden_knight` | Golden Knight |
| `skeleton_king` | Skeleton King |

## Usage

These IDs are used throughout the application:

- **Team Compositions**: In `team-comps.ts`, the `cards` array contains these troop IDs
- **Game State**: When placing troops on the board
- **Filtering**: When searching or filtering troops in the UI

## Example

```typescript
// In team-comps.ts
{
  id: 1,
  tier: "S",
  name: "Clan Avengers",
  cards: ["barbarian", "archer", "valkyrie", "mega_knight", "bandit", "archer_queen"]
}
```

The system automatically resolves these IDs to full troop objects with stats, traits, and images from the `TROOPS` array.