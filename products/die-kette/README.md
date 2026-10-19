# Die Kette

**Marke:** [KETTE](../../brands/kette/) ([ADR 0003](../../decisions/0003-kette-eigene-marke.md)) · **Priorität:** in Einführung, Warteliste · **Website:** [kette.itdone.de](https://kette.itdone.de)

> **Deine Design-System-Infrastruktur. Verkettet von Agenten.**

Die Kette ist das zentrale Produkt der Marke KETTE: unser Design System für komplexe Business-Apps, verbunden zu einer durchgängigen Kette und gepflegt von Agenten für Claude Code. Sie ist die Basis, auf der workload.zero läuft, und wir verkaufen sie eigenständig: als Paket zum Selbstnutzen und als Überführung bestehender Design Systems.

---

## Die Kette in sieben Stationen

```text
Prototyp → Tokens → Figma → Komponenten → Fachkomponenten → Seitenvorlagen → Apps
```

Jede Änderung fließt in eine Richtung und wird an jeder Station geprüft. Der Wert liegt nicht im einzelnen Glied, sondern in der Verbindung: Eine Änderung an einem Token kommt in Figma, in den Komponenten, in den Seitenvorlagen und in den Apps an.

| Station | Was dort liegt |
|---|---|
| **Prototyp** | interaktiver Prototyp von workload.zero, Vorlage für Abläufe und Zustände |
| **Tokens** | ein Token-Repo als einzige Quelle für Farbe, Typografie und Abstände, hell und dunkel |
| **Figma** | Figma-Dateien, deren Variablen aus den Tokens gespeist werden |
| **Komponenten** | React-Komponentenbibliothek auf Radix-Basis, mit Storybook und Tests |
| **Fachkomponenten** | Fachkomponenten für Business-Apps (zero), gebaut auf der Library |
| **Seitenvorlagen** | fertige Seiten mit allen Zuständen (Zero Pages), man schließt nur die Business-Logik an |
| **Apps** | Anwendungen und Landingpages, die auf der Kette laufen, darunter workload.zero |

Dahinter steht ein gesteuerter Loop von Agenten: Anforderung, UX, UI, Bau, danach sechs unabhängige Prüfungen (QA, Barrierefreiheit, Material, Design-Review, Sicherheit, Performance). Befunde gehen an den Verursacher zurück, nicht pauschal an den Entwickler.

## Für wen wir es bauen

**Hauptanwender:**

- Entwickler, die Claude Code intensiv nutzen und Produkte allein oder für Kunden bauen
- Freelance-Entwickler und -Designer mit Festpreisprojekten
- Gründer, die mit KI ihre erste App bauen und nicht nach Standard-Template aussehen wollen
- UX- und UI-Designer in Produktteams, die Figma und Code zusammenhalten müssen

**Wirtschaftliche Käufer:**

- Einzelne: entscheiden selbst, kaufen per Karte
- CTO oder Lead Frontend in B2B-SaaS-Firmen mit kleinen Entwicklerteams, ohne eigenes Design-System-Team
- Technical Director oder Geschäftsführung von Digitalagenturen mit vielen Kundenmarken
- Firmen mit bestehendem Design System über mehrere Apps oder Marken (Überführung)

**Technische Entscheider:** Lead Frontend, Tech Lead, Design-System-Verantwortliche. Über ein Design System entscheidet meist das Team, deshalb sind öffentliche Storybooks und der Prototyp wichtig zum Weiterreichen.

## Welches Problem wir lösen

KI baut Oberflächen schnell, aber nach Gefühl. Der Agent meldet "fertig" und prüft sich selbst. Kontrast, Fokus und Zustände fehlen, und keiner merkt es. Gratis-Skills geben Stil vor, setzen aber nichts durch.

Dazu kommen die alten Probleme jedes Design Systems:

- Figma und Code laufen auseinander, besonders bei hell, dunkel und mehreren Marken.
- Das System aktuell zu halten kostet viel Handarbeit, irgendwann verliert man den Überblick.
- Tabellen, Formulare und Zeitraster werden in jedem Projekt neu gebaut. Kits liefern Breite und hören bei der Fachlogik auf.

## Warum der Fit stark ist

- **Gewachsen statt für den Verkauf gebaut.** Die Kette ist seit Oktober 2023 in echten Projekten entstanden und trägt heute unsere eigenen Apps. Seit 2026 arbeiten wir mit agentischer Unterstützung.
- **Ein Durchstich statt einzelner Teile.** Andere verkaufen ein UI-Kit, eine Figma-Datei oder ein Skill-Paket. Die Kette verbindet alle Stationen von Prototyp bis App.
- **Die Agenten pflegen, was sie gebaut haben.** Dieselben Agenten, die die Kette aufgebaut und geprüft haben, sind Teil des Pakets.
- **Fachtiefe für datenlastige Apps.** Fachkomponenten und Seitenvorlagen mit Zuständen decken genau das ab, was generische Kits auslassen.
- **Belege statt Versprechen.** Jede Zahl auf der Seite ist aus unseren Repos gezählt, auch die unbequemen, zum Beispiel offen benannte Audit-Befunde.

### Gezählt auf kette.itdone.de (Stand 18.10.2026)

| Bereich | Umfang |
|---|---|
| Kette | 6 Repos, 14 Figma-Dateien, 13 Pipelines mit automatischen npm-Releases |
| Tokens | 1.564 Tokens, 40 Theme-Dateien |
| Library | 145 Komponenten, 2.485 Tests, Barrierefreiheit je Story geprüft |
| Fachkomponenten | 100 Fachkomponenten, 981 Stories |
| Seitenvorlagen | 18 Vorlagen mit 394 Zuständen |
| Agenten | 26 Agenten, 18 Skills, 132 Regeln und 52 Do/Don't-Paare |
| Historie | 2.020 Commits in 6 Repos, 218 Releases, erster Commit im Oktober 2023 |

## Wie wir den Ablauf verändern

**Problem:** Ein Team baut mit Claude Code Oberflächen. Jede sieht anders aus, Figma und Code driften, und am Ende ist der Mensch das einzige Gate.

**Mit Die Kette:**

1. Tokens sind die einzige Quelle, Figma und Code werden daraus gespeist.
2. Neue Oberflächen entstehen aus Komponenten, Fachkomponenten und Seitenvorlagen statt aus Eigenbau.
3. Ein Loop führt jede Änderung von der Anforderung bis zum Release.
4. Sechs unabhängige Prüfungen nehmen ab, Befunde gehen mit Beleg an die Ursache.
5. Releases, Figma-Sync und visuelle Regressionstests laufen automatisch.

**Wer schon ein Design System hat**, baut nicht neu. Bei der [Überführung](https://kette.itdone.de/ueberfuehrung) hängen wir Tokens, Figma-Dateien und Repos Stufe für Stufe an Die Kette: Bestandsaufnahme, Tokens, Figma, Repos, Apps, Betrieb. Alt und Neu laufen parallel, bis das Alte weg ist. Auf Wunsch laufen die meisten Agenten auf eigener Hardware beim Kunden.

## Wie wir uns differenzieren

- Durchgängige Kette von Prototyp bis App statt Einzelteile
- Agenten mit unabhängigen Prüfungen und Befund-Routing an die Ursache
- Fachkomponenten und Seitenvorlagen für Business-Apps, nicht nur Basiskomponenten
- Öffentliche Storybooks und ein öffentlicher Prototyp als nachprüfbarer Beleg
- Ehrliche Grenzen, offen kommuniziert (siehe unten)

## Was Die Kette nicht ist

- Kein Nachweis für Barrierefreiheit nach BFSG oder BITV. Die Agenten prüfen nach WCAG 2.2 AA und melden Befunde mit Beleg.
- Die Agenten laufen nur mit Claude Code. Tokens, Library, Figma-Dateien und Vorlagen lassen sich auch ohne nutzen.
- Beim Paket gibt es keinen persönlichen Support. Persönliche Zusammenarbeit gibt es bei der Überführung.
- Der Look ist workload.zero. Die eigene Marke entsteht über ein eigenes Theme.

## Wie wir Geld verdienen

**Unsere Erlösbausteine:**

| Angebot | Preis | Für wen |
|---|---|---|
| **Die Kette** | 249 € einmalig, inkl. MwSt., 12 Monate Updates | eine Person |
| **Team** | 990 € zzgl. MwSt. | Teams bis 10 Personen |
| **Kleine Pakete** | ab 49 € (Design-Review-Pack 49 €, Agenten-Pack 149 €) | Einstieg für Einzelne |
| **Agenturen** | auf Anfrage | Agenturen mit Kundenprojekten |
| **Überführung** | auf Anfrage, nach der Bestandsaufnahme ein Festpreis | Firmen mit bestehendem Design System |

**Status:** Warteliste. Verkaufsstart am **01.11.2026**.

Die Überführung ist der einzige Weg mit Personenzeit. Jedes Überführungsprojekt enthält die Teamlizenz Die Kette, damit der Kunde den Betrieb mit denselben Agenten selbst führen kann. Wer den Betrieb nicht selbst führen will, bucht ihn monatlich bei uns.

## Wie wir Die Kette einschätzen

Arbeitsstand. Noch ohne Verkäufe, also ohne Beleg aus dem Markt.

| Kriterium | Einschätzung |
|---|---|
| Problemstärke | hoch (Qualität von KI-Oberflächen, Drift zwischen Figma und Code) |
| Zahlungsbereitschaft | Einzelne niedrig bis mittel, Teams und Agenturen mittel, Überführung hoch |
| Erklärungsbedarf | Paket mittel, Überführung hoch |
| Vertriebszyklus | Paket kurz (Self-Service), Überführung mittel bis lang |
| Skalierbarkeit | Paket sehr hoch, Überführung niedrig |
| Markenfit | Kernprodukt von KETTE; ZERO läuft darauf und dient als Referenz; kein Bezug zu WERK |

## Links

| Was | Wo |
|---|---|
| Verkaufsseite und Warteliste | <https://kette.itdone.de> |
| Überführung bestehender Design Systems | <https://kette.itdone.de/ueberfuehrung> |
| Storybook Komponenten (Library) | <https://components.itdone.de> |
| Storybook Fachkomponenten (zero) | <https://zero.itdone.de> |
| Storybook Seitenvorlagen (Zero Pages) | <https://zero-pages.itdone.de> |
| Interaktiver Prototyp workload.zero | <https://zero-design.itdone.de> |

Alle Oberflächen dort zeigen fiktive Beispieldaten. Mehr zum Design System in [design/README.md](../../design/README.md).
