# Constellation of the Good

Eine immersive Kunstausstellung von Lucas Denhof, Joshua Jackson, Jonas Riedinger, Yuanzhen Sun.

Zwölf Philosoph*innen, angeordnet nach ihrer Antwort auf die Frage: Was macht einen guten Menschen aus?

## Aufbau

Statische Website — kein Build-Schritt, keine Abhängigkeiten. Die Dateien werden so ausgeliefert, wie sie hier liegen.

```
index.html              Startseite mit der Konstellations-Karte
style.css               gemeinsame Styles für alle Seiten
profiles/               zwölf Profilseiten
Assets/heads_web/       Porträts der Köpfe (WebP)
Assets/BG/              Hintergrund (WebP)
.nojekyll               schaltet Jekyll-Verarbeitung auf GitHub Pages ab
```

## Lokal ansehen

```bash
python -m http.server 8000
```

Dann http://localhost:8000 öffnen. (Ein Doppelklick auf `index.html` funktioniert auch, aber über den Server entspricht es dem späteren Live-Verhalten.)

## Auf GitHub Pages veröffentlichen

1. Inhalt dieses Ordners in ein Repository pushen (Branch `main`).
2. Im Repo unter **Settings → Pages** als Quelle `main` und Ordner `/ (root)` wählen.
3. Die Seite erscheint nach ein bis zwei Minuten unter `https://<user>.github.io/<repo>/`.

Alle internen Pfade sind relativ, die Seite läuft also sowohl unter einer eigenen Domain als auch in einem Unterordner wie `/<repo>/`.

## Hinweise

- Die Schrift **Manrope** wird von Google Fonts geladen — die einzige externe Abhängigkeit. Ohne Internetverbindung fällt die Seite auf eine System-Schrift zurück.
- Die Porträts liegen als WebP vor (~820 KB insgesamt). Die PNG-Originale sind bewusst nicht Teil dieses Builds.
