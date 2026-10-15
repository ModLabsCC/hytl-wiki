---
hytlMarkdown: 1
locale: "de"
title: "Einen Hytale-Server einrichten"
slug: "server/setup"
description: "Freundeswelt oder dedizierter Server: Java und Dateien vorbereiten, Server starten, authentifizieren und die Verbindung einrichten."
status: "complete"
sourceLocale: "en"
sourceRevision: "ee07a87dd5a7d0d1cae20d8e500fad031124b5f043c7fcd31913f7e814f3df3e"
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

Ein dedizierter Server läuft unabhängig vom Spielclient. Für eine kurze Runde mit Freunden genügt eventuell eine freigegebene Einzelspielerwelt. Diese Anleitung wurde am **15. Oktober 2026** mit den offiziellen Support-Artikeln und den installierten **0.7.2**-Release-Dateien abgeglichen.

## Nur mit Freunden spielen?

Fügt euch zuerst als Hytale-Freunde hinzu. Öffne in deiner Welt **ESC → Online Play**, aktiviere **Allow Other Players to Join**, setze bei Bedarf ein Passwort und speichere. Dein Freund öffnet **Servers → Join via Code** und trägt den Code ein. Freigabecodes verraten Netzwerkadressen und können das Passwort enthalten: Teile sie privat. Nutze bei Problemen **Copy Network Report** und beachte den angezeigten Verbindungsstatus, bevor du Router-Einstellungen änderst.

## Dedizierte Installation vorbereiten

Offiziell erforderlich sind mindestens **Java 25** und **4 GB Arbeitsspeicher** auf x64 oder arm64. Das ist eine Mindestanforderung und keine Zusage für eine bestimmte Spielerzahl. Prüfe Java im vorgesehenen Terminal:

```sh
java --version
```

Nutze ein separates Serververzeichnis. Für eine vorhandene Windows-Installation öffnest du `%appdata%\Hytale\install\release\package\game\latest` und kopierst **Server/** zusammen mit **Assets.zip**. Beide müssen zum gleichen Release gehören. Den authentifizierten Downloader und weitere Betriebssysteme beschreibt das [offizielle Server-Handbuch](https://support.hytale.com/hc/en-us/articles/45326769420827-Hytale-Server-Manual).

## Starten und authentifizieren

Öffne bei diesem kopierten Aufbau ein Terminal **im kopierten Server-Verzeichnis**. Assets.zip liegt eine Ebene darüber:

```sh
java -jar HytaleServer.jar --assets ../Assets.zip --backup --backup-dir backups --backup-frequency 30
```

Die Pfade passen zu genau diesem Aufbau. Bei einer fehlenden JAR oder Assets-Datei prüfst du zuerst Arbeitsverzeichnis und Pfade. Die Startoptionen deiner Version kannst du ohne Weltstart mit `java -jar HytaleServer.jar --help` ansehen.

Authentifiziere dich anschließend **in der laufenden Serverkonsole**:

```text
auth login device
```

Öffne den offiziellen Autorisierungslink, den dein eigener Server ausgibt, und melde dich an. Prüfe danach `auth status`. Das geprüfte Release registriert den Zugangsdaten-Speicher `Encrypted`. Wähle ihn mit `auth persistence Encrypted`, kontrolliere das Ergebnis mit `auth persistence` und prüfe nach einem Neustart erneut `auth status`. Behandle erzeugte Zugangsdaten und Schlüsseldateien vertraulich.

## Den regulären Launcher einrichten

Während der Server aus `Server/` läuft, gibst du ein:

```text
update setup
stop
```

Warte das Herunterfahren ab. Starte dann im **übergeordneten Verzeichnis mit Assets.zip** den erzeugten Launcher:

| Plattform | Start im übergeordneten Verzeichnis |
| --- | --- |
| Windows PowerShell | `.\start.bat` |
| Linux- oder macOS-Shell | `./start.sh` |

Der mitgelieferte Launcher startet innerhalb von `Server/`, übergibt den passenden Assets-Pfad und aktiviert regelmäßige Backups. Er behandelt außerdem den Neustart-Code des Updaters. Lies vor dem ersten Update :wiki[Backups und Updates]{page="server-backups-and-updates"}.

## Die Verbindung erreichbar machen

Der dedizierte Standardport ist **5520/UDP**. Hytale verwendet QUIC über UDP. Erlaube diesen UDP-Port in der Host-Firewall und leite ihn bei Betrieb hinter einem Router an den Serverrechner weiter. Eine reine TCP-Regel reicht nicht.

Für einen anderen Port akzeptiert der direkte Java-Start `--bind 5521`. Verwende denselben UDP-Port in Firewall, Router und Client-Adresse. Ein Verbindungsversuch von außerhalb deines Heimnetzes prüft die Portweiterleitung sinnvoll.

Verbinde dich über die Serveroberfläche des Spiels mit Serveradresse und Port. Bei Fehlern prüfst du Prozess, `auth status`, `Server/logs/`, Port und Netzwerkregeln. Deaktiviere nicht als vermeintliche Netzwerk-Lösung die Authentifizierung.

## Administratoren und Beitritt verwalten

Richte den ersten vertrauenswürdigen Administrator in der dedizierten Konsole mit `op add <Spieler-UUID>` ein. Die :wiki[Befehlsreferenz]{page="commands-and-permissions"} erklärt OP, Spielerbefehle und Whitelist. Trage gewünschte Spieler ein, bevor du die Whitelist aktivierst.

Prüfe einen erfolgreichen Beitritt und danach einen vollständigen Neustart über den Launcher. Welt und Einstellungen sollen erhalten bleiben und Backups erfolgreich abschließen. Das sind Abnahmeschritte für deine Installation; Router und Hosting-Panels können sich unterscheiden.

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
          "id": "server-backups-and-updates",
          "label": "Server-Backups, Updates und Konfiguration"
        }
      ]
    }
  ]
}
```
