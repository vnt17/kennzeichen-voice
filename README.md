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

### Parkplatzmodus
Der Knopf **🅿 Parkplatz** unter dem Mikrofon startet das Zuhören **ohne Codewort**: Du sagst direkt das Kennzeichen, z. B. „WI“ oder „Polen WGM“, und es wird sofort gewertet. „Kennzeichen“ davor ist erlaubt, aber nicht nötig. Rückgängig, Land wechseln und Stopp funktionieren wie sonst. Ein weiterer Tipp auf den Knopf beendet den Modus. Achtung: Es wird alles Gesagte ausgewertet, also nur dort nutzen, wo sonst niemand redet.

### Sammler-Backup in Drive aktualisieren

> **⚠ Keine Garantie.** Diese Funktion hat bei Tests funktioniert. Trotzdem kann für Datenverlust **absolut keine Garantie** gegeben werden: weder in Kennzeichen Voice noch in der Kennzeichensammler-App noch in deinem Google Drive. Lege vorher eigene Sicherungen an und prüfe das Ergebnis. Nutzung auf eigene Gefahr.

**Wozu?** Die Kennzeichensammler-App fragt Google Drive über die Drive-API ab, aber nur mit dem Berechtigungsumfang `drive.file`. Damit sieht sie ausschließlich Dateien, die sie **selbst** angelegt hat. Ein Backup aus Kennzeichen Voice, das du von Hand in Drive legst, findet sie nicht, auch wenn der Name `KennzeichensammlerBackupX-…` stimmt.

**Wie funktioniert es?** Kennzeichen Voice legt keine neue Datei an, sondern schreibt den Inhalt einer bereits von der Sammler-App angelegten Datei neu. Sie bleibt dieselbe Drive-Datei und damit weiterhin eine Datei der Sammler-App.
1. In der Sammler-App einmal ein Backup anlegen (dort „Backup / Wiederherstellen“). Es liegt danach in Drive unter **Meine Ablage** und heißt `KennzeichensammlerBackupX-TT.MM.JJJJ`.
2. In Kennzeichen Voice: Menü ⋮ → **„Sammler-Backup in Drive aktualisieren …“**. Im Dateiauswahldialog über ☰ → **Drive** → **Meine Ablage** (oder über die Suche) genau diese Datei wählen. Die Auswahl merkt sich die App, beim nächsten Mal reicht ein Tipp.
3. Die App liest die Datei und prüft, ob sie ein Sammler-Backup ist. Der Dialog zeigt, wie viele Einträge sie enthält, wie viele in Kennzeichen Voice fehlen und wie viele Kennzeichen Voice selbst hat. Fehlende Einträge werden auf Wunsch (Häkchen, standardmäßig an) vorher in Kennzeichen Voice übernommen, damit nichts verloren geht.
4. **Überschreiben:** Zuerst speichert die App eine **Kopie des alten Inhalts** in `Downloads/Drive-Backup-Sicherung-<Datum>-<Zeit>.bak`. Dann erzeugt sie aus deiner ganzen Sammlung ein Backup im Format der Sammler-App (zlib-komprimiert, Kennung `KX1`, darin eine SQLite-Datenbank) und schreibt es über die Drive-App in die gewählte Datei.
5. **Gegenprobe:** Die App liest die Datei wieder ein und vergleicht die Anzahl der Einträge. Stimmt sie nicht oder tritt ein Fehler auf, versucht sie, den alten Inhalt zurückzuschreiben, und meldet das.
6. Die Drive-App lädt die Änderung im Hintergrund hoch. Danach kann die Sammler-App die Datei über „Wiederherstellen aus Google Drive“ lesen.

**Voraussetzungen:** Drive-App installiert und angemeldet, Internet für das Hochladen, die Datei der Sammler-App liegt in deinem Drive.

