# Versionshistorie

Alle Versionen stehen unter [Releases](../../releases) zum Download bereit. Die SHA-256-Prüfsumme jeder APK steht in den Hinweisen des jeweiligen Releases.

## 2.2 – 02.11.2026
- **Neu: Parkplatzmodus.** Eigener Knopf **„🅿 Parkplatz“** unter dem Mikrofon. Ein Tipp startet das Zuhören ohne Codewort: Du sagst direkt das Kennzeichen („WI“, „Polen WGM“, einen Ortsnamen oder buchstabiert) und es wird sofort gewertet. Ein vorangestelltes „Kennzeichen“ stört nicht. „rückgängig“, „Land …“ und „Stopp“ funktionieren weiter. Erneutes Tippen auf den Knopf (oder Stopp am Mikrofon) beendet den Modus; er gilt nur, solange das Zuhören läuft. **Hinweis:** Im Parkplatzmodus wird alles Gesagte ausgewertet, auch Gespräche in der Nähe. Nur einschalten, wo sonst niemand redet.
- Neu: **Auswertung und Statistik** (Balkendiagramm-Symbol oben): was schon gesammelt ist, was noch fehlt, dazu Statistiken je Land.
- Das Kennzeichen-Schild zeigt den blauen EU-Streifen größer, mit besser lesbarer Länderkennung.
- Der Zwischenstand 2.1 wurde nicht veröffentlicht; 2.2 enthält alles davon.

## 2.0 – 01.11.2026
- **Neu (Beta): Android Auto.** Die App erscheint jetzt im Launcher des Autos als „Kennzeichen“ mit einem großen grünen Knopf **„Kennzeichen sagen“**. Der Knopf startet die Spracherkennung des Handys (Handy-Mikrofon), das Ergebnis steht groß auf dem Auto-Display und wird vorgelesen. Es gelten dieselben Eingaben wie sonst: Kürzel, Orte, „Polen WZW“, „rückgängig“, „Land Polen“. Zusätzlich gibt es die Unterhaltung „Kennzeichen“ (Menü → „Android Auto (Beta): Unterhaltung starten“), auf die du in Android Auto per „Antworten“ sprichst.
  - **Beta-Hinweis:** Die Funktion ist neu und nur eingeschränkt getestet. Android Auto hat keine Kategorie für diese App; sie meldet sich als „Orte“-App an und funktioniert nur, wenn in den Android-Auto-Entwickleroptionen **„Unbekannte Quellen“** eingeschaltet ist. Während der Erkennung pausiert Musik, danach läuft sie normalerweise weiter. Rückmeldungen willkommen.
- Neu: Die Liste in der App aktualisiert sich sofort, wenn über Android Auto ein Kennzeichen eingetragen wird (vorher erst nach Neustart der App).
- Behoben: Ein Ortsname wie „Karlsruhe“ wurde als mehrdeutig gewertet (KA und BR „Landkreis Karlsruhe“). Jetzt gewinnt der Ableitungsort (KA), und ein vollständiger Kreisname („Landkreis Karlsruhe“) gewinnt am meisten (BR).
- Die Zwischenstände 1.10 bis 1.12 wurden nicht veröffentlicht; 2.0 enthält alles davon.

## 1.8 – 01.11.2026
- Neu: **Updates aus der App.** Menü → „Nach Updates suchen …“ fragt GitHub nach der neuesten Version und zeigt die Neuerungen. Auf Wunsch lädt die App die APK herunter, prüft die SHA-256-Prüfsumme und übergibt sie an den Android-Installer; du bestätigst dort die Installation. Deine Daten bleiben erhalten. Zusätzlich prüft die App einmal pro Tag beim Start und zeigt bei einer neuen Version oben einen grünen Hinweis. Die automatische Prüfung lässt sich im Menü ausschalten. Beim ersten Mal verlangt Android eine einmalige Freigabe „Unbekannte Apps installieren“.
- Dunkelmodus dunkler: Status- und Navigationsleiste werden ausgeblendet, die Helligkeit geht auf das Minimum, der Hinweistext ist dunkler und verschwindet schneller. Android zeigt dabei beim ersten Mal eine eigene Vollbild-Meldung, die du mit „Verstanden“ bestätigst.

