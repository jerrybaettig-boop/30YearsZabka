# Fabi-Geschenk-Seite — Setup-Anleitung

## 1. Formspree einrichten (damit du ihre Antworten per E-Mail bekommst)
1. Gehe auf https://formspree.io und erstelle einen kostenlosen Account.
2. Erstelle ein neues Formular, du bekommst eine Endpoint-URL wie
   `https://formspree.io/f/abcd1234`.
3. Öffne `geschenk/quiz.html`, suche die Zeile:
   `const FORMSPREE_ENDPOINT = "https://formspree.io/f/DEIN_CODE_HIER";`
   und ersetze `DEIN_CODE_HIER` mit deinem echten Code.
4. Formspree verlangt beim allerersten Test eine Bestätigung per E-Mail —
   einmal durchklicken lassen, bevor du den Link an sie schickst.

## 2. Bilder ergänzen
Siehe `images/README.md` für die genaue Liste. Bilder einfach mit dem
passenden Dateinamen in den `images`-Ordner legen.

## 3. Auf GitHub Pages publishen
1. Erstelle ein neues GitHub-Repository (z. B. `fabi-geschenk`).
2. Lade den kompletten Inhalt dieses Ordners hoch (alle Dateien und
   Unterordner: `assets/`, `geschenk/`, `images/`, alle `.html`-Dateien).
3. Gehe im Repo zu Settings → Pages.
4. Bei "Source" wähle den `main`-Branch und Ordner `/ (root)`.
5. Nach ein bis zwei Minuten ist die Seite erreichbar unter:
   `https://DEIN-GITHUB-NAME.github.io/fabi-geschenk/`

## 4. Testen vor dem Fest
- Öffne die Seite selbst einmal komplett durch (Passcode-Quiz und
  Reise-Quiz), damit du siehst, ob die Formspree-Mail ankommt.
- Der Fortschritt beim Passcode-Quiz wird nur im Browser der Person
  gespeichert (sessionStorage) — beim Schliessen des Tabs geht er
  verloren, das ist so gewollt (kein Vorspulen ohne Quiz).

## Struktur
```
index.html              Startseite mit Navigation
the-beginning.html       Kennenlern-Geschichte
highlights.html          Bildergalerie
hobbies.html             Hobbies-Übersicht
spruche.html             Zitate (noch mit Platzhaltern)
ueber-sie.html           Kurzporträt
assets/style.css         Gemeinsames Stylesheet
geschenk/index.html      Passcode-Quiz (6 Fragen -> Code 11.11.22)
geschenk/quiz.html       Reise-Quiz (20 Fragen -> Destination + Termine)
images/                  Alle Bilder
```