**Warum es trotzdem schiefgehen kann**
- Das Dateiformat der Sammler-App ist nicht offiziell dokumentiert (aus Backups abgeleitet). Ein Update der Sammler-App kann es ändern.
- Beim Schreiben oder Hochladen können Fehler passieren (Verbindungsabbruch, Drive-Synchronisation, Speicherplatz). Die Gegenprobe prüft nur die lokale Sicht der Drive-App, nicht, ob der Upload fertig ist.
- Wählst du die falsche Datei, wird sie überschrieben. Der alte Inhalt liegt dann nur in der Kopie in Downloads.
- Eine Wiederherstellung in der Sammler-App kann deren Daten verändern oder überschreiben.

**Was du vorher tun solltest:** Menü → **Backup exportieren** und die Datei an einem zweiten Ort aufbewahren, in der Sammler-App ebenfalls ein Backup anlegen, die Kopie in Downloads erst löschen, wenn alles stimmt.

### Kamera-Scanner
Kamera-Symbol oben rechts. Halte das Kennzeichen ins Bild, die App liest den Text und sucht das Muster *Kürzel + Buchstaben + Ziffern* (z. B. „KA AB 123“).
- Ein Kennzeichen zählt erst, wenn es mehrfach hintereinander gelesen wurde. Halte die Kamera daher 1–2 Sekunden ruhig.
- **Auto** aus (Standard): Bei einem neuen Kennzeichen fragt die App „Hinzufügen?“. **Auto** an: Neue Kennzeichen werden sofort eingetragen (Vibration und Ton).
- Bereits gesammelte Kennzeichen zeigt die App nur kurz als „schon gesehen“ an. Dasselbe Kürzel wird danach 8 Sekunden lang ignoriert.
- Mit **1× / 2× / 4× / 8× / Max** oder mit zwei Fingern zoomst du heran. Der Rahmen bleibt dabei klein und gleich groß, nur das Bild wird größer.
- Plakette und blauer EU-Streifen stören nicht. Für gute Ergebnisse: genug Licht, Schild möglichst gerade und scharf, nicht zu weit weg.

### Dunkelmodus
Mit dem Mond-Symbol oben wird das Display schwarz und auf minimale Helligkeit gestellt, das Zuhören startet automatisch und läuft weiter. Alle Berührungen werden geschluckt, damit nichts versehentlich ausgelöst wird (z. B. in der Tasche oder Halterung). Status- und Navigationsleiste werden ausgeblendet und die Helligkeit auf das Minimum gestellt; beim ersten Mal zeigt Android dazu eine eigene Vollbild-Meldung, die du mit „Verstanden“ bestätigst. Zum Beenden **doppeltippen** oder die Zurück-Taste drücken. Ein einzelner Tipp blendet den Hinweis kurz ein. Schaltest du den Bildschirm mit der Ein-Taste aus, stoppt das Zuhören; der Dunkelmodus ersetzt das ausgeschaltete Display.

### Android Auto (Beta)
Die Funktion ist neu und noch wenig getestet. Es gibt zwei Wege:

**1. Eigene App im Auto-Launcher (großer Knopf)**
1. Einmalig auf dem Handy: **Android Auto** öffnen → Einstellungen → die **Versionsnummer 10-mal antippen** → Entwickleroptionen → **„Unbekannte Quellen“** einschalten. Das ist nötig, weil die App nicht aus dem Play Store kommt und Android Auto dafür keine passende Kategorie hat (die App meldet sich als „Orte“-App an).
2. Handy neu mit dem Auto verbinden, im Launcher **„Kennzeichen“** öffnen.
3. Auf **Kennzeichen sagen** tippen und das Kennzeichen sprechen. Das Handy-Mikrofon hört zu, das Ergebnis steht auf dem Display und wird vorgelesen. Es gelten dieselben Eingaben wie sonst („Karlsruhe“, „HH“, „Polen WZW“, „rückgängig“, „Land Polen“). Das Codewort ist hier nicht nötig.

**2. Unterhaltung „Kennzeichen“**
In der App: Menü → **Android Auto (Beta): Unterhaltung starten** (Benachrichtigungen erlauben). In Android Auto die Unterhaltung öffnen → **Antworten** → Kennzeichen sagen. Die Antwort kommt als Nachricht („KA, Stadt/Landkreis Karlsruhe, neu“).

