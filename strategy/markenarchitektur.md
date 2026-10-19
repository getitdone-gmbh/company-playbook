# Markenarchitektur

Unsere strategische Grundentscheidung steht: Wir führen drei getrennte Produktwelten, **WERK**, **ZERO** und **KETTE**, unter einer gemeinsamen Unternehmens- und Technologiebasis. ZERO hat mit [ADR 0002](../decisions/0002-workload-zero-ersetzt-work.md) die frühere Marke WORK abgelöst. KETTE ist mit [ADR 0003](../decisions/0003-kette-eigene-marke.md) als eigene Marke dazugekommen, damit erweitern wir unsere Produktpalette.

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
├── ZERO · Dachmarke workload.zero
│   Modulare Business-Suite für Unternehmen, Teams und Professionals
│   │
│   ├── backoffice.zero
│   ├── workstream.zero
│   ├── vacancy.zero
│   ├── jobsearch.zero
│   └── coldcall.zero
│
└── KETTE
    Design-System-Infrastruktur, verkettet von Agenten
    │
    ├── Die Kette            komplette Design-System-Infrastruktur (eine Person / Team)
    ├── Agenten-Pack
    ├── Design-Review-Pack
    ├── Überführung          Dienstleistung, auf Anfrage
    ├── öffentliche Storybooks und Prototyp als Schaufenster
    └── weitere KETTE-Produkte
```

ZERO läuft auf KETTE: workload.zero und alle .zero-Produkte bauen auf der Kette auf und dienen KETTE als Referenz und Beweis.

Damit trennen wir bewusst drei unterschiedliche Märkte:

| Marke | Markt | Nutzer | Käufer | Vertriebsmodell |
|---|---|---|---|---|
| **WERK** | Fertigung und industrielle Dienstleistungen | Ingenieure, Technologen, Service- und Produktionsmitarbeiter | Werksleitung, COO, Serviceleitung, IT/OT | beratungsnaher B2B-Vertrieb |
| **ZERO** | Dienstleister, Vermittler, Freelancer, Projektteams, Unternehmen mit Teams | Freelancer, Berater, Projektteams, Recruiter, Vertrieb, Verwaltung, Professionals | Solo: der Nutzer selbst; Teams: Geschäfts- oder Bereichsleitung | Self-Service, Product-led Growth, SEO je Produkt-Landingpage |
| **KETTE** | Entwickler, Produktteams, Agenturen und Firmen mit bestehendem Design System | Entwickler mit Claude Code, Freelancer, Designer in Produktteams | Einzelne: der Nutzer selbst; Teams: CTO oder Lead Frontend; Agenturen: Geschäftsführung | Self-Service mit Warteliste, Überführung als Dienstleistung auf Anfrage |
| **Get IT Done** | übergreifender Unternehmensrahmen | Management, Partner und Bestandskunden | Geschäftsführung, IT-Leitung, Fachbereiche | Beratung, Implementierung und Betrieb |

Diese Trennung löst unser früheres Portfolio-Problem: workload.zero muss nicht künstlich auf die Fertigungspositionierung einzahlen, und WERK müssen wir nicht so breit formulieren, dass auch Dienstleister und Freelancer darunterpassen. Die Grenze verläuft über den Markt: industrielle Arbeit (WERK), Dienstleistung, Projekt- und Wissensarbeit (ZERO) und Menschen, die selbst Oberflächen bauen oder ein Design System pflegen (KETTE).

> **Unser Leitgedanke: Gemeinsames Unternehmen und gemeinsame Technologie – aber getrennte Märkte, Botschaften und Vertriebssysteme.**

> Die zugrunde liegenden Entscheidungen dokumentieren wir in [ADR 0001](../decisions/0001-markenarchitektur-werk-work.md), [ADR 0002](../decisions/0002-workload-zero-ersetzt-work.md) und [ADR 0003](../decisions/0003-kette-eigene-marke.md).

---

## Die Aufgaben unserer Markenebenen

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

Wir erklären auf der Startseite nicht alle Leistungen gleichrangig. Stattdessen führen wir zu unseren drei klaren Produktwelten:

- **WERK – für Industrie und Produktion**
- **workload.zero: für Dienstleister, Teams und Professionals**
- **KETTE: für alle, die Oberflächen bauen und ein Design System pflegen**

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

### KETTE

KETTE ist unsere Produktwelt für Design-System-Infrastruktur: Prototyp → Tokens → Figma → Komponenten → Fachkomponenten → Seitenvorlagen → Apps, gepflegt und geprüft von Agenten. Details unter [`brands/kette/`](../brands/kette/) und [`products/die-kette/`](../products/die-kette/).

> **Deine Design-System-Infrastruktur. Verkettet von Agenten.**

**Unsere Produktlogik:**

- **Die Kette:** die komplette Infrastruktur, für eine Person oder ein Team
- **Agenten-Pack** und **Design-Review-Pack:** kleinere Einstiege
- **Überführung:** bestehende Design Systems an Die Kette hängen, als Dienstleistung auf Anfrage
- **Schaufenster:** öffentliche Storybooks und Prototyp als nachprüfbarer Beleg

**Schreibweise:** Marke **KETTE** in Versalien wie WERK und ZERO, Produktname **Die Kette**.

**Verhältnis zu ZERO:** ZERO läuft auf KETTE und dient als Referenz und Beweis. workload.zero verkauft eine Business-Suite, KETTE verkauft die Infrastruktur, mit der man solche Apps baut. WERK bleibt unberührt.

Ein Produkt nehmen wir in KETTE auf, wenn es mindestens drei der Kriterien aus [`brands/kette/`](../brands/kette/) erfüllt.
