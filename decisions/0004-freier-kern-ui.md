# ADR 0004: Freier Kern @getitdone-gmbh/kette-design-community neben der privaten Library

- **Status:** akzeptiert
- **Datum:** 2026-10-19
- **Betroffene Bereiche:** KETTE, Design System, Open Source, Go-to-Market

## Kontext

Unsere Komponenten-Library `getitdone-gmbh/component-library-react` ist privat und Teil von Die Kette ([ADR 0003](./0003-kette-eigene-marke.md)). Ihre Lizenz verbietet die Weitergabe, und ihre Git-Geschichte enthält Dateien mit ungeklärter Lizenz.

Für Sichtbarkeit (npm, shadcn-Verzeichnis, Backlinks) wollen wir trotzdem einen Teil frei anbieten, ohne das Bezahlprodukt zu verschenken.

## Entscheidung

Wir veröffentlichen einen **freien Kern** als eigenes, öffentliches Repo **`getitdone-gmbh/kette-design-community`** (MIT, npm `@getitdone-gmbh/kette-design-community`, shadcn-Registry `zero-design.itdone.de/r`).

| | component-library-react | kette-design |
|---|---|---|
| Sichtbarkeit | privat | öffentlich |
| Lizenz | Die Kette | MIT |
| Inhalt | alle Komponenten | Primitives und allgemeine Komponenten |
| Registry | GitHub Packages | npmjs.com |
| Geschichte | vollständig | neu, ohne alte Historie |
| Rolle | Quelle, hier wird entwickelt | Schaufenster, Kopie der Quelle |

Regeln:

1. **Die Library ist die Quelle.** Komponenten werden nie zuerst in `kette-design` geändert, sondern in der Library und von dort übernommen.
2. **Nicht in `kette-design`:** Fachkomponenten (zero), Seitenvorlagen (zero-pages), Agenten, Regeln und alles mit Kundenbezug. Das bleibt Die Kette.
3. **Abgleich nach jedem Library-Release:** Komponenten-Schnappschuss, Theme aus den Design-Tokens, Tests, Registry, npm-Release. Ablauf in `getitdone-gmbh/kette-design-community/docs/MAINTAINING.md`.
4. **Veröffentlichen auf npm** macht Alex im eigenen Terminal (Bestätigung im Browser).

## Zuständigkeit

- **Abgleich und Release von `kette-design`:** Agent `design-system-release-engineer` (Abschnitt "Freier Kern").
- **Überwachung:** Agent `design-system-atlas-keeper` führt `kette-design` im Atlas und meldet, wenn es hinter der Library zurückliegt.
- **Inhaltliche Grenzen (was frei wird):** Alex.

## Konsequenzen

- Ohne Abgleich veraltet `kette-design` mit jedem Library-Release; der Atlas macht das sichtbar.
- Zwei Komponenten-Bestände bedeuten doppelte Pflege. Deshalb nur Kopie, nie eigene Weiterentwicklung in `kette-design`.
