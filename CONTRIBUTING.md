# Contributing Guide

Vielen Dank für Beiträge zu diesem Projekt.

## Entwicklungsprinzipien

- Änderungen klein, fokussiert und nachvollziehbar halten.
- Bestehende Struktur respektieren (statisch, ohne Build-Tooling).
- Keine unnötigen Frameworks oder Abhängigkeiten hinzufügen.
- Vor jedem Commit lokal testen.

## Lokales Setup

```bash
python3 -m http.server 8000
```

Prüfen:

- http://localhost:8000
- http://localhost:8000/my-links/

## Branching

Empfohlene Branch-Namen:

- `feat/<kurze-beschreibung>`
- `fix/<kurze-beschreibung>`
- `docs/<kurze-beschreibung>`

## Commit-Konvention (empfohlen)

- `feat: ...`
- `fix: ...`
- `docs: ...`
- `refactor: ...`
- `chore: ...`

Beispiel:

```text
fix: guard missing loader element in main script
```

## Pull Request-Checkliste

- [ ] Änderung ist klar abgegrenzt
- [ ] Seiten lokal getestet (Desktop + Mobile)
- [ ] Keine defekten Links eingeführt
- [ ] Rechtstexte bleiben konsistent
- [ ] README / Doku bei Bedarf aktualisiert

## Code-Style

- Verständliche, sprechende Bezeichner verwenden
- Bestehende Formatierung pro Datei beibehalten
- Kein toter Code im produktiven Pfad

## Was nicht Teil dieses Repositories ist

- Kein Backend
- Keine Build-Pipeline
- Kein Paketmanager-Setup (npm/pnpm/yarn)
