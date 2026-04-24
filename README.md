# DMS Releases

Offizielle Download-Seite für die **DMS** App (Document Management System für Danwood-Vertrieb).

> **Sourcecode:** [Swifty-Chris/DMS](https://github.com/Swifty-Chris/DMS) (privat)

---

## Download

### macOS

**Minimum:** macOS 14.0 (Sonoma)

- Lade die neueste `.dmg` von der [**Releases**-Seite](https://github.com/Swifty-Chris/DMS-Releases/releases/latest)
- Doppelklick auf die `.dmg`, DMS nach `/Programme` ziehen
- Die App ist **signiert & bei Apple notarisiert** — kein Gatekeeper-Workaround nötig
- **Auto-Update:** Die App prüft automatisch auf neue Versionen via Sparkle. Manuell: `DMS → Nach Updates suchen…`

### iOS / iPadOS

**Minimum:** iOS/iPadOS 18.4

Die App wird per **Ad-Hoc Distribution** verteilt. Du brauchst:

1. **Deine UDID an Christian schicken** (einmalig).
   So findest du deine UDID:
   - iPhone/iPad per Kabel an den Mac
   - Finder öffnen → Gerät in der Seitenleiste wählen
   - Oben auf die Gerätebezeichnung klicken, bis die **UDID** erscheint → kopieren → per E-Mail schicken
2. Warte, bis du eine Bestätigung bekommst (Christian fügt deine UDID zum Profil hinzu und baut eine neue Version)
3. Öffne den Installations-Link (kommt per E-Mail) in **Safari** (nicht Chrome!)
4. Bestätige die Installation

**Auto-Update:** Die App zeigt dir in den Einstellungen, wenn eine neue Version verfügbar ist. Tippe auf den Link → Safari installiert die neue Version.

---

## Systemanforderungen

| Plattform | Minimum-Version |
|-----------|-----------------|
| macOS     | 14.0 (Sonoma)   |
| iOS       | 18.4            |
| iPadOS    | 18.4            |

---

## Privacy & Datenschutz

- [Datenschutz](https://danwood.nrw/datenschutz/)
- [Impressum](https://danwood.nrw/impressum/)

Verantwortlich: **cs-training UG (haftungsbeschraenkt)**, Lerchenweg 1, 21726 Oldendorf, Deutschland

---

## Updates verwalten (für Christian)

### macOS Appcast

Sparkle liest die Update-Informationen aus:

```
https://github.com/Swifty-Chris/DMS-Releases/raw/main/appcast.xml
```

### iOS Manifest

iOS installiert neue Versionen via OTA-Manifest:

```
https://github.com/Swifty-Chris/DMS-Releases/raw/main/manifest.plist
```

Diese beiden Dateien werden bei jedem Release automatisch durch die **GitHub Action im privaten DMS-Repo** aktualisiert (Tag `v*.*.*`).
