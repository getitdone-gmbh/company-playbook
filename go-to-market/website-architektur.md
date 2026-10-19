# Website-Architektur

So strukturieren wir die Auftritte von Get IT Done und unseren drei Marken.

## Get IT Done

**Website:** <https://itdone.de>

Unsere Hauptnavigation:

- Unternehmen
- WERK
- workload.zero
- KETTE
- Leistungen
- Referenzen
- Kontakt

Auf der Startseite machen wir alle drei Produktwelten direkt sichtbar.

## WERK

**Produkt-Websites:** WERK Agent → <https://werksagent.de> · WERK Cloud → <https://itdone.cloud>

Unsere Navigation:

- **Produkte**
  - WERK Agent
  - WERK Cloud
  - später WERK Einsatz
- **Lösungen**
  - Qualität
  - Stillstand
  - Instandhaltung
  - Industrial AI
  - Service
- Branchen
- Sicherheit
- Referenzen
- Demo

## ZERO (workload.zero)

**Suite-Website:** workload.zero → workloadzero.de (bis zur Umstellung <https://workbase.itdone.de>)

**Produkt-Websites:** backoffice.zero → backofficezero.de · workstream.zero → workstreamzero.de · vacancy.zero → vacancyzero.de · jobsearch.zero → jobsearchzero.de · coldcall.zero → coldcallzero.de

Navigation der Suite-Website:

- **Produkte**
  - backoffice.zero
  - workstream.zero
  - vacancy.zero
  - jobsearch.zero
  - coldcall.zero
- **Für wen**
  - Freelancer und Solos
  - Agenturen und Dienstleister
  - Vermittler
  - Professionals
- Preise
- Ressourcen
- Login
- Kostenlos testen

Jede Produkt-Landingpage führt mit dem Problem, das das Produkt auf null bringt, verweist auf die Suite ("part of workload.zero") und hat einen eigenen Testzugang. Themen wie E-Rechnung, DATEV und Freelancer-CV bekommen eigene SEO-Seiten unter dem jeweiligen Produkt.

## KETTE (Die Kette)

Eigene Marke seit [ADR 0003](../decisions/0003-kette-eigene-marke.md). Der Auftritt läuft heute auf Subdomains von itdone.de. Ob KETTE eigene Domains bekommt, klären wir mit der Markenprüfung.

| Domain | Rolle |
|---|---|
| <https://kette.itdone.de> | Verkaufsseite mit Warteliste, Paketvergleich, Making-of und FAQ |
| <https://kette.itdone.de/ueberfuehrung> | Unterseite für Firmen mit bestehendem Design System, Anfrage zur Bestandsaufnahme |
| <https://components.itdone.de> | öffentliches Storybook der Komponenten (Library) |
| <https://zero.itdone.de> | öffentliches Storybook der Fachkomponenten (zero) |
| <https://zero-pages.itdone.de> | öffentliches Storybook der Seitenvorlagen (Zero Pages) |
| <https://zero-design.itdone.de> | interaktiver Prototyp von workload.zero, erste Station der Kette |

Navigation der Verkaufsseite:

- Kette
- Making-of
- Geprüft
- So läuft's
- Warteliste
- Überführung
- FAQ

Die Storybooks und der Prototyp sind das Schaufenster von KETTE. Sie sind ohne Login erreichbar, dienen als nachprüfbarer Beleg und lassen sich im Team weiterreichen. Alle Oberflächen zeigen fiktive Beispieldaten.

**Verknüpfung mit den anderen Auftritten:** Die .zero-Landingpages verkaufen workload.zero und verweisen nicht aktiv auf KETTE. Auf itdone.de führt KETTE als eigene Produktwelt in der Hauptnavigation, die Überführung erscheint zusätzlich unter Leistungen.
