# Themes – semantische Tokens pro Marke

Jede Marke ist ein **Theme** (Token-Set) im Token-Repo. Ein Theme belegt die geteilten [Primitive](./foundations.md) mit semantischer Bedeutung (`primary`, `background`, `foreground`, `border`, `ring`, `destructive` …) – shadcn-kompatibel, mit Light-/Dark-Mode.

## Überblick

| Marke / Produkt | Theme | Primary | Neutrals | Status |
|---|---|---|---|---|
| Get IT Done | `blue` | `blue.600` `#2563eb` | slate / gray | live im Frontend |
| Workbase (WORK) | `workbase` | `blue.600` `#2563eb` | slate | Theme vorhanden |
| WERK | – | – | – | **noch zu definieren** |
| WORK (Marke) | offen | – | – | **noch zu klären** |

## Get IT Done — Theme `blue`

Unser aktuelles Auftreten (Dachmarke, Frontend).

| Semantisches Token | Wert |
|---|---|
| `primary` | `{blue.600}` = `#2563eb` |
| `ring.default` | `{blue.600}` |
| `foreground.default` | `{slate.900}` |
| `foreground.muted` | `#64748b` (`slate.500`) |
| `background` | `{basic.white}` |
| `background.muted` | `#f1f5f9` (`slate.100`) |
| `error` | `{red.500}` |

## Workbase — Theme `workbase`

Eigenes Theme, eng verwandt mit `blue` (gleiche Primärfarbe), Neutrals konsequent auf `slate` referenziert.

| Semantisches Token | Wert |
|---|---|
| `primary` | `{blue.600}` = `#2563eb` |
| `foreground.default` | `{slate.900}` |
| `foreground.muted` | `{slate.500}` |
| `background` | `{basic.white}` |
| `background.muted` | `{slate.100}` |
| `button.background.hover` | `{blue.700}` |
| `button.subtle.default` | `{slate.100}` |

## WERK — noch zu definieren

WERK adressiert einen anderen Markt (industriell, seriös, B2B). Wir sollten ein **eigenes Theme `werk`** anlegen, statt `blue` mitzunutzen. Offene Fragen:

- Eigene Primärfarbe, die zu „industrieller Arbeit" passt (z. B. ein technisches Blau/Stahl oder ein Signal-Akzent)?
- Kantigere Radien / nüchternere Anmutung als WORK?
- Eigene Dark-Mode-Variante für Werkshallen-/Shopfloor-Kontexte?

## WORK — noch zu klären

Zu entscheiden: Bekommt die **Marke WORK** ein eigenes Theme, oder ist das `workbase`-Theme faktisch das WORK-Theme (weil Workbase das erste und tragende WORK-Produkt ist)? Empfehlung: zunächst `workbase` als WORK-Referenz nutzen und erst bei einem zweiten WORK-Produkt aufsplitten.

---

**Änderungen an Werten** erfolgen im Token-Repo (`figma-tokens/themes/*`), nicht hier. Neue Themes (`werk`, ggf. `work`) legen wir dort als Token-Set an; dieses Dokument spiegelt die Zuordnung wider.