## 1.7 – 01.11.2026
- Neu: **Dunkelmodus** (Mond-Symbol oben). Das Display wird schwarz mit minimaler Helligkeit, das Zuhören läuft weiter und startet automatisch. Alle Berührungen werden geschluckt, beendet wird per **Doppeltipp** oder mit der Zurück-Taste. Ein Tipp blendet den Hinweis kurz ein.
- Behoben: Beim Scannen tschechischer (und anderer) Kennzeichen wurde die Länderkennung im EU-Streifen („CZ“) fälschlich als Region gelesen (z. B. „C“ für Südböhmen). Die Länderkennung wird jetzt ignoriert.

## 1.6 – 31.10.2026
- Kamera-Scanner: Der Rahmen ist jetzt kleiner und bleibt beim Zoomen gleich groß. Nur dieser kleinere Ausschnitt wird ausgewertet.
- Behoben: Teilen sich mehrere Zulassungsbezirke dasselbe Kürzel (BK, HZ, L, NH, ST, TG, TS), wurde beim Scannen immer nur der erste eingetragen und der zweite nie. Jetzt zählt jedes weitere Schild für den nächsten fehlenden Bezirk. Per Sprache gibt es dafür kein „Mehrdeutig“ mehr. Die Karte zeigt „Kürzel gilt für 2 Bezirke“.
- „Schon gesehen“ zeigt jetzt das Datum der ersten Sichtung an.
- Neu: Umschalter „Ausführlich: Ansage“ / „Schnell: nur Töne“ unter dem Mikrofon. Im Schnellmodus gibt es keine Sprachausgabe, sondern „ding-ding“ für neue Kennzeichen und „deet-deet“ für schon gesehen oder nicht erkannt. Das Codewort wird weiterhin mit einem Ton bestätigt.

## 1.5 – 31.10.2026
- Kamera-Scanner: Rahmen, in den das Kennzeichen gehalten wird. Nur dieser Bereich wird ausgewertet, dadurch werden entferntere Kennzeichen deutlich besser gelesen. Der Rahmen färbt sich orange, wenn ein Kennzeichen gelesen wird, und grün, wenn es erkannt wurde.
- Mehr Zoom: stufenlos per Zwei-Finger-Geste bis zum Maximum der Kamera, dazu Zoomstufen 1×, 2×, 4×, 8× und Max sowie eine Zoom-Anzeige.
- Antippen stellt an der Stelle scharf. Höhere Auflösung für die Texterkennung.

## 1.4 – 30.10.2026
- Neu: Die Versionsnummer wird in der App angezeigt (im Kopfbereich und im Dialog „Info & Haftung“).

## 1.3 – 30.10.2026
- Neu: Einträge für ein anderes Land per Sprache, ohne den Modus zu wechseln: „Kennzeichen Polen WA“, „Kennzeichen Bulgarien CA“. „Kennzeichen HH“ ergibt weiterhin Hamburg.
- Die Ergebniskarte zeigt in diesem Fall das Land und den passenden Länderstreifen auf dem Schild.

## 1.2 – 30.10.2026
- Neu: NATO-Buchstabieralphabet (englisch) in der Spracheingabe, auch mit eingedeutschten Schreibweisen („Oskar“, „Maik“).
- Neu: Kurzanleitung für die Sprache in der App (Menü → Info & Haftung).

## 1.1 – 30.10.2026
- Neu: Haftungsausschluss in der App (beim ersten Start und im Menü) und in der README.

## 1.0 – 30.10.2026
- Erste Version: Spracheingabe mit Codewort „Kennzeichen“, Kamera-Scanner, Import/Export des Kennzeichensammler-Backups, CSV-Liste, 37 Länder. Die Kennzeichen-Liste wird beim ersten Start geladen.
- Hinweis: Dieser Release wurde kurz nach der Veröffentlichung durch 1.1 ersetzt, weil der Haftungsausschluss fehlte, und ist nicht mehr als Download verfügbar.
