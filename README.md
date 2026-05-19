# AlchemistCraft

> **Powerful Custom Recipe Plugin for Minecraft 1.13 – 26.1.2+**

AlchemistCraft gives you complete control over your server's crafting system.
Add, remove, and manage custom recipes through an intuitive in-game GUI or commands — with full support for Spigot, Paper, and Purpur.

---

## ✨ Features

### 🆓 Free
- Unlimited custom shaped & shapeless recipes
- Remove & restore vanilla recipes
- Furnace, Blast Furnace, Smoker, Campfire recipe support
- In-game GUI Recipe Editor
- Recipe Book integration
- Import & Export recipes (.json)
- SQLite, JSON, MySQL storage support
- Full config customization
- PlaceholderAPI & Vault integration (optional)
- EXP cost recipes
- Recipe categories & tags
- Third-party item recognition (ItemsAdder, MMOItems, Oraxen)
- 14 language support
- Update notifications

### 👑 Premium
- Custom item metadata support (enchants, lore, custom name)
- Conditional recipes (permission / world / time)
- Per-player recipe cooldown & craft limit
- Random chance results
- Recipe discovery & unlock system
- Custom sounds & particles on craft
- Usage statistics & logs
- Discord Webhook integration
- Web dashboard
- Advanced third-party plugin integration (ItemsAdder, MMOItems, Oraxen, MythicMobs)
- Recipe visibility (group-based)

---

## 📥 Downloads

| Edition | Link |
|---|---|
| 🆓 Free | [GitHub Releases](../../releases/latest) |
| 👑 Premium | [Polymart](링크) · [BuiltByBit](링크) |

---

## 🔧 Requirements

| Item | Requirement |
|---|---|
| Minecraft | 1.13 – 26.1.2+ |
| Java | 17 or higher (25+ for 26.1+) |
| Server | Spigot / Paper / Purpur |

### Optional Dependencies
- [Vault](https://www.spigotmc.org/resources/vault.34315/)
- [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/)
- [ItemsAdder](https://www.spigotmc.org/resources/itemsadder.73355/)
- [MMOItems](https://www.spigotmc.org/resources/mmoitems-premium.39267/)
- [Oraxen](https://www.spigotmc.org/resources/oraxen.72448/)

---

## 🚀 Quick Start

1. Download `AlchemistCraft-free-x.x.x.jar` from [Releases](../../releases/latest)
2. Place the jar in your server's `/plugins` folder
3. Restart your server
4. Edit `plugins/AlchemistCraft/config.yml` as needed
5. Use `/ac reload` to apply changes without restarting

---

## 💬 Commands

| Command | Description |
|---|---|
| `/ac recipe add <name>` | Add a new recipe (opens GUI) |
| `/ac recipe remove <name>` | Remove a custom or vanilla recipe |
| `/ac recipe list` | Browse all recipes |
| `/ac recipe info <name>` | Show recipe details |
| `/ac recipe enable/disable <name>` | Toggle a recipe |
| `/ac import <file>` | Import recipes from .json |
| `/ac export <file>` | Export recipes to .json |
| `/ac reload` | Reload the plugin |
| `/ac help` | Show help |

Full command reference → [Wiki: Commands](../../wiki/Commands)

---

## 🔑 Permissions

| Permission | Description | Default |
|---|---|---|
| `alchemistcraft.admin` | Full access | OP |
| `alchemistcraft.recipe.add` | Add & edit recipes | OP |
| `alchemistcraft.recipe.remove` | Remove recipes | OP |
| `alchemistcraft.recipe.list` | View recipe list | Everyone |
| `alchemistcraft.gui.view` | Open recipe view GUI | Everyone |
| `alchemistcraft.gui.edit` | Open recipe editor GUI | OP |
| `alchemistcraft.import` | Import recipes | OP |
| `alchemistcraft.export` | Export recipes | OP |
| `alchemistcraft.reload` | Reload plugin | OP |

Full permission reference → [Wiki: Permissions](../../wiki/Permissions)

---

## 🌐 Language Support

AlchemistCraft supports **14 languages** out of the box.
Set your language in `config.yml`:

```yaml
language: en  # en, ko, ja, zh_CN, zh_TW, de, fr, es, pt_BR, ru, pl, nl, tr, vi
```

---

## 🗄️ Storage Options

Configure your preferred storage in `config.yml`:

```yaml
storage:
  type: SQLITE  # SQLITE / JSON / MYSQL
```

| Type | Description |
|---|---|
| SQLite | Default. No setup required. |
| JSON | File-based. Simple and lightweight. |
| MySQL | External database. Recommended for large servers. |

---

## ❌ Error Codes

If an error occurs, AlchemistCraft will display a code like `ERROR_5` or `UNKNOWN-7A3F2B`.

- Known errors (`ERROR_1` ~ `ERROR_14`) → [Wiki: Error Codes](../../wiki/Error-Codes)
- Unknown errors (`UNKNOWN-XXXXXX`) → Please [open an issue](../../issues) with the code

---

## 🔗 Links

| | |
|---|---|
| 📖 Wiki | [GitHub Wiki](../../wiki) |
| 🐛 Bug Report | [GitHub Issues](../../issues) |
| 💬 Discord | [링크 추후 추가] |
| 🛒 SpigotMC | [링크 추후 추가] |
| 👑 Polymart | [링크 추후 추가] |
| 👑 BuiltByBit | [링크 추후 추가] |

---

## 📄 License

AlchemistCraft Free is provided as-is for use on your Minecraft server.
Redistribution or modification of the plugin files is not permitted.
