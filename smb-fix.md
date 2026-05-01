# SMB Mac ↔ Windows 11 – aktueller Stand

## Status
- PC erreichbar (ping ok)
- SMB-Verbindung schlägt fehl: **Authentication error**

## Windows-Credentials

```
DESKTOP-RR8FK9G\dennis
```

Auf dem Mac verbinden mit:
```
smbutil view //dennis@192.168.178.36
```

## Falls Authentication weiter fehlschlägt

Microsoft-Konto macht oft Probleme. Fix: Lokalen Windows-User anlegen:
1. Einstellungen → Konten → Familie und andere Benutzer → Konto hinzufügen
2. "Ich kenne die Anmeldedaten nicht" → "Benutzer ohne Microsoft-Konto"
3. Lokalen User + Passwort erstellen
4. Ordner-Freigabe für diesen User erlauben (Rechtsklick Ordner → Eigenschaften → Freigabe)

## Wenn verbunden

Im Mac Finder: Gehe zu → Mit Server verbinden → `smb://192.168.178.36`
