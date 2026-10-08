# Themes – semantische Tokens pro Marke

Jede Marke ist ein **Theme** (Token-Set) im Token-Repo. Ein Theme belegt die geteilten [Primitive](./foundations.md) mit semantischer Bedeutung (`primary`, `background`, `foreground`, `border`, `ring`, `destructive` …) – shadcn-kompatibel, mit Light-/Dark-Mode.

## Überblick

| Marke / Produkt | Theme | Primary | Neutrals | Status |
|---|---|---|---|---|
| Get IT Done | `blue` | `blue.600` `#2563eb` | slate / gray | live im Frontend |
| workload.zero (ZERO) | `workbase` (Umbenennung in `zero` offen) | `blue.600` `#2563eb` | slate | Theme vorhanden |
| WERK | – | – | – | **noch zu definieren** |

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

## workload.zero — Theme `workbase`

Das bisherige Workbase-Theme ist das Theme von workload.zero und allen .zero-Produkten. Eigenes Theme, eng verwandt mit `blue` (gleiche Primärfarbe), Neutrals konsequent auf `slate` referenziert.

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
- Kantigere Radien / nüchternere Anmutung als workload.zero?
- Eigene Dark-Mode-Variante für Werkshallen-/Shopfloor-Kontexte?

## workload.zero — offene Punkte

- Umbenennung des Token-Sets `workbase` in `zero` im Token-Repo (Breaking Change für konsumierende Apps, daher mit Major-Release).
- Ob die fünf .zero-Produkte eigene Akzentfarben bekommen oder alle das Suite-Theme teilen. Empfehlung: ein Suite-Theme, Unterscheidung über Produktname und Icon, nicht über Farbe.

---

**Änderungen an Werten** erfolgen im Token-Repo (`figma-tokens/themes/*`), nicht hier. Neue Themes (`werk`, ggf. `zero`) legen wir dort als Token-Set an; dieses Dokument spiegelt die Zuordnung wider.
