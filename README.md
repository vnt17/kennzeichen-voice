# Kennzeichen Voice

Android-App zum Sammeln von Kfz-Kennzeichen – per **Spracheingabe**, **Kamera-Scanner** oder Tippen.
Kompatibel mit Backups der App „Kennzeichensammler“ (Import und Export).

## Funktionen
- **Sprache mit Codewort:** Nur Sätze, die mit „Kennzeichen“ beginnen, werden ausgewertet („Kennzeichen Karlsruhe“, „Kennzeichen KA“). Alles andere wird ignoriert. Bestätigung per Ton und Sprachausgabe.
- **Kamera-Scanner:** liest Kennzeichen im Kamerabild (Texterkennung auf dem Gerät), Eintrag automatisch oder nach Rückfrage.
- 37 Länder, Fortschrittsanzeige, Rückgängig, Liste der letzten Funde.
- **Import/Export** des Kennzeichensammler-Backups sowie CSV-Liste.

## Installation
1. APK unter [Releases](../../releases/latest) herunterladen.
2. In den Android-Einstellungen „Installation aus unbekannten Quellen“ für den Browser/Dateimanager erlauben.
3. APK öffnen und installieren. Voraussetzung: Android 8 oder neuer, 64-Bit-ARM-Gerät (praktisch alle aktuellen Handys).

SHA-256 von `kennzeichen-voice-1.0.apk`: `a37dbb6d8f69b81bc210a5959566fc059b05c668c8f97dc76c5c85252249477e`

## Datenschutz
- Es gibt kein Konto, keine Werbung und keine Statistik. Deine Funde bleiben auf dem Gerät.
- Beim **ersten Start** lädt die App einmalig die Kennzeichen-Liste (`data.db`, ca. 1,5 MB) vom GitHub-Projekt [JPTK04/kennzeichen](https://github.com/JPTK04/kennzeichen). Danach funktioniert sie offline. Die Daten gehören dem jeweiligen Projekt und sind nicht Teil dieser App.
- Mikrofon: Die Spracherkennung übernimmt der Android-Spracherkenner deines Geräts. Je nach Gerät kann dieser Audio an seinen Anbieter (z. B. Google) senden.
- Kamera: Die Texterkennung (Google ML Kit) läuft auf dem Gerät.

## Hinweise
- Nicht während der Fahrt bedienen; der Scanner ist für Beifahrer oder Pausen gedacht.
- Inoffizielles Projekt, nicht mit der App „Kennzeichensammler“ verbunden.
