# Fabi-Geschenk-Seite — Setup-Anleitung (Update)

## 1. Formspree einrichten
1. https://formspree.io — kostenlosen Account MIT jerry.baettig@gmail.com erstellen
   (das Konto-E-Mail ist automatisch das Empfänger-Postfach).
2. Neues Formular erstellen, Endpoint-URL kopieren (z.B. https://formspree.io/f/abcd1234)
3. In `geschenk/quiz.html` die Zeile mit FORMSPREE_ENDPOINT anpassen.
4. Ersten Test-Versand per E-Mail bestätigen (Formspree verlangt das einmalig).

## 2. Admin-Code für Zurücksetzen
In `geschenk/quiz.html` steht `const ADMIN_CODE = "KNOBLI2026";` — passe den
Code an, falls gewünscht. Falls das Quiz schon abgeschlossen wurde und
nochmal gemacht werden soll, gibt man diesen Code auf der Sperrseite ein.
Wichtig: das ist ein rein clientseitiger Schutz (kein echtes Server-Login) —
für den Partyzweck aber ausreichend.

## 3. Bilder ergänzen
Siehe `images/README.md`. Eure eigenen Fotos sind schon eingebaut
(Highlights, Hobbies, Startseite). Es fehlen noch die Quiz-Bild-Fragen
und ein Foto von dir für den Gutschein am Schluss.

## 4. Community-Foto-Wand (optional)
GitHub Pages kann keine Uploads von Gästen entgegennehmen (kein Server).
Empfehlung: kostenloses Padlet (padlet.com) erstellen, Link/QR-Code am
Fest bereitstellen, als Kachel auf `highlights.html` vermerkt.

## 5. Fragen im Reise-Quiz anpassen
Nutze `reise-quiz-fragen.xlsx` (separat mitgeliefert) — dort sind alle
20 Fragen mit Antworten, Bildern und Punkte-Vergabe editierbar. Schick
mir die ausgefüllte Datei zurück, ich baue den Code neu.

## 6. Auf GitHub Pages publishen
Wie gehabt: Dateien hochladen (inkl. neuer `bauplan.html`, ohne die alte
`ueber-sie.html` — die wurde ersetzt), Settings → Pages → main / root.

## Struktur (aktualisiert)
```
index.html              Startseite (Sticky-Nav, Foto-Badge)
the-beginning.html       Kennenlern-Geschichte + Diashow
highlights.html          Bildergalerie (echte Fotos) + Padlet-Hinweis
hobbies.html             Hobbies mit Foto-Karten
spruche.html             Zitate (Platzhalter)
bauplan.html             NEU: "Bauplan von Fabi" Infografik
assets/style.css         Zabka-Park Design + Sticky-Nav
geschenk/index.html      Passcode-Quiz (8 Fragen -> 11.11.22)
geschenk/quiz.html       Reise-Quiz (20 Fragen, Resume, One-Time-Gate, PDF-Gutschein)
images/                  Alle Bilder
reise-quiz-fragen.xlsx   Editierbare Fragentabelle (separat)
```
