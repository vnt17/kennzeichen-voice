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

SHA-256 von `kennzeichen-voice-1.1.apk`: `e4e07764c75f91fe1ee18c4ca23d664ff9a951a6a2dfc10e50079e48b784b47d`

## Datenschutz
- Es gibt kein Konto, keine Werbung und keine Statistik. Deine Funde bleiben auf dem Gerät.
- Beim **ersten Start** lädt die App einmalig die Kennzeichen-Liste (`data.db`, ca. 1,5 MB) vom GitHub-Projekt [JPTK04/kennzeichen](https://github.com/JPTK04/kennzeichen). Danach funktioniert sie offline. Die Daten gehören dem jeweiligen Projekt und sind nicht Teil dieser App.
- Mikrofon: Die Spracherkennung übernimmt der Android-Spracherkenner deines Geräts. Je nach Gerät kann dieser Audio an seinen Anbieter (z. B. Google) senden.
- Kamera: Die Texterkennung (Google ML Kit) läuft auf dem Gerät. Der beim Scannen gelesene Kennzeichen-Text wird nur lokal im Verlauf der App gespeichert.

## Haftungsausschluss

Diese App wurde mit besten Absichten und nach bestem Wissen erstellt. Sie wird unentgeltlich und ohne jede Gewähr zur Verfügung gestellt. Es wird nicht zugesichert, dass sie fehlerfrei, vollständig, jederzeit verfügbar oder für einen bestimmten Zweck geeignet ist. Das gilt insbesondere für die Spracherkennung, die Texterkennung der Kamera und die Kennzeichen-Daten, die Fehler enthalten können.

Die Nutzung erfolgt auf eigene Gefahr. Für Schäden jeder Art, die aus der Nutzung oder Nichtnutzung der App entstehen – etwa Datenverlust, falsche Einträge, beschädigte oder nicht importierbare Backup-Dateien oder Unfälle durch Ablenkung im Straßenverkehr –, wird keine Haftung übernommen, soweit dies gesetzlich zulässig ist. Unberührt bleibt die Haftung für Vorsatz und grobe Fahrlässigkeit sowie für Schäden aus der Verletzung von Leben, Körper oder Gesundheit.

**Straßenverkehr:** Bediene die App nur, wenn weder du noch andere dadurch gefährdet werden. Als Fahrer gilt deine volle Aufmerksamkeit dem Verkehr. Den Kamera-Scanner nutzt du nur als Beifahrer oder im Stand.

**Deine Daten:** Erstelle regelmäßig Sicherungen deiner Sammlung (Menü → Backup exportieren). Bevor du ein von dieser App erzeugtes Backup in eine andere App einliest, sichere deren bestehende Daten.

**Datenquelle und Dritte:** Die Kennzeichen-Liste stammt aus dem GitHub-Projekt [JPTK04/kennzeichen](https://github.com/JPTK04/kennzeichen) und gehört dem jeweiligen Urheber; ihre Richtigkeit wurde nicht geprüft. Diese App ist ein inoffizielles Projekt und nicht mit der App „Kennzeichensammler“ verbunden.

**Datenschutz beim Fotografieren und Notieren:** Kfz-Kennzeichen können personenbezogene Daten sein. Nutze die App nur im Rahmen der geltenden Gesetze und veröffentliche keine Kennzeichen oder Standortdaten anderer Personen.

Dieser Text steht auch in der App unter Menü → „Info & Haftung“.
