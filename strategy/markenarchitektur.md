# Markenarchitektur

Unsere strategische Grundentscheidung steht: Wir führen zwei getrennte Produktwelten, **WERK** und **ZERO**, unter einer gemeinsamen Unternehmens- und Technologiebasis. ZERO hat mit [ADR 0002](../decisions/0002-workload-zero-ersetzt-work.md) die frühere Marke WORK abgelöst.

```text
Get IT Done GmbH
│
├── WERK
│   Software und Services für Fertigung, Produktion und industrielle Arbeit
│
│   ├── WERK Agent
│   ├── WERK Cloud
│   ├── WERK Einsatz – potenzielles eigenständiges Industrieprodukt
│   └── weitere vertikale WERK-Produkte
│
└── ZERO · Dachmarke workload.zero
    Modulare Business-Suite für Unternehmen, Teams und Professionals
    │
    ├── backoffice.zero
    ├── workstream.zero
    ├── vacancy.zero
    ├── jobsearch.zero
    └── coldcall.zero
```

**Vorschlag ([ADR 0003](../decisions/0003-die-kette-als-fundament.md), Status vorgeschlagen):** Unter Get IT Done kommt neben WERK und ZERO eine Ebene **Fundament** dazu. Sie ist keine dritte Produktwelt, sondern trägt geteilte Infrastruktur, die wir auch eigenständig verkaufen. Heute liegt dort nur **Die Kette**.

```text
Get IT Done GmbH
│
├── WERK
├── ZERO · Dachmarke workload.zero
│
└── Fundament (Vorschlag)
    └── Die Kette
        Design-System-Infrastruktur, verkettet von Agenten
        Basis von workload.zero, eigenständig als Paket und Überführung verkauft
```

Damit trennen wir bewusst zwei unterschiedliche Märkte:

| Marke | Markt | Nutzer | Käufer | Vertriebsmodell |
|---|---|---|---|---|
| **WERK** | Fertigung und industrielle Dienstleistungen | Ingenieure, Technologen, Service- und Produktionsmitarbeiter | Werksleitung, COO, Serviceleitung, IT/OT | beratungsnaher B2B-Vertrieb |
| **ZERO** | Dienstleister, Vermittler, Freelancer, Projektteams, Unternehmen mit Teams | Freelancer, Berater, Projektteams, Recruiter, Vertrieb, Verwaltung, Professionals | Solo: der Nutzer selbst; Teams: Geschäfts- oder Bereichsleitung | Self-Service, Product-led Growth, SEO je Produkt-Landingpage |
| **Die Kette** (Fundament, Vorschlag) | Entwickler, Produktteams und Agenturen, die selbst Oberflächen bauen | Entwickler mit Claude Code, Freelancer, Designer in Produktteams | Einzelne: der Nutzer selbst; Teams: CTO oder Lead Frontend; Agenturen: Geschäftsführung | Self-Service mit Warteliste, Überführung als Dienstleistung auf Anfrage |
| **Get IT Done** | übergreifender Unternehmensrahmen | Management, Partner und Bestandskunden | Geschäftsführung, IT-Leitung, Fachbereiche | Beratung, Implementierung und Betrieb |

Diese Trennung löst unser früheres Portfolio-Problem: workload.zero muss nicht künstlich auf die Fertigungspositionierung einzahlen, und WERK müssen wir nicht so breit formulieren, dass auch Dienstleister und Freelancer darunterpassen. Die Grenze verläuft über den Markt: industrielle Arbeit (WERK) gegenüber Dienstleistung, Projekt- und Wissensarbeit (ZERO).

> **Unser Leitgedanke: Gemeinsames Unternehmen und gemeinsame Technologie – aber getrennte Märkte, Botschaften und Vertriebssysteme.**

> Die zugrunde liegenden Entscheidungen dokumentieren wir in [ADR 0001](../decisions/0001-markenarchitektur-werk-work.md) und [ADR 0002](../decisions/0002-workload-zero-ersetzt-work.md).

---

## Die Aufgaben unserer drei Markenebenen

### Get IT Done GmbH

**Website:** <https://itdone.de>

Get IT Done ist unsere Unternehmens-, Kompetenz- und Vertrauensmarke.

**Aufgaben:**

