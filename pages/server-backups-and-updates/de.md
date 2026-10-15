---
hytlMarkdown: 1
locale: "de"
title: "Server-Backups, Updates und Konfiguration"
slug: "server/backups-and-updates"
description: "Backup-Ziel einrichten, den Update-Ablauf mit Launcher verstehen und Konfigurationsdateien sicher bearbeiten."
status: "complete"
sourceLocale: "en"
sourceRevision: "966dba93c632474bfba9946e2aa44ed7444d1b9961abbbdb37986c0acb70c79f"
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

Prüfe nach der :wiki[Server-Einrichtung]{page="dedicated-server-setup"} Backups und Neustarts, bevor Spieler viel Zeit in die Welt stecken. Diese Hinweise beruhen auf den Befehlsdefinitionen und dem mitgelieferten Launcher von **Release 0.7.2**, geprüft am **15. Oktober 2026**.

## Backups vor der ersten Sicherung konfigurieren

Der mitgelieferte Launcher übergibt `--backup --backup-dir backups --backup-frequency 30`. Da er aus `Server/` startet, ist das relative Ziel **Server/backups/**. Ein direkter Java-Start benötigt eigene Backup-Argumente. Dieses Beispiel setzt denselben Verzeichnisaufbau voraus:

```sh
java -jar HytaleServer.jar --assets ../Assets.zip --backup --backup-dir backups --backup-frequency 30
```

Gib in der laufenden Konsole `backup` ein und warte auf die Abschlussmeldung. Der geprüfte Backup-Befehl verweigert den Start vor Ende des Bootvorgangs oder ohne konfiguriertes Backup-Verzeichnis. Die Annahme des Befehls beweist noch keinen fertig geschriebenen Sicherungsstand.

Bewahre eine weitere Kopie außerhalb des Serverrechners auf und teste die Wiederherstellung in einem separaten Verzeichnis. Das ist eine Betriebsempfehlung: Eine vorhandene Archivdatei beweist allein noch keinen funktionierenden Wiederherstellungsablauf.

## Verzeichnisse verstehen

| Unter Server/ | Was du sichern oder prüfen solltest |
| --- | --- |
| `universe/` | Welt- und Spielerdaten. |
| `config.json` | Servereinstellungen. |
| `permissions.json` | Eingebaute Berechtigungseinstellungen. |
| `whitelist.json`, `bans.json` | Beitrittsbeschränkungen. |
| `mods/` | Erweiterungen; Kompatibilität vor Updates prüfen. |
| `logs/` | Diagnose für Start und laufenden Betrieb. |

Stoppe den Server vor manuellen Konfigurationsänderungen. Ein späterer Schreibvorgang des laufenden Servers könnte sonst deine Änderung überschreiben. Behalte vor Änderungen eine funktionierende Kopie. Unterstützte Befehle für laufende Zugriffsverwaltung findest du in der :wiki[Befehlsreferenz]{page="commands-and-permissions"}.

## Updates über den Launcher ausführen

Beim vorgesehenen Aufbau liegen `Assets.zip` und `start.sh` beziehungsweise `start.bat` über `Server/`. Führe den erzeugten Launcher aus diesem übergeordneten Verzeichnis aus. Mit `update setup` kann der laufende Server in `Server/` die eingebetteten Startskripte erzeugen.

Nutze in der **Serverkonsole** diese Reihenfolge und prüfe nach jedem Schritt das Ergebnis:

```text
update status
update check
update download
```

Wenn die Bereitstellung abgeschlossen ist, informiere Spieler und prüfe dein Backup. Wende das Update anschließend bewusst an:

```text
update apply --confirm
```

:::callout{kind="warning" title="Das Anwenden beendet den laufenden Server"}
Dies ist ein Wartungsschritt. Der reguläre Update-Pfad beendet sich mit Code 8. Der mitgelieferte Launcher behandelt diesen Code, installiert die bereitgestellten Dateien und startet neu. Ein einzelner Java-Prozess übernimmt diesen Wrapper-Neustart nicht.
:::

Die mitgelieferten Launcher starten für den Update-Code neu; sie sind keine allgemeine Absturzüberwachung. `WhenEmpty` und `Scheduled` sind optionale Anwendungsmodi des Updaters und keine Zusage für automatische Updates jeder kopierten Installation. Prüfe Hilfe und Konfiguration deiner Version, bevor du das automatische Anwenden aktivierst.

## Nach dem Neustart

Lies die Startlogs, prüfe `update status`, betrete die Welt und kontrolliere Speicherstände, Rechte und eingesetzte Mods. Stoppe bei Fehlern wiederholte Neustarts und prüfe Logs und Backups, bevor du Dateien ersetzt. Überschreibe beim Zurücksetzen nicht ungeprüft die einzige Kopie deiner Welt.

Das offizielle Handbuch beschreibt die vollständige Update-Konfiguration und den Wrapper-Aufbau. Wiederherstellungs- und Abnahmeprüfungen auf dieser Seite sind Empfehlungen; für die Veröffentlichung wurde kein laufender Spielserver aktualisiert oder wiederhergestellt.

```hytl:navbox
{
  "title": "Server-Guides",
  "groups": [
    {
      "title": "Weiterlesen",
      "links": [
        {
          "kind": "wiki",
          "id": "commands-and-permissions",
          "label": "Befehle und Berechtigungen"
        },
        {
          "kind": "wiki",
          "id": "dedicated-server-setup",
          "label": "Einen Hytale-Server einrichten"
        }
      ]
    }
  ]
}
```
