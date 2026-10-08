# Company Playbook

Unser öffentliches Playbook: Produkt- und Markenstrategie, Positionierung, Go-to-Market, Prozesse und ausgewählte Standards der **Get IT Done GmbH** – in unseren eigenen Worten.

> _Public playbook for product strategy, brand architecture, go-to-market, processes and selected company standards at Get IT Done GmbH._

Alles Wissenswerte, das wir öffentlich teilen können, sammeln wir hier als versionierte Markdown-Dateien. Jede Änderung ist über die Git-Historie nachvollziehbar.

---

## Unsere Markenarchitektur auf einen Blick

```text
Get IT Done GmbH
│
├── WERK   – Software und Services für Fertigung, Produktion und industrielle Arbeit
│   ├── WERK Agent   – Produktionsdaten verstehen
│   ├── WERK Cloud   – Anwendungen und KI sicher betreiben
│   ├── WERK Einsatz – Service- und Einsatzmanagement (in Validierung)
│   └── weitere vertikale WERK-Produkte
│
└── ZERO   · workload.zero, die modulare Business-Suite für Unternehmen, Teams und Professionals
    ├── backoffice.zero  · Verwaltung, Zeiten, Personal, Abrechnung
    ├── workstream.zero  · Projekte, Ressourcen, Zusammenarbeit
    ├── vacancy.zero     · Recruiting und Vermittlung
    ├── jobsearch.zero   · Profil, CV, Job- und Projektmatching
    └── coldcall.zero    · Sales-CRM und Kundengewinnung
```

**Unser Leitgedanke:** Gemeinsames Unternehmen und gemeinsame Technologie – aber getrennte Märkte, Botschaften und Vertriebssysteme.

---

## Offizielle Websites

| Marke / Produkt | Website |
|---|---|
| Get IT Done GmbH | <https://itdone.de> |
| WERK Agent | <https://werksagent.de> |
| WERK Cloud | <https://itdone.cloud> |
| workload.zero (Suite) | workloadzero.de, bis zur Umstellung <https://workbase.itdone.de> |
| backoffice.zero · workstream.zero · vacancy.zero · jobsearch.zero · coldcall.zero | jeweils `<name>zero.de` (in Vorbereitung) |

## Design-Ressourcen (Figma)

| Datei | Zweck | Link |
|---|---|---|
| Design Tokens | Figma-Variablen (Light/Dark), Sync mit dem Token-Repo | <https://www.figma.com/design/j2RxwrgeeDp9MWTEElzKm3/Design-Tokens> |
| Component Library („🚧 GetITDone-Basic") | Komponenten-Specs, konsumiert das Token-File | <https://www.figma.com/design/bzBnRLfRJNknGg9UYJIHb0/%F0%9F%9A%A7-GetITDone-Basic> |

Details zum Design-System in [design/README.md](./design/README.md).

---

## Inhaltsverzeichnis

### 📐 [`strategy/`](./strategy/) – Strategische Grundlagen
- [Markenarchitektur](./strategy/markenarchitektur.md) – die drei Markenebenen und ihre Aufgaben
- [Geschäftsmodell](./strategy/geschaeftsmodell.md) – wie wir Beratung, Produkt und Betrieb verbinden
- [Portfolio](./strategy/portfolio-bewertung.md) – wie wir unser Portfolio einschätzen und zusammenspielen lassen
- [Roadmap & Priorisierung](./strategy/roadmap.md) – unser Handlungsplan und Gesamtbild

### 🏷️ [`brands/`](./brands/) – Marken
- [WERK](./brands/werk/) – unsere vertikale Produktmarke für industrielle Arbeit
- [ZERO](./brands/zero/) · unsere Produktwelt workload.zero für Dienstleistung, Projekt- und Wissensarbeit

### 📦 [`products/`](./products/) – Produkte
- [WERK Agent](./products/werk-agent/) – unser Leitprodukt für industrielle Datenanalyse
- [WERK Cloud](./products/werk-cloud/) – unsere sichere Betriebsplattform für WERK-Produkte
- [WERK Einsatz](./products/werk-einsatz/) – Service- und Einsatzmanagement (in Validierung)
- [workload.zero](./products/workload-zero/) · modulare Business-Suite mit fünf .zero-Produkten

### 🚀 [`go-to-market/`](./go-to-market/) – Markt & Vertrieb
- [Markt- und Vertriebslogik](./go-to-market/README.md)
- [Marketingpositionierung](./go-to-market/marketing-positionierung.md)
- [Website-Architektur](./go-to-market/website-architektur.md)
- [Unsere Services](./go-to-market/services.md)

### 🎨 [`design/`](./design/) – Marken-Tokens & Design-System
- [Foundations](./design/foundations.md) – geteilte Primitive (Farbe, Typo, Spacing)
- [Themes](./design/themes.md) – semantische Tokens pro Marke

### 🛠️ [`engineering/`](./engineering/) – Technik-Standards
- [Bevorzugter Tech-Stack](./engineering/tech-stack.md) – Next.js/Tailwind/shadcn (FE), NestJS/Prisma (BE)

### 🔬 [`research/`](./research/) – Marktforschung & Analysen
### 🧩 [`templates/`](./templates/) – Vorlagen
### 🗂️ [`decisions/`](./decisions/) – Entscheidungsgrundlagen (ADRs)

---

## Beitragen

Dieses Playbook ist ein lebendes Dokument. Vorschläge und Korrekturen sind willkommen – per Pull Request oder Issue.

## Lizenz

Diese Inhalte stehen unter der [Creative Commons Attribution 4.0 International (CC BY 4.0)](./LICENSE) – Weiterverwendung ist erlaubt, solange Get IT Done GmbH genannt wird.
