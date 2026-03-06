# Personalisierungsleitfaden

Diese Datei beschreibt, wie das Projekt strukturiert ist und welche Stellen für inhaltliche oder visuelle Anpassungen vorgesehen sind.

## 1) Hauptseite (`/`)

### Relevante Dateien

- `index.html` – Struktur und Inhalte
- `style.css` – Designsystem, Layout, Responsive-Verhalten
- `script.js` – Typing-Animation und UI-Interaktionen

### Typische Anpassungen

- Name, Claim, Texte in `index.html` aktualisieren
- Navigationseinträge und Kontaktlink (`mailto:`) prüfen
- Farbvariablen in `style.css` unter `:root` anpassen
- Texte der Typing-Animation in `script.js` (`words`-Array) bearbeiten

## 2) Linkseite (`/my-links`)

### Relevante Dateien

- `my-links/index.html` – Linkkarten, Impressum, Datenschutz
- `my-links/style.css` – Styling und Modal-Darstellung
- `my-links/background.js` – interaktiver Partikelhintergrund + Modal-Steuerung
- `my-links/links.json` – optionale strukturierte Linkliste

### Hinweise

- Aktuell sind die sichtbaren Karten direkt in `my-links/index.html` gepflegt.
- `my-links/script.js` ist derzeit nicht eingebunden und hat keinen Einfluss auf die produktive Ansicht.

## 3) Lokales Testing

```bash
python3 -m http.server 8000
```

Testen:

- `http://localhost:8000`
- `http://localhost:8000/my-links/`

## 4) Deployment-Checkliste

- [ ] Repository korrekt verbunden: `https://github.com/ribershamoelias/ribershamoelias.github.io`
- [ ] Inhalte und Links final prüfen
- [ ] Rechtliche Texte (Impressum/Datenschutz) verifizieren
- [ ] Mobile Ansicht validieren
- [ ] GitHub Pages aktivieren
- [ ] Custom Domain (`CNAME`) + DNS prüfen

## 5) Qualitätsrichtlinien

- Semantische HTML-Struktur beibehalten
- Konstante Designsprache zwischen Haupt- und Linkseite
- Keine ungenutzten Skripte dauerhaft im produktiven Pfad belassen
- Änderungen immer lokal testen, bevor sie gepusht werden