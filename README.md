# MoveMeXiv

A Dalamud plugin for FFXIV that provides destination-first travel — get your character to any location (data center, world, aetheryte, or coordinates) through a unified flow, controllable both in-game and remotely via Discord.

## Features

- **Unified "Go To" Travel** - Chain DC, world, aetheryte, and coordinate movement into one seamless journey
- **Coordinate Movement** - Teleport instantly or smooth-move to any X/Y/Z coordinate
- **Aetheryte Teleportation** - Browse and teleport to any unlocked aetheryte with search
- **World Travel** - Visit other worlds on the same data center
- **Cross-DC Travel** - Travel to worlds on different data centers (requires Lifestream plugin)
- **Coordinate Bookmarks** - Save, load, and delete positions
- **Discord Bot Integration** - Interactive wizard to control everything remotely from Discord

## Plugin UI

The plugin window has 3 tabs:

| Tab | What It Does |
|-----|-------------|
| **Go To** | Quick coordinate input, world selector, aetheryte list, and live journey status |
| **Bookmarks** | Save/load/delete coordinate bookmarks |
| **Settings** | Movement speed, mount preference, Discord connection |

## Installation

### Plugin
1. In FFXIV, open the Dalamud plugin installer
2. Add the custom repository URL (see Releases)
3. Search for "MoveMeXiv" and install

### Discord Bot
1. Invite the bot to your private Discord server
2. Run `/setup` in Discord to get a pairing code
3. In-game: `/mmx` > Settings tab > enter pairing code

## In-Game Commands

| Command | Description |
|---------|-------------|
| `/mmx` | Open/close the plugin window |
| `/mmxgo <world\|x y z>` | Quick travel to a world or coordinates |

## Discord Commands

| Command | Description |
|---------|-------------|
| `/go` | Interactive destination picker wizard |
| `/go world:<name>` | Travel to a specific world |
| `/go x:<n> y:<n> z:<n>` | Move to coordinates |
| `/setup` | Generate a pairing code to link your plugin |
| `/status` | Show current character position, world, and state |
| `/bookmark save <name>` | Save current position as a bookmark |

## Requirements

- FFXIV with XIVLauncher and Dalamud
- .NET 8+ SDK (for building from source)
- Lifestream plugin (optional, for cross-DC travel)
