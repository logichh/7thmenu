# 7thMenu

7thMenu is a Paper plugin that gives players one central menu for travel, social tools, store access, and onboarding. It is built for Java + Bedrock mixed servers and is configurable through `config.yml`.

## What A Buyer Gets

- One `/menu` hub for common server actions.
- Java inventory UI plus Bedrock form/chat UI support.
- Built-in RTP, starter kit, MenuStar item, and blocking system.
- Optional integrations with Essentials, Towny, Floodgate, Geyser, and Cumulus.
- Config-driven buttons, labels, commands, lore, and messages.

## Feature Systems

### 1) Menu Hub System
- Main menu with configurable size, filler, title, and item actions.
- Buttons for shop, towny, auction, rtp, store, teleport, world expansion, war, skills, spawn, homes, tpa, friends, trade, and more.
- Submenus included: Teleport, TPA, Friends, Blocking, Store, Towny, Town Spawns, Worlds, Teleport Guide, and Store Guide.

### 2) MenuStar System
- `/menustar` gives a tagged custom nether star that opens the menu on right-click.
- Optional first-join auto-give.
- Protection layer prevents star abuse (dropping, crafting, moving into restricted inventories, and pickup duplication cases).

### 3) Starter Kit System
- One-time `/starterkit` claim with saved claim tracking.
- Optional auto-grant on first join (`give-starterkit-on-join`).
- Admin grant command: `/starterkitgive <player>`.
- Inventory-space validation to prevent item loss.

### 4) RTP System
- `/rtp` command and menu action.
- Per-world RTP regions (circle or cuboid), safe-location search, and world-border buffer support.
- Optional cooldown, warmup, cancel-on-move, Towny wilderness-only mode, and post-teleport invulnerability.

### 5) Teleport And Homes System
- Spawn teleport with safety checks.
- Homes list with teleport/delete flows and set-home shortcut.
- TPA request/accept/deny flow from menu.
- World and hub teleport shortcuts.

### 6) Friends And Blocking System
- Friends menu shortcuts for add/list/remove command workflows.
- Built-in block/unblock/list UI.
- Blocked players are prevented from messaging, TPA, and direct teleport commands.
- Block data persists in `blocked.yml`.

### 7) Store Menu System
- Store submenu with open/ranks/holiday/cosmetics/help actions.
- Optional Bedrock clickable store URL on menu use.

### 8) Towny System
- Towny submenu and town spawn shortcuts.
- Public town list + teleport flow.
- RTP can avoid claimed land by requiring wilderness when Towny is available.

### 9) Bedrock Support System
- Detects Bedrock players through Floodgate.
- Uses Cumulus forms when available (`bedrock.use-forms`).
- Falls back to chat-rendered menus if forms are unavailable.

## Commands

- `/menu [action]`
- `/menustar`
- `/rtp`
- `/starterkit`
- `/starterkitgive <player>`

## Permissions

- `7thmenu.use`
- `7thmenu.menustar`
- `7thmenu.rtp`
- `7thmenu.starterkit`
- `7thmenu.starterkit.admin`
