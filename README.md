# Riber Shamo Elias – Personal Website

Professionelles, statisches Portfolio-Projekt mit Hauptseite und separater Link-Hub-Seite für GitHub Pages.

## Live

- Hauptdomain: https://ribershamoelias.com
- Repository: https://github.com/ribershamoelias/ribershamoelias.github.io

## Projektüberblick

Dieses Repository enthält zwei statische Web-Frontends:

1. Hauptseite (`/`) mit Navigation, Hero, About, Systems, Today
2. Linkseite (`/my-links`) mit externen Profilen und rechtlichen Hinweisen

Das Projekt ist bewusst ohne Build-Tooling umgesetzt (Plain HTML/CSS/JavaScript), um Wartung, Deployment und langfristige Stabilität einfach zu halten.

## Struktur

```text
.
├── CNAME
├── index.html
├── style.css
├── script.js
├── PERSONAL_WEBSITE.md
├── my-links/
│   ├── index.html
│   ├── style.css
│   ├── background.js
│   ├── script.js
│   └── links.json
└── README.md
```

## Tech Stack

- HTML5
- CSS3 (Custom Properties, Responsive Layout)
- Vanilla JavaScript
- GitHub Pages + Custom Domain (`CNAME`)

## Lokal starten

Option 1 (empfohlen):

```bash
python3 -m http.server 8000
```

Dann öffnen:

- `http://localhost:8000`
- `http://localhost:8000/my-links/`

Option 2:

- Dateien direkt im Browser öffnen (für schnelle Sichtprüfung)

## Deployment auf GitHub Pages

1. Repository nach GitHub pushen (`https://github.com/ribershamoelias/ribershamoelias.github.io`).
2. In GitHub: `Settings` → `Pages`.
3. Source auf Branch `main` und Root setzen.
4. Domain mit `CNAME` (`ribershamoelias.com`) verknüpfen.
5. DNS-Einträge beim Domain-Provider auf GitHub Pages zeigen lassen.

Optional (falls lokal noch kein Remote gesetzt ist):

```bash
git remote add origin https://github.com/ribershamoelias/ribershamoelias.github.io.git
git branch -M main
git push -u origin main
```

## Inhalt anpassen

- Hauptseite: `index.html`, `style.css`, `script.js`
- Linkseite: `my-links/index.html`, `my-links/style.css`, `my-links/background.js`
- Zusätzliche Linkdaten (optional): `my-links/links.json`

Weitere Detailanleitung: [PERSONAL_WEBSITE.md](./PERSONAL_WEBSITE.md)

## Qualität & Wartung

- Keine externen Build-Abhängigkeiten
- Klare Trennung von Hauptseite und Link-Hub
- Deployment-freundlich für statisches Hosting
- Rechtstexte (Impressum/Datenschutz) auf `my-links` integriert

## Hinweise

- Die Datei `my-links/script.js` enthält aktuell Legacy-/Experimentiercode und ist in `my-links/index.html` nicht eingebunden.
- Für kollaborative Arbeit siehe [CONTRIBUTING.md](./CONTRIBUTING.md).
- Für Sicherheitsmeldungen siehe [SECURITY.md](./SECURITY.md).

## Lizenz

Aktuell ist keine Open-Source-Lizenz hinterlegt.
Falls externe Beiträge oder Wiederverwendung gewünscht sind, sollte eine passende Lizenzdatei (`LICENSE`) ergänzt werden.