- rechtlicher Anbieter
- Arbeitgeber
- Technologie- und Umsetzungspartner
- Produktentwickler
- Beratungs- und Implementierungseinheit
- Betreiber von Cloud- und KI-Lösungen
- Partner für individuelle Integrationen

**Wie wir kommunizieren:**

> **Wir entwickeln und betreiben digitale Produkte für industrielle Unternehmen, Dienstleister und Professionals.**

Wir erklären auf der Startseite nicht alle Leistungen gleichrangig. Stattdessen führen wir zu unseren zwei klaren Produktwelten:

- **WERK – für Industrie und Produktion**
- **workload.zero: für Dienstleister, Teams und Professionals**

### WERK

WERK ist unsere vertikale Produktmarke für Fertigung, Produktion und industrielle Dienstleistungen. Details unter [`brands/werk/`](../brands/werk/).

> **Unser Markenversprechen: WERK digitalisiert industrielle Arbeit – von der Koordination der Menschen über die Analyse der Anlagendaten bis zum sicheren Betrieb der Anwendungen.**

**Unsere Produktlogik:**

- **WERK Agent:** Daten verstehen
- **WERK Einsatz:** Arbeit koordinieren
- **WERK Cloud:** Anwendungen und KI sicher betreiben

Ein Produkt nehmen wir in WERK auf, wenn es mindestens **drei** dieser Kriterien erfüllt:

1. Es löst ein Problem in Produktion, Instandhaltung, Service oder Engineering.
2. Seine Nutzer arbeiten mit Maschinen, Anlagen oder industriellen Prozessen.
3. Seine Käufer sitzen in Operations, Produktion, Service, IT oder OT.
4. Es nutzt industrielle Daten oder industrielle Workflows.
5. Es lässt sich sinnvoll mit mindestens einem anderen WERK-Produkt verbinden.

### ZERO

ZERO ist unsere Produktwelt für Dienstleistung, Projekt- und Wissensarbeit. Dachmarke ist **workload.zero**. Details unter [`brands/zero/`](../brands/zero/) und [`products/workload-zero/`](../products/workload-zero/).

> **Unser Markenversprechen: workload.zero nimmt die Arbeit rund um die eigentliche Arbeit ab. Durch gemeinsame Informationen, durchgängige Abläufe und Automatisierung.**

**Unsere Produktlogik:** Jedes Produkt trägt die Form `<name>.zero` und hat eine eigene Domain (`<name>zero.de`) und Landingpage.

- **backoffice.zero:** Verwaltung und Abrechnung
- **workstream.zero:** Projekte und Ressourcen
- **vacancy.zero:** Stellen und Projektbedarfe besetzen
- **jobsearch.zero:** Profil, CV und passende Gelegenheiten
- **coldcall.zero:** Kunden gewinnen ohne Kaltakquise

Ein neues Produkt nehmen wir in workload.zero auf, wenn es einen eigenen Arbeitsbereich mit eigener Zielgruppe abdeckt, auf der gemeinsamen Datenbasis arbeitet und mit mindestens einem bestehenden .zero-Produkt durchgängige Abläufe bildet.

### Fundament: Die Kette (Vorschlag)

Die Kette ist unsere Design-System-Infrastruktur: Prototyp → Tokens → Figma → Komponenten → Fachkomponenten → Seitenvorlagen → Apps, gepflegt und geprüft von Agenten. Details unter [`products/die-kette/`](../products/die-kette/).

> **Deine Design-System-Infrastruktur. Verkettet von Agenten.**

**Warum ein Fundament und keine Produktwelt:** Die Kette trägt workload.zero technisch und wird zugleich an einen eigenen Markt verkauft (Entwickler, Produktteams, Agenturen). Für eine eigene Dachmarke ist sie heute ein Produkt zu wenig, unter WERK oder ZERO würde sie deren Botschaften verwässern. Markenauftritt: **Die Kette by Get IT Done**.

**Abgrenzung:** workload.zero verkauft eine Business-Suite, Die Kette verkauft die Infrastruktur, mit der man solche Apps baut. WERK bleibt unberührt.

Ob wir diese Einordnung übernehmen, ist offen. Die Entscheidung trifft Alex über [ADR 0003](../decisions/0003-die-kette-als-fundament.md).
