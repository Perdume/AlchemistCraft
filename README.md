# AlchemistCraft

**Advanced Custom Recipe Plugin for Minecraft 1.13 – 1.21+**  
Spigot · Paper · Purpur

---

## What is AlchemistCraft?

AlchemistCraft is a premium-grade recipe management plugin that lets server administrators create, edit, and control every recipe — entirely through an in-game GUI, no config editing required.

---

## Features

### Recipe Types
| Type | Station |
|---|---|
| Crafting Table (Shaped) | Crafting Table |
| Crafting Table (Shapeless) | Crafting Table |
| Furnace | Furnace |
| Blast Furnace | Blast Furnace |
| Smoker | Smoker |
| Campfire | Campfire |
| Stonecutter | Stonecutter |
| Smithing | Smithing Table |

### Ingredient Matching
- **Material** — any item of that material type
- **NBT / PDC** — exact ItemStack match including metadata, enchantments, custom model data, PersistentDataContainer
- **ItemsAdder** — match by `namespace:id`
- **MMOItems** — match by `TYPE:ID`
- **Oraxen** — match by item id

### Economy & Access Control
- **EXP cost** — require experience levels per craft (per-recipe, configurable)
- **Vault cost** — require currency per craft (per-recipe, configurable)
- **Craft permission** — restrict individual recipes to any permission node

### Storage Backends
| Backend | Use Case |
|---|---|
| SQLite | Default — zero setup, single server |
| JSON | Human-readable flat files |
| MySQL | Shared storage across multiple servers |

### Plugin Compatibility
| Plugin | Support |
|---|---|
| Vault | Economy integration (craft costs) |
| PlaceholderAPI | Placeholder expansion |
| ItemsAdder | Custom item ingredients & results |
| MMOItems | Custom item ingredients & results |
| Oraxen | Custom item ingredients & results |

### Other Highlights
- Full **in-game GUI editor** — create and edit recipes without touching any files
- **Vanilla recipe control** — toggle any vanilla recipe on/off per-server
- **Custom cook time & XP** — configure per-recipe for all furnace-type stations
- **Import / Export** — share recipe packs as JSON files
- **14 languages** — en, ko, ja, zh_CN, zh_TW, de, fr, es, pt_BR, ru, pl, nl, tr, vi
- **Developer API** — programmatically add/remove/toggle recipes from other plugins
- **Event API** — `RecipeAddEvent`, `RecipeRemoveEvent`, `RecipeToggleEvent`, `VanillaRecipeToggleEvent`
- **Internal diagnostics** — `/ac test` for live plugin health checks

---

## Quick Start

1. Drop `AlchemistCraft.jar` into your `plugins/` folder
2. Restart the server
3. Run `/ac` in-game to open the recipe list GUI
4. Click the **+** (Emerald) button to create a new recipe
5. Set ingredients, result item, and recipe type — then click **Save**

---

## Commands

| Command | Description | Permission |
|---|---|---|
| `/ac` | Open recipe list GUI | `alchemistcraft.gui.view` |
| `/ac recipe add <name>` | Create a new recipe | `alchemistcraft.recipe.add` |
| `/ac recipe remove <name>` | Delete a recipe | `alchemistcraft.recipe.remove` |
| `/ac recipe list [page]` | List all recipes | `alchemistcraft.recipe.list` |
| `/ac recipe info <name>` | Show recipe details | `alchemistcraft.recipe.list` |
| `/ac recipe enable <name>` | Enable a recipe | `alchemistcraft.recipe.add` |
| `/ac recipe disable <name>` | Disable a recipe | `alchemistcraft.recipe.add` |
| `/ac import <file>` | Import recipes from JSON | `alchemistcraft.import` |
| `/ac export <file>` | Export recipes to JSON | `alchemistcraft.export` |
| `/ac reload` | Reload all plugin data | `alchemistcraft.reload` |
| `/ac debug` | Toggle debug mode | `alchemistcraft.debug` |
| `/ac test [category]` | Run internal diagnostics | `alchemistcraft.test` |

---

## Configuration (excerpt)

```yaml
language: en          # en, ko, ja, zh_CN, zh_TW, de, fr, es, pt_BR, ru, pl, nl, tr, vi

storage:
  type: SQLITE        # SQLITE / JSON / MYSQL

features:
  vault-integration: true
  exp-cost: true
  craft-permission: true

recipe-defaults:
  furnace:
    cook-time: 200    # ticks (200 = 10s)
    cook-xp: 0.1
```

Full reference → [Wiki: Configuration](wiki/Configuration.md)

---

## Requirements

- Java 17 or higher
- Spigot / Paper / Purpur 1.13+

---

## Downloads

| Version | Link |
|---|---|
| Latest | [Polymart](링크) / [BuiltByBit](링크) |

---

## Links

- [Wiki](wiki/Home.md)
- [Bug Report](../../issues)
- [Discord](discord 링크)
- [Developer API](wiki/Developer-API.md)

---

## Supported Versions

- Minecraft: 1.13 – 1.21+
- Java: 17+
- Server: Spigot / Paper / Purpur
