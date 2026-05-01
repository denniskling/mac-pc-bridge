# SMB Mac ↔ Windows 11 – aktueller Stand

## Ziel

Rekordbox-Musikordner vom PC (`D:\Musik\Rekordbox`) über SMB auf dem Mac einbinden, damit Rekordbox auf dem Mac die MP3s vom PC abspielen/auflegen kann.

## Status
- SMB-Verbindung funktioniert ✓
- Ordner `Rekordbox` gemountet, Dateien sichtbar ✓
- Ordner liegt unter `/Volumes/Rekordbox` auf dem Mac

## Rekordbox einrichten

**Option A – Ordner zur Collection hinzufügen (empfohlen):**
1. Rekordbox öffnen
2. Linke Sidebar: Rechtsklick auf **Collection** → **Ordner zur Collection hinzufügen**
3. `/Volumes/Rekordbox` auswählen → Rekordbox scannt alle Tracks

**Option B – Musikordner-Pfad setzen:**
1. Rekordbox → Einstellungen (Zahnrad oben rechts)
2. **Erweitert** → **Musikordner** → auf `/Volumes/Rekordbox` setzen

## Wichtig
- Vor dem Auflegen sicherstellen, dass der SMB-Share gemountet ist (Finder → Netzwerk oder `Cmd+K`)
- Bei jedem Mac-Neustart muss die Verbindung neu hergestellt werden (außer du richtest Auto-Mount ein)