Bekannte Einschränkungen: Während der Erkennung pausiert Musik kurz. Rückmeldungen und Fehlerberichte bitte als Issue.

### Updates
Menü → **Nach Updates suchen …**: Die App fragt GitHub nach der neuesten Version. Gibt es eine, siehst du die Neuerungen und kannst mit **Jetzt aktualisieren** die APK laden. Die App prüft die SHA-256-Prüfsumme und startet den Android-Installer, in dem du die Installation bestätigst. Deine Sammlung bleibt erhalten. Beim ersten Mal musst du Android einmalig erlauben, dass Kennzeichen Voice Updates installieren darf („Unbekannte Apps installieren“). Zusätzlich prüft die App einmal am Tag beim Start; bei einer neuen Version erscheint oben ein grüner Hinweis. Die automatische Prüfung kannst du im Menü ausschalten. Die erste Version mit dieser Funktion (1.8) musst du noch von Hand installieren.

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
- Updates: Die App fragt bei GitHub (api.github.com) nach der neuesten Version, auf Knopfdruck und automatisch einmal am Tag (abschaltbar). Dabei werden keine persönlichen Daten übertragen. Installiert wird nur nach deiner Bestätigung, und Android nimmt nur Updates mit dem gleichen Signaturschlüssel an.
- Kamera: Die Texterkennung (Google ML Kit) läuft auf dem Gerät. Der beim Scannen gelesene Kennzeichen-Text wird nur lokal im Verlauf der App gespeichert.

## Haftungsausschluss

Diese App wurde mit besten Absichten und nach bestem Wissen erstellt. Sie wird unentgeltlich und ohne jede Gewähr zur Verfügung gestellt. Es wird nicht zugesichert, dass sie fehlerfrei, vollständig, jederzeit verfügbar oder für einen bestimmten Zweck geeignet ist. Das gilt insbesondere für die Spracherkennung, die Texterkennung der Kamera und die Kennzeichen-Daten, die Fehler enthalten können.

Die Nutzung erfolgt auf eigene Gefahr. Für Schäden jeder Art, die aus der Nutzung oder Nichtnutzung der App entstehen – etwa Datenverlust, falsche Einträge, beschädigte oder nicht importierbare Backup-Dateien oder Unfälle durch Ablenkung im Straßenverkehr –, wird keine Haftung übernommen, soweit dies gesetzlich zulässig ist. Unberührt bleibt die Haftung für Vorsatz und grobe Fahrlässigkeit sowie für Schäden aus der Verletzung von Leben, Körper oder Gesundheit.

**Straßenverkehr:** Bediene die App nur, wenn weder du noch andere dadurch gefährdet werden. Als Fahrer gilt deine volle Aufmerksamkeit dem Verkehr. Den Kamera-Scanner nutzt du nur als Beifahrer oder im Stand.

**Deine Daten:** Erstelle regelmäßig Sicherungen deiner Sammlung (Menü → Backup exportieren). Bevor du ein von dieser App erzeugtes Backup in eine andere App einliest, sichere deren bestehende Daten.

**Datenquelle und Dritte:** Die Kennzeichen-Liste stammt aus dem GitHub-Projekt [JPTK04/kennzeichen](https://github.com/JPTK04/kennzeichen) und gehört dem jeweiligen Urheber; ihre Richtigkeit wurde nicht geprüft. Diese App ist ein inoffizielles Projekt und nicht mit der App „Kennzeichensammler“ verbunden.

**Datenschutz beim Fotografieren und Notieren:** Kfz-Kennzeichen können personenbezogene Daten sein. Nutze die App nur im Rahmen der geltenden Gesetze und veröffentliche keine Kennzeichen oder Standortdaten anderer Personen.

Dieser Text steht auch in der App unter Menü → „Info & Haftung“, dort zusammen mit einer Kurzanleitung für die Sprache.
