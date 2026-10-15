---
hytlMarkdown: 1
locale: "de"
title: "Befehle und Berechtigungen"
slug: "server/commands"
description: "Befehlshilfe, Operator-Rechte, Whitelist und häufige Spieler- und Serverbefehle. Mit Release 0.7.2 abgeglichen."
status: "complete"
sourceLocale: "en"
sourceRevision: "85bcc1b80fb125337f0f8cb4bd934b614bab42c31185501f1f87d7662e4b793a"
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

Die Beispiele beschreiben eingebaute Befehle aus **Hytale Server 0.7.2**, geprüft am **15. Oktober 2026**. Plugins und Berechtigungen können verändern, welche Befehle ein Spieler sieht. Prüfe bei abweichenden Versionen zuerst die Hilfe deines laufenden Servers.

## Den passenden Befehl finden

Gib im Chat `/help` ein. `/help give`, `/help op` und `/help whitelist` öffnen die Hilfe der jeweiligen Befehlsfamilie. Laut den offiziellen Update-5-Notizen blätterst du mit **Tab** durch Chat-Vorschläge und mit **Shift+Tab** durch Varianten.

Die Tabellen zeigen Chat-Befehle mit `/`. Im Terminal des dedizierten Servers verwendest du den Namen ohne Schrägstrich. Shell-Befehle wie `java --version` gehören in PowerShell beziehungsweise ein Terminal. Ersetze Platzhalter in spitzen Klammern; die Klammern werden nicht mit eingegeben.

:::callout{kind="warning" title="OP bedeutet administrative Rechte"}
Vergib OP nur an vertrauenswürdige Administratoren. Prüfe bei fehlenden Rechten die zugewiesene Rolle, statt allen Spielern OP zu geben. Berechtigungsplugins können den eingebauten Anbieter ersetzen.
:::

## Operator-Rechte

| Befehl | Zweck und Kontext |
| --- | --- |
| `/op add <Spieler-UUID>` | Fügt die UUID zur eingebauten Gruppe `hytale:Admin` hinzu. Richte den ersten Administrator über die Serverkonsole ein und übernimm die UUID korrekt. |
| `/op remove <Spieler-UUID>` | Entfernt die Mitgliedschaft in der eingebauten Administratorgruppe. |
| `/op self` | Schaltet die eigenen eingebauten OP-Rechte um, soweit erlaubt. Im Einzelspieler wird der Weltbesitzer geprüft. Im Mehrspieler gibt es eine Startoption für Selbst-OP; der Befehl verschafft dir nicht allgemein Adminrechte auf fremden Servern. |

Die geprüfte Implementierung verweigert `/op self` außerdem, wenn ein anderer Berechtigungsanbieter den eingebauten ersetzt hat. Nutze dann dessen Anleitung. Für deinen ersten dedizierten Server hilft :wiki[Server einrichten]{page="dedicated-server-setup"}.

## Häufige Befehle

| Befehl | Wirkung |
| --- | --- |
| `/help` | Zeigt die für den Absender und seine Rechte verfügbaren Befehle. |
| `/help <Befehl>` | Öffnet die Hilfe einer Befehlsfamilie. |
| `/give Weapon_Sword_Iron` | Gibt dem ausführenden Spieler das Eisenschwert; benötigt passende Rechte und einen Spieler als Absender. |
| `/gamemode Creative` | Wechselt den eigenen Spielmodus mit Berechtigung zu Creative. |
| `/gamemode Adventure` | Verwendet den in 0.7.2 erfassten Moduswert `Adventure`. Ersetze ihn nicht durch `survival` oder `exploration` aus anderen Anleitungen. |
| `/kick <Spieler>` | Trennt einen Spieler vom Server, ohne dadurch einen Bann einzutragen. |
| `/whitelist status` | Zeigt, ob die Whitelist aktiv ist. |
| `/whitelist list` | Listet die Whitelist-Einträge auf. |
| `/whitelist add <Spieler>` | Fügt einen Spieler über die Profilsuche hinzu. Prüfe Name und Ergebnis. |
| `/whitelist remove <Spieler>` | Entfernt einen Whitelist-Eintrag. |
| `/whitelist enable` | Beschränkt den Beitritt auf die Whitelist. Trage die gewünschten Spieler vorher ein. |
| `/whitelist disable` | Deaktiviert diese Beitrittsbeschränkung. |
| `/auth status` | Prüft die Server-Authentifizierung in der dedizierten Konsole. |
| `/backup` | Fordert ein Welt-Backup an, wenn ein Backup-Ziel eingerichtet wurde. Warte auf den Abschluss. |
| `/stop` | Fährt den Server regulär herunter. |

Die Schwert-ID führt direkt zum :item[Item-Eintrag]{id="Weapon_Sword_Iron"}. Anzeigename und Item-ID sind unterschiedliche Dinge. Verwende für weitere `/give`-Befehle die Funktion zum Kopieren der ID auf der Item-Seite.

## Wenn ein Befehl fehlschlägt

Prüfe Schreibweise, Absender, Rechte und die Hilfe deiner Version. Ein Spielerbefehl erhält aus einer reinen Serverkonsole keine Spielerposition und kein Inventar. Plugin-Befehle können fehlen, sobald das zugehörige Plugin nicht installiert ist.

Start, Authentifizierung und Ports erklärt :wiki[Server einrichten]{page="dedicated-server-setup"}. Die Schritte für `/backup` und Updates stehen unter :wiki[Backups und Updates]{page="server-backups-and-updates"}.

```hytl:navbox
{
  "title": "Server-Guides",
  "groups": [
    {
      "title": "Weiterlesen",
      "links": [
        {
          "kind": "wiki",
          "id": "dedicated-server-setup",
          "label": "Einen Hytale-Server einrichten"
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
