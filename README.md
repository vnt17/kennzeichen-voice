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

Die SHA-256-Prüfsumme jeder APK steht in den Hinweisen des jeweiligen Releases. Alle früheren Versionen bleiben verfügbar, siehe [Versionshistorie](CHANGELOG.md).

## Bedienung

### Spracheingabe
Mikrofon-Button antippen, dann läuft das Zuhören dauerhaft weiter (Display bleibt an). **Es wird nur ausgewertet, was mit dem Codewort „Kennzeichen“ beginnt**, alles andere wird ignoriert. Höchstens ein Wort davor ist erlaubt („okay Kennzeichen …“). Sagst du das Codewort mitten im Satz, zählt es nicht.

Zwei Arten:

| So sagst du es | Was passiert |
|---|---|
| „Kennzeichen Karlsruhe“ | Ton, Kennzeichen wird sofort eingetragen |
| „Kennzeichen“ … (Ton) … „Karlsruhe“ | Nach dem Ton hast du 8 Sekunden Zeit für das Kennzeichen |

**Was du nach dem Codewort sagen kannst**

- **Das Kürzel:** „KA“, „M“, „HH“ (gesprochen wie ausgesprochen: „Ka“, „Em“, „Ha Ha“).
- **Buchstabiert mit Buchstabennamen:** „Ka Be“ → KB, „Ha Ha“ → HH. Verstanden werden: a, be, ce/ze, de, e, ef, ge, ha, i, jot, ka, el, em, en, o, pe, ku, er, es, te, u, vau/fau, we, ix, ypsilon, zet/zett. Einzelne Laute wie „Ä“, „Ö“, „Ü“ sagst du als Buchstabe.
- **Buchstabiert mit der Buchstabiertafel:** „Anton Berta“ → AB. Anton, Berta, Cäsar, Dora, Emil, Friedrich, Gustav, Heinrich, Ida, Julius, Kaufmann, Ludwig, Martha, Nordpol, Otto, Paula, Quelle, Richard, Samuel, Theodor, Ulrich, Viktor, Wilhelm, Xanthippe, Ypsilon, Zacharias; für Umlaute Ärger, Ökonom, Übermut.
- **Buchstabiert mit dem NATO-Alphabet (englisch):** „Alpha Bravo“ → AB. Alfa/Alpha, Bravo, Charlie, Delta, Echo, Foxtrot, Golf, Hotel, India, Juliett, Kilo, Lima, Mike, November, Oscar, Papa, Quebec, Romeo, Sierra, Tango, Uniform, Victor, Whiskey, X-Ray, Yankee, Zulu. Auch eingedeutschte Schreibweisen des Erkenners (z. B. „Oskar“, „Maik“, „Tscharli“) werden akzeptiert.
- **Den Ort oder Kreis:** „Karlsruhe“, „München“, „Landkreis Karlsruhe“, „Stadt Pforzheim“. Vorangestellte Wörter wie Stadt, Landkreis, Kreis, Landeshauptstadt, Städteregion, Region, Regionalverband, Hansestadt, Freie, Powiat werden ignoriert.

**Anderes Land, ohne den Modus zu wechseln:** „Kennzeichen Polen WA“, „Kennzeichen Bulgarien CA“, „Kennzeichen Österreich W“ tragen das Kennzeichen direkt im genannten Land ein, auch wenn gerade Deutschland eingestellt ist. „Kennzeichen HH“ bleibt Hamburg. Nach dem Ländernamen kannst du Kürzel, Buchstabiertes (auch NATO) oder Orte sagen. Nur der Ländername allein („Kennzeichen Polen“) bewirkt nichts.

**Befehle** (ebenfalls mit „Kennzeichen“ davor)

| Sagen | Wirkung |
|---|---|
| „Kennzeichen rückgängig“ (auch: zurück, löschen, falsch, letzte löschen) | Entfernt den zuletzt hinzugefügten Eintrag |
| „Kennzeichen Land Polen“ | Wechselt das Land. Möglich sind alle Länder der Auswahlliste, z. B. Österreich, Schweiz, Frankreich, Italien, Tschechien, Großbritannien (auch: UK, England), Türkei, USA |
| „Kennzeichen Land Länder“ | Wechselt in die Liste der Länder selbst (ganzes Land eintragen, z. B. „Kennzeichen Polen“) |
| „Kennzeichen Stopp“ (auch: stop, ende, pause, aufhören) | Beendet das Zuhören |

