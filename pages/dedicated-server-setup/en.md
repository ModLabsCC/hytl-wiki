---
hytlMarkdown: 1
locale: "en"
title: "Set up a Hytale server"
slug: "server/setup"
description: "Choose friend-hosted play or a dedicated server, prepare Java and server files, authenticate, and configure the connection."
status: "complete"
sources:
  - url: "https://support.hytale.com/hc/en-us/articles/45326769420827-Hytale-Server-Manual"
    title: "Hytale Server Manual"
    revision: "sha256:974be931fd6386fca693a0aa58083c8e0f406023e1dd788460735199058425f3"
    retrievedAt: "2026-10-15T15:24:02.116810+00:00"
    license: "Factual reference; copyright retained by Hypixel Studios. Original summary, no source prose or media reproduced."
    attribution: "Hypixel Studios / Hytale Team"
    modifications: "Independently written instructions; source checked on 15 October 2026."
  - url: "https://support.hytale.com/hc/en-us/articles/45324238811291-Joining-Friends"
    title: "Joining Friends"
    revision: "sha256:8336c7a956f84fffe58b7396f14c3e61a573680a27ebdf2c5768e28b6dcddb21"
    retrievedAt: "2026-10-15T15:24:02.214875+00:00"
    license: "Factual reference; copyright retained by Hypixel Studios. Original summary, no source prose or media reproduced."
    attribution: "Hypixel Studios / Hytale Team"
    modifications: "Independently written instructions; source checked on 15 October 2026."
  - url: "https://hytale.com/download"
    title: "Installed Hytale Server 0.7.2, release revision d769dc3d57881261a62858e1394f0e4de9a21eca"
    revision: "sha256:23f71f03763422ce7c04df191db49cd0e7d87d43b12baad75c43fdc202410aff"
    retrievedAt: "2026-10-15T15:24:02.400298+00:00"
    license: "Factual reference to locally installed Hytale server command definitions. Original game code is not redistributed."
    attribution: "Hypixel Studios; installed official release server JAR"
    modifications: "Read-only inspection of command registrations, argument types, bundled launchers and --help output. No server world was started. Evidence lists the inspected entries in provenance/server-guides-2026-10-15.json."
---

A dedicated server runs independently of your game client. For a short session with friends, opening a singleplayer world may be enough. This guide was checked on **15 October 2026** against the official support articles and the installed **0.7.2** release files.

## Just playing with friends?

Add each other as Hytale friends first. In your world, open **ESC → Online Play**, enable **Allow Other Players to Join**, optionally set a password, then save. Your friend uses **Servers → Join via Code** and enters your code. Share codes reveal network addresses and can contain the password: send them privately. Use **Copy Network Report** when troubleshooting, and follow the connection result shown by the game before changing router settings.

## Prepare a dedicated installation

The official minimum is **Java 25** and **4 GB memory**, on x64 or arm64. This is a starting requirement, not a player-capacity guarantee. Check Java in the terminal you will use:

```sh
java --version
```

Use a separate server directory. To copy an existing Windows installation, open `%appdata%\Hytale\install\release\package\game\latest` and copy **Server/** and **Assets.zip** together. Keep the two from the same release. For the authenticated downloader and other operating systems, follow the [official Server Manual](https://support.hytale.com/hc/en-us/articles/45326769420827-Hytale-Server-Manual).

## Start and authenticate

For the copied layout, open a terminal **inside the copied Server directory**. The assets are one directory above it:

```sh
java -jar HytaleServer.jar --assets ../Assets.zip --backup --backup-dir backups --backup-frequency 30
```

This command intentionally uses paths matching that layout. A missing JAR or assets error usually means the working directory or path differs. To inspect the installed build's flags without starting a world, run `java -jar HytaleServer.jar --help`.

In the **running server console**, authenticate:

```text
auth login device
```

Open the official device-authorization link printed by your own server and complete the account login. Then check `auth status`. The inspected release registers the `Encrypted` credential store. Select it with `auth persistence Encrypted`, inspect the result with `auth persistence`, and verify `auth status` again after a restart. Keep generated credential and key files private.

## Install the normal launcher

With the server running from `Server/`, enter:

```text
update setup
stop
```

Wait for shutdown. From the **parent directory containing Assets.zip**, use the generated launcher:

| Platform | Start from the parent directory |
| --- | --- |
| Windows PowerShell | `.\start.bat` |
| Linux or macOS shell | `./start.sh` |

The bundled launcher starts inside `Server/`, supplies the parent assets path and enables periodic backups. It also handles the update restart exit code. See :wiki[Backups and updates]{page="server-backups-and-updates"} before your first upgrade.

## Make the connection reachable

The default dedicated port is **5520/UDP**. Hytale uses QUIC over UDP. Allow that UDP port in the host firewall; if hosting behind a router, forward it to the server machine. A TCP-only rule does not serve this connection.

For another port, the direct Java command accepts `--bind 5521`; use that same UDP port consistently in firewall, router and client address. A connection from outside your home is the useful acceptance test for a router forward.

Join through the game's server interface using your server address and port. If joining fails, check the process, `auth status`, `Server/logs/`, the selected port and network rules. Do not turn off authenticated mode as a shortcut for a network error.

## Add administrators and limit joining

Use the dedicated console to grant the first trusted administrator access with `op add <player-uuid>`. The :wiki[command reference]{page="commands-and-permissions"} explains OP, player context and whitelist commands. Add your intended players before enabling the whitelist.

Confirm a successful join, then shut down and restart through the launcher. Check that the world and settings remain available and that backups complete. These are your installation checks; this article does not claim that every router or hosting panel behaves identically.

```hytl:navbox
{
  "title": "Server guides",
  "groups": [
    {
      "title": "Read next",
      "links": [
        {
          "kind": "wiki",
          "id": "commands-and-permissions",
          "label": "Commands and permissions"
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
