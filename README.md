# MoveMeXiv

A Dalamud plugin for FFXIV that allows you to freely move your character to any coordinate, teleport, mount, and travel between worlds -- all controllable remotely via a Discord bot.

## Features

- **Coordinate Movement** - Teleport instantly or smooth-move to any X/Y/Z coordinate
- **Relative Movement** - Nudge your character by offset amounts
- **Aetheryte Teleportation** - Browse and teleport to any unlocked aetheryte
- **Mount Controls** - Mount roulette, mount by ID, dismount, take flight
- **World Travel** - Visit other worlds on the same data center
- **Cross-DC Travel** - Travel to worlds on different data centers (requires Lifestream plugin)
- **Coordinate Bookmarks** - Save and recall positions
- **Discord Bot Integration** - Control everything remotely from Discord with rich embed menus

## Installation

### Plugin
1. In FFXIV, open the Dalamud plugin installer
2. Add the custom repository URL (see Releases)
3. Search for "MoveMeXiv" and install

### Discord Bot
1. Invite the bot to your private Discord server
2. Run `/setup` in Discord to get a pairing code
3. In-game: `/mmx` > Settings tab > enter server URL and pairing code

## In-Game Commands

| Command | Description |
|---------|-------------|
| `/mmx` | Open/close the plugin window |
| `/mmxtp <x> <y> <z>` | Instant teleport to coordinates |
| `/mmxmove <x> <y> <z>` | Smooth movement to coordinates |
| `/mmxworld <worldname>` | Travel to another world |

## Discord Commands

| Command | Description |
|---------|-------------|
| `/setup` | Generate a pairing code to link your plugin |
| `/status` | Show current character position, world, and state |
| `/travel` | World travel menu with DC/world selection |
| `/moveto <x> <y> <z>` | Move character to coordinates |
| `/mount` | Mount/dismount/flight controls |
| `/bookmark save\|list` | Manage coordinate bookmarks |

## Requirements

- FFXIV with XIVLauncher and Dalamud
- .NET 8+ SDK (for building from source)
- Lifestream plugin (optional, for cross-DC travel)