**Rückmeldung:** Ein Ton zeigt, dass das Codewort gehört wurde. Mit dem Umschalter unter dem Mikrofon wählst du die Art der Rückmeldung:
- **🔊 Ausführlich:** Die App sagt z. B. „KA, Karlsruhe, neu“ oder „… schon gesehen“.
- **⚡ Schnell:** Keine Ansage, nur Töne: „ding-ding“ bei einem neuen Kennzeichen, „deet-deet“ bei schon gesehen oder nicht erkannt.

Ausführlich: Teilen sich mehrere Bezirke dasselbe Kürzel (z. B. L, ST, HZ), zählt jedes Schild für den nächsten Bezirk, der noch fehlt. Passt ein Name auf mehrere verschiedene Kürzel, sagt sie „Mehrdeutig“ und nennt Kandidaten. Dann sag das Kürzel direkt („Kennzeichen KA“). Wird nichts erkannt, trägt die App nichts ein und zeigt „Nicht erkannt“.

**Tipps**
- Ortsnamen, die deutsche Buchstabiertafel und das NATO-Alphabet werden zuverlässiger erkannt als einzelne Buchstaben. Du kannst die Alphabete auch mischen („Anton Bravo“).
- Spricht der Erkenner das Codewort falsch, hilft langsames, deutliches Sprechen. Gängige Varianten („Kenn Zeichen“, „Kennzeichnen“) werden akzeptiert.
- Ohne Internet funktioniert die Spracherkennung nur, wenn dein Gerät das deutsche Offline-Sprachpaket installiert hat.
- Falsch eingetragen? „Kennzeichen rückgängig“ oder den Eintrag in der Liste antippen und entfernen.

### Kamera-Scanner
Kamera-Symbol oben rechts. Halte das Kennzeichen ins Bild, die App liest den Text und sucht das Muster *Kürzel + Buchstaben + Ziffern* (z. B. „KA AB 123“).
- Ein Kennzeichen zählt erst, wenn es mehrfach hintereinander gelesen wurde. Halte die Kamera daher 1–2 Sekunden ruhig.
- **Auto** aus (Standard): Bei einem neuen Kennzeichen fragt die App „Hinzufügen?“. **Auto** an: Neue Kennzeichen werden sofort eingetragen (Vibration und Ton).
- Bereits gesammelte Kennzeichen zeigt die App nur kurz als „schon gesehen“ an. Dasselbe Kürzel wird danach 8 Sekunden lang ignoriert.
- Mit **1× / 2× / 4× / 8× / Max** oder mit zwei Fingern zoomst du heran. Der Rahmen bleibt dabei klein und gleich groß, nur das Bild wird größer.
- Plakette und blauer EU-Streifen stören nicht. Für gute Ergebnisse: genug Licht, Schild möglichst gerade und scharf, nicht zu weit weg.

### Dunkelmodus
Mit dem Mond-Symbol oben wird das Display schwarz und auf minimale Helligkeit gestellt, das Zuhören startet automatisch und läuft weiter. Alle Berührungen werden geschluckt, damit nichts versehentlich ausgelöst wird (z. B. in der Tasche oder Halterung). Zum Beenden **doppeltippen** oder die Zurück-Taste drücken. Ein einzelner Tipp blendet den Hinweis kurz ein. Schaltest du den Bildschirm mit der Ein-Taste aus, stoppt das Zuhören; der Dunkelmodus ersetzt das ausgeschaltete Display.

### Tippen
Über das Tastatur-Symbol kannst du ein Kürzel oder einen Ort eintippen. Hier ist **kein** Codewort nötig.

### Import und Export
Drei-Punkte-Menü oben rechts:
- **Backup importieren:** liest ein Backup der App „Kennzeichensammler“ ein. Vorhandene Einträge bleiben unverändert, nichts wird doppelt angelegt.
- **Backup exportieren:** erzeugt eine Backup-Datei mit allen alten und neuen Kennzeichen, die du in „Kennzeichensammler“ wieder einlesen kannst. Android hängt manchmal eine Endung wie `.bin` an, benenne die Datei dann um.
- **Liste exportieren (CSV):** Datum, Land, Kennzeichen, Ort und Region zum Öffnen in Excel o. Ä.
- **Info & Haftung:** zeigt den Haftungsausschluss.

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

Dieser Text steht auch in der App unter Menü → „Info & Haftung“, dort zusammen mit einer Kurzanleitung für die Sprache.
