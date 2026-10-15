---
hytlMarkdown: 1
locale: "en"
title: "Commands and permissions"
slug: "server/commands"
description: "Find command help, grant operator access, manage the whitelist and use common player and server commands. Checked against release 0.7.2."
status: "complete"
sources:
  - url: "https://hytale.com/download"
    title: "Installed Hytale Server 0.7.2, release revision d769dc3d57881261a62858e1394f0e4de9a21eca"
    revision: "sha256:23f71f03763422ce7c04df191db49cd0e7d87d43b12baad75c43fdc202410aff"
    retrievedAt: "2026-10-15T15:24:02.400298+00:00"
    license: "Factual reference to locally installed Hytale server command definitions. Original game code is not redistributed."
    attribution: "Hypixel Studios; installed official release server JAR"
    modifications: "Read-only inspection of command registrations, argument types, bundled launchers and --help output. No server world was started. Evidence lists the inspected entries in provenance/server-guides-2026-10-15.json."
  - url: "https://hytale.com/news/2026/5/update-5-patch-notes"
    title: "Update 5: command suggestions and permissions"
    revision: "sha256:cef62caaf06f4bd59ad44603fefb1a552468f49d4da1eaec9997f92f838bea71"
    retrievedAt: "2026-10-15T15:24:02.305780+00:00"
    license: "Factual reference; copyright retained by Hypixel Studios. Original summary, no source prose or media reproduced."
    attribution: "Hypixel Studios / Hytale Team"
    modifications: "Independently written instructions; source checked on 15 October 2026."
  - url: "https://support.hytale.com/hc/en-us/articles/45326769420827-Hytale-Server-Manual"
    title: "Hytale Server Manual"
    revision: "sha256:974be931fd6386fca693a0aa58083c8e0f406023e1dd788460735199058425f3"
    retrievedAt: "2026-10-15T15:24:02.116810+00:00"
    license: "Factual reference; copyright retained by Hypixel Studios. Original summary, no source prose or media reproduced."
    attribution: "Hypixel Studios / Hytale Team"
    modifications: "Independently written instructions; source checked on 15 October 2026."
---

These examples describe the built-in commands observed in **Hytale Server 0.7.2** on **15 October 2026**. Plugins and permissions can change what a player sees. Start with your running server's help before using an example from another version.

## Find the right command

Enter `/help` in chat. `/help give`, `/help op` and `/help whitelist` open help for those command families. The chat suggestion UI supports **Tab** to cycle suggestions and **Shift+Tab** to browse variants, as documented in the official Update 5 notes.

The tables use chat notation with a leading `/`. In the dedicated server terminal, use the command name without the slash. Shell commands such as `java --version` belong in PowerShell or a terminal, not in game chat. Replace angle-bracket placeholders; do not type the brackets.

:::callout{kind="warning" title="Operator access is administrative access"}
Only grant OP to trusted administrators. A missing permission is a reason to check the assigned role, rather than giving every player OP. Permission plugins can replace the built-in permission provider.
:::

## Operator access

| Command | Purpose and context |
| --- | --- |
| `/op add <player-uuid>` | Add that UUID to the built-in `hytale:Admin` group. Use the server console for the first administrator; copy the player's UUID accurately. |
| `/op remove <player-uuid>` | Remove that player's membership of the built-in admin group. |
| `/op self` | Toggle your own built-in OP membership where permitted. In singleplayer this checks that you own the world. Multiplayer has a self-OP startup gate; it is not a universal way to become admin on someone else's server. |

The inspected implementation also refuses `/op self` when another permission provider has replaced the built-in one. Follow that provider's instructions instead. For the first dedicated server, follow :wiki[Server setup]{page="dedicated-server-setup"}.

## Everyday reference

| Command | What to expect |
| --- | --- |
| `/help` | Discover commands available to your sender and permissions. |
| `/help <command>` | Read a command family's help before filling its arguments. |
| `/give Weapon_Sword_Iron` | Give the executing player the Iron Sword item; requires the corresponding permission and a player context. |
| `/gamemode Creative` | Set your own game mode to Creative with permission. |
| `/gamemode Adventure` | Set your own mode to the `Adventure` value observed in 0.7.2. Do not substitute `survival` or `exploration` from another game's guide. |
| `/kick <player>` | Disconnect a player; it does not itself add a ban. |
| `/whitelist status` | Inspect whether the whitelist is enabled. |
| `/whitelist list` | List whitelist entries. |
| `/whitelist add <player>` | Add a player through the profile lookup. Check the name and result. |
| `/whitelist remove <player>` | Remove a whitelist entry. |
| `/whitelist enable` | Restrict joining to the whitelist. Add your intended players first. |
| `/whitelist disable` | Disable that join restriction. |
| `/auth status` | Inspect server authentication in the dedicated console. |
| `/backup` | Request a universe backup once backup storage has been configured. Wait for completion. |
| `/stop` | Shut the server down normally. |

The Iron Sword ID links directly to :item[the item record]{id="Weapon_Sword_Iron"}. A display name with spaces is not interchangeable with an item ID. Use the item page's copy-ID control when building another `/give` command.

## If a command fails

Check spelling, sender context, permissions and the current build's help, in that order. A player-only command cannot acquire a player position or inventory from a plain server console. A command supplied by a plugin may disappear when that plugin is absent.

For startup, authentication and ports, see :wiki[Server setup]{page="dedicated-server-setup"}. For `/backup` and the update sequence, see :wiki[Backups and updates]{page="server-backups-and-updates"}.

```hytl:navbox
{
  "title": "Server guides",
  "groups": [
    {
      "title": "Read next",
      "links": [
        {
          "kind": "wiki",
          "id": "dedicated-server-setup",
          "label": "Set up a Hytale server"
        },
        {
          "kind": "wiki",
          "id": "server-backups-and-updates",
          "label": "Server backups, updates and configuration"
        }
      ]
    }
  ]
}
```
