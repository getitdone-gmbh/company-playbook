# Design & Marken-Tokens

So beschreiben wir unsere Marken visuell – über **Design-Tokens**: benannte, wiederverwendbare Werte für Farbe, Typografie, Abstände und mehr. Ein gemeinsames Fundament, darüber pro Marke ein eigenes Theme. Das ist die visuelle Übersetzung unseres Leitgedankens: **gemeinsame Technologie – getrennte Marken**.

## Single Source of Truth: das Token-Repo

Unsere Tokens leben **nicht** in diesem Playbook, sondern in einem eigenen, aus Figma gesyncten Repository:

**`figma-design-tokens`** – `@alexfriedl/figma-design-tokens` (npm, GitHub Packages)

Dieses Playbook *beschreibt* das System und die Marken-Zuordnung; die konkreten Werte pflegen wir zentral dort. So vermeiden wir zwei konkurrierende Quellen.

### Pipeline

```text
Figma Native Variables
        │  (Export)
        ▼
figma-tokens/*.json        ← Tokens-Studio-Format (core, default_theme, themes/*)
        │  Style Dictionary
        ▼
dist/
├── tailwind.preset.cjs    → Tailwind-Preset für Produkt-UIs
├── theme.css              → CSS-Variablen (Light/Dark)
└── themes.js              → Runtime setTheme() / setMode()
```

Das Fundament ist **shadcn/ui**-kompatibel (semantische Tokens wie `primary`, `background`, `foreground`, `border`, `ring`, `destructive` …), mit **Light- und Dark-Mode**.

## Aufbau in drei Ebenen

1. **Primitive Tokens** (geteilt) – Rohwerte: `slate`, `gray`, `blue` … Type-Scale, Breakpoints. Quelle: `figma-tokens/core.json`. Siehe [foundations.md](./foundations.md).
2. **Semantische Tokens pro Theme** – `primary`, `background`, `foreground` usw., je Marke unterschiedlich belegt. Siehe [themes.md](./themes.md).
3. **Komponenten-Tokens** – z. B. `button.background.hover` – bereits im Token-Repo vorhanden, pro Theme.

## Marke → Theme

Jede Marke ist ein **Theme** (Token-Set) im Token-Repo. Details und Werte in [themes.md](./themes.md).

| Marke / Produkt | Theme | Status |
|---|---|---|
| Get IT Done (Dachmarke) | `blue` | live im Frontend |
| Workbase (WORK) | `workbase` | Theme vorhanden |
| WERK | — | **noch zu definieren** |
| WORK (Marke) | offen | **noch zu klären** |

## Pflege-Regel

> Die Werte ändern wir im **Token-Repo**, nicht hier. Dieses Playbook hält nur Architektur, Zuordnung und Prinzipien fest – und bleibt damit pflegearm.

## Marken- und Nutzungsrechte

Farb-, Typo- und Spacing-Tokens sind bewusst offen dokumentiert. **Unsere Logos, Wortmarken und das visuelle Erscheinungsbild sind markenrechtlich geschützt und nicht Teil der [CC-BY-Freigabe](../LICENSE)** dieses Playbooks.
