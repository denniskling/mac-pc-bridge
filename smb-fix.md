# SMB Mac ↔ Windows 11 – ABGESCHLOSSEN ✓

## Setup
- PC: `DESKTOP-RR8FK9G`, User `dennis`, IP `192.168.178.36`
- Freigabe: `D:\Musik\Rekordbox` → Freigabename `Rekordbox`
- Mac verbinden: Finder → `Cmd+K` → `smb://dennis@192.168.178.36/Rekordbox`
- Gemountet unter: `/Volumes/Rekordbox`

## Rekordbox
- Collection → Ordner hinzufügen → `/Volumes/Rekordbox`
- Tracks analysieren: alle markieren → Rechtsklick → Analysieren (BPM, Key, Waveform)
- Auto-Analyse: Einstellungen → Analyse → automatisch aktivieren

## Wichtig
- SMB-Share muss vor Rekordbox gemountet sein
- Bei Mac-Neustart erneut verbinden (`Cmd+K`)
