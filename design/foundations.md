# Foundations – geteilte Primitive Tokens

Die geteilte Basis aller Marken. **Quelle der Wahrheit:** `figma-tokens/core.json` im Token-Repo (`@alexfriedl/figma-design-tokens`). Die Werte hier sind eine lesbare Zusammenfassung, kein Ersatz.

## Farbprimitive

Das Fundament entspricht der **shadcn/Tailwind-Palette** (`slate`, `gray`, `zinc`, `blue`, `red` …), jeweils in Stufen `50`–`900`/`950`. Auszug der bei uns tragenden Skalen:

**Blue** (unsere aktuelle Primärfarbe, siehe [themes.md](./themes.md)):

| Token | Hex |
|---|---|
| `blue-500` | `#3b82f6` |
| `blue-600` | `#2563eb` ← Primary |
| `blue-700` | `#1d4ed8` |

**Slate / Gray** (Neutrals – Text, Flächen, Rahmen):

| Token | Hex | Typische Nutzung |
|---|---|---|
| `white` | `#ffffff` | Basis-Hintergrund |
| `slate-50` | `#f8fafc` | Flächen |
| `slate-100` | `#f1f5f9` | Flächen / muted background |
| `slate-500` | `#64748b` | muted foreground |
| `slate-900` | `#0f172a` | Text / foreground default |
| `gray-200` | `#e5e7eb` | Rahmen / Trennlinien |
| `gray-600` | `#4b5563` | sekundärer Text |
| `gray-900` | `#111827` | primärer Text (Get-IT-Done-Frontend) |

> Die vollständige Palette (alle Farben, alle Stufen) steht in `figma-tokens/core.json`.

## Typografie

**Schriftfamilie (Get-IT-Done-Frontend):** Inter (Google Fonts, via `next/font`), mit System-Fallback.

**Type-Scale (fluid, `clamp()`):** responsiv skalierend, definiert in `getitdone/frontend/tailwind.config.js`.

| Token | min → max | Zeilenhöhe |
|---|---|---|
| `text-xs` | 0.75 → 0.875 rem | 1.5 |
| `text-sm` | 0.875 → 1 rem | 1.5 |
| `text-base` | 1 → 1.125 rem | 1.75 |
| `text-lg` | 1.125 → 1.25 rem | 1.75 |
| `text-xl` | 1.25 → 1.5 rem | 1.75 |
| `text-2xl` | 1.5 → 1.875 rem | 1.5 |
| `text-3xl` | 1.875 → 2.25 rem | 1.2 |
| `text-4xl` | 2.25 → 3 rem | 1.1 |
| `text-5xl`–`text-9xl` | 3 → 12 rem | 1–1.1 |

> Das Token-Repo pflegt Typografie und **Breakpoints** (`sm`/`md`/`lg`) zusätzlich als eigene Token-Sets.

## Spacing & Radius

Standard-Tailwind-Skala (`0.25rem`-Schritte) und shadcn-Radien. Markenspezifische Abweichungen (z. B. WERK kantiger, WORK weicher) dokumentieren wir bei Bedarf im jeweiligen Theme in [themes.md](./themes.md).

## Modi

Das Token-System unterstützt **Light- und Dark-Mode** (`default_theme.json` / `default_theme_dark.json`), umschaltbar zur Laufzeit über `setMode('dark')`.
