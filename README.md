# Music Logger Docs

Dies ist das Dokumentations-Repository für die **Music Logger App**.
Die Dokumentation basiert auf [MkDocs](https://www.mkdocs.org/) und dem Theme [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

Die Live-Version ist hier verfügbar: [https://adn94.github.io/music-logger-docs/](https://adn94.github.io/music-logger-docs/)

---

## 🚀 Erste Schritte

### 1. Voraussetzungen
Du benötigst **Python** installiert.
Installiere dann MkDocs und das Material Theme:

```bash
pip install mkdocs-material
```

### 2. Lokalen Server starten
Um die Änderungen live zu sehen, während du schreibst:

```bash
mkdocs serve
```
Die Seite ist dann unter `http://127.0.0.1:8000` erreichbar.

---

## 📝 Inhalte bearbeiten

### Neue Seite hinzufügen
1.  Erstelle eine neue `.md` Datei im Ordner `docs/` (z.B. `docs/kontakt.md`).
2.  Öffne die Datei `mkdocs.yml`.
3.  Füge die neue Seite unter `nav:` hinzu:

```yaml
nav:
  - Home: index.md
  - Kontakt: kontakt.md  # <-- Neue Seite hier eintragen
  - Rechtliches: ...
```

### Bestehende Inhalte ändern
Bearbeite einfach die entsprechenden Markdown-Dateien im `docs/` Ordner.

---

## ☁️ Veröffentlichen (Deploy)

Um die Änderungen auf GitHub Pages online zu stellen:

1.  Stelle sicher, dass alles funktioniert (`mkdocs serve`).
2.  Führe folgenden Befehl aus:

```bash
mkdocs gh-deploy
```

Dies baut die Webseite und lädt sie automatisch in den `gh-pages` Branch auf GitHub hoch.
Vergiss nicht, deine Änderungen (Quellcode) auch normal zu committen und zu pushen:

```bash
git add .
git commit -m "update documentation"
git push
```
