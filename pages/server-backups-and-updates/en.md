---
hytlMarkdown: 1
locale: "en"
title: "Server backups, updates and configuration"
slug: "server/backups-and-updates"
description: "Configure backup storage, understand the launcher update flow and edit server files without losing changes."
status: "complete"
sources:
  - url: "https://hytale.com/download"
    title: "Installed Hytale Server 0.7.2, release revision d769dc3d57881261a62858e1394f0e4de9a21eca"
    revision: "sha256:23f71f03763422ce7c04df191db49cd0e7d87d43b12baad75c43fdc202410aff"
    retrievedAt: "2026-10-15T15:24:02.400298+00:00"
    license: "Factual reference to locally installed Hytale server command definitions. Original game code is not redistributed."
    attribution: "Hypixel Studios; installed official release server JAR"
    modifications: "Read-only inspection of command registrations, argument types, bundled launchers and --help output. No server world was started. Evidence lists the inspected entries in provenance/server-guides-2026-10-15.json."
  - url: "https://support.hytale.com/hc/en-us/articles/45326769420827-Hytale-Server-Manual"
    title: "Hytale Server Manual"
    revision: "sha256:974be931fd6386fca693a0aa58083c8e0f406023e1dd788460735199058425f3"
    retrievedAt: "2026-10-15T15:24:02.116810+00:00"
    license: "Factual reference; copyright retained by Hypixel Studios. Original summary, no source prose or media reproduced."
    attribution: "Hypixel Studios / Hytale Team"
    modifications: "Independently written instructions; source checked on 15 October 2026."
---

Once :wiki[your server is running]{page="dedicated-server-setup"}, check its backup and restart path before players invest time in the world. These notes describe the **0.7.2** release command definitions and bundled launcher inspected on **15 October 2026**.

## Configure backups before requesting one

The bundled launcher supplies `--backup --backup-dir backups --backup-frequency 30`. Because it runs from `Server/`, this relative backup destination is **Server/backups/**. A direct Java launch needs its own backup arguments; the following example assumes the same directory layout:

```sh
java -jar HytaleServer.jar --assets ../Assets.zip --backup --backup-dir backups --backup-frequency 30
```

In the running console, enter `backup` and wait for the completion message. The inspected backup command refuses to start before boot finishes or when no backup directory is configured. A request being accepted is not evidence that the archive finished writing.

Keep another copy outside the server machine and test a restore in a separate directory. This is an operating recommendation: the existence of an archive alone does not prove that your recovery process works.

## Understand the directories

| Under Server/ | What to preserve or inspect |
| --- | --- |
| `universe/` | World and player saves. |
| `config.json` | Server settings. |
| `permissions.json` | Built-in permission settings. |
| `whitelist.json`, `bans.json` | Join restrictions. |
| `mods/` | Installed extensions; check compatibility before upgrades. |
| `logs/` | Startup and runtime diagnostics. |

Stop the server before manual configuration edits. Otherwise a later write from the running server can replace the file you just edited. Keep a known-good copy before changing values. Use :wiki[the command reference]{page="commands-and-permissions"} for supported runtime access-control commands.

## Use the launcher for updates

The expected structure has `Assets.zip` and `start.sh` or `start.bat` above `Server/`. Run the generated launcher from that parent directory. `update setup` can create the embedded launchers when the running server is in `Server/`.

Use this sequence in the **server console**, checking the result after each command:

```text
update status
update check
update download
```

After staging completes, notify players and verify your backup. Then deliberately apply it:

```text
update apply --confirm
```

:::callout{kind="warning" title="Applying an update stops the server"}
This is a maintenance action. The normal update path exits with code 8. The bundled launcher handles that code, installs the staged files and restarts. A plain Java process does not provide that wrapper restart.
:::

The bundled launchers restart for the update exit code; they are not a general crash supervisor. The updater's `WhenEmpty` and `Scheduled` application modes are optional configuration, not a promise that an arbitrary copied installation will update itself. Check your build's help and current configuration before enabling automatic application.

## After the restart

Read startup logs, check `update status`, join the world and verify saves, permissions and any mods you use. If an update fails, stop repeated restarts and inspect the logs and available backups before replacing files. Avoid a blind rollback over the only copy of your world.

The official manual documents the full update configuration and wrapper layout. This page's restore and post-update checks are recommendations; no live server update or recovery was performed to publish the article.

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
          "id": "dedicated-server-setup",
          "label": "Set up a Hytale server"
        }
      ]
    }
  ]
}
```
