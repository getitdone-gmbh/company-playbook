# ADR 0003: Die Kette als Fundament unter Get IT Done

- **Status:** vorgeschlagen
- **Datum:** 2026-10-19
- **Betroffene Bereiche:** Markenarchitektur, Produkte, Go-to-Market, Design

## Kontext

Unsere Markenarchitektur kennt heute zwei Produktwelten: **WERK** für industrielle Arbeit und **ZERO** mit der Suite workload.zero für Dienstleistung, Projekt- und Wissensarbeit ([ADR 0001](./0001-markenarchitektur-werk-work.md), [ADR 0002](./0002-workload-zero-ersetzt-work.md)).

Mit **Die Kette** kommt ein Angebot dazu, das in keine der beiden Welten sauber passt:

- Die Kette ist unsere Design-System-Infrastruktur: Prototyp → Tokens → Figma → Komponenten → Fachkomponenten → Seitenvorlagen → Apps, gepflegt und geprüft von Agenten.
- Sie ist das technische Fundament hinter workload.zero. Alle .zero-Produkte und ihre Landingpages bauen darauf auf.
- Gleichzeitig verkaufen wir Die Kette eigenständig: als Paket für Einzelne und Teams auf [kette.itdone.de](https://kette.itdone.de) und als Dienstleistung, die ein bestehendes Design System in Die Kette überführt ([/ueberfuehrung](https://kette.itdone.de/ueberfuehrung)).
- Ihre Käufer sind weder Werksleitungen (WERK) noch Dienstleister, die eine Business-Suite suchen (ZERO), sondern Entwickler, Produktteams, Designerinnen und Agenturen, die selbst Oberflächen bauen.

Ohne Einordnung bleibt offen, unter welchem Absender Die Kette auftritt, wer für sie verantwortlich ist und ob sie die Grenzen zwischen WERK und ZERO verwischt.

## Entscheidung

Wir schlagen vor, Die Kette als **Fundament direkt unter der Unternehmensmarke Get IT Done** zu führen, neben den Produktwelten WERK und ZERO, aber nicht als dritte Produktwelt mit eigener Dachmarke. Markenauftritt: **Die Kette by Get IT Done**.

```text
Get IT Done GmbH
│
├── WERK   Produktwelt für industrielle Arbeit
├── ZERO   Produktwelt workload.zero
│
└── Fundament (Vorschlag)
    └── Die Kette  Design-System-Infrastruktur, verkettet von Agenten
                   intern Basis von workload.zero, extern als Paket und Überführung verkauft
```

## Begründung

- **Eigener Markt, keine eigene Produktfamilie.** Die Kette spricht Entwickler, Produktteams und Agenturen an. Das ist ein dritter Markt, aber heute nur ein Produkt. Eine dritte Dachmarke mit eigenem Namenssystem, eigenen Domains und eigener Markenpflege wäre zu viel Aufwand für ein Produkt.
- **Die Kette belegt, was Get IT Done kann.** Get IT Done ist laut [Markenarchitektur](../strategy/markenarchitektur.md) Produktentwickler und Technologiepartner. Eine sichtbare, gezählte Infrastruktur zahlt direkt auf diese Unternehmensmarke ein.
- **Der Absender steht schon fest.** Die Live-Seite tritt als "Die Kette by Get IT Done" auf, auf einer Subdomain von itdone.de. Der Vorschlag beschreibt, was im Markt bereits sichtbar ist.
- **Das Fundament ist markenneutral.** Die Kette trägt heute ZERO, sie kann über Themes aber auch WERK-Oberflächen tragen. Unter ZERO würde sie diese Offenheit verlieren.
- **Klare Grenzen bleiben.** WERK und ZERO müssen ihre Botschaften nicht erweitern. workload.zero verkauft weiter eine Business-Suite, Die Kette verkauft Infrastruktur.

**Erwogene Alternativen:**

- *Dritte Produktwelt neben WERK und ZERO:* verworfen für den Moment. Eine Produktwelt rechtfertigt sich erst mit mehreren Produkten für denselben Markt. Wenn aus Die Kette weitere eigenständige Produkte entstehen, prüfen wir das neu.
- *Unter ZERO, etwa als weiteres .zero-Produkt:* verworfen. Die Kette ist kein Arbeitsbereich der Business-Suite, ihre Käufer sind andere, und das .zero-Namenssystem verspricht "ein Problem auf null". Die Kette würde die Suite-Botschaft verwässern.
- *Unter WERK, etwa neben WERK Cloud:* verworfen. Kein Bezug zu industrieller Arbeit, die Kriterien für WERK-Produkte erfüllt Die Kette nicht.
- *Rein intern als Technologie, ohne Verkauf:* verworfen. Die Kette wird bereits eigenständig angeboten, Warteliste läuft.

## Konsequenzen

**Positiv:**

- WERK und ZERO bleiben unverändert und fokussiert.
- Die Kette bekommt einen klaren Absender und einen Platz im Playbook, ohne neue Markenpflege.
- Eine Ebene "Fundament" kann später weitere geteilte Infrastruktur aufnehmen, ohne die Produktwelten anzufassen.
- Die Kette wird zum sichtbaren Beleg für unsere Produktentwicklungskompetenz.

**Negativ / Risiken:**

- Get IT Done tritt damit selbst als Produktabsender auf, nicht nur als Unternehmensrahmen. Wir müssen darauf achten, uns nicht zu breit darzustellen (siehe [Roadmap](../strategy/roadmap.md), Gesamtbild).
- Der Look der Kette ist heute workload.zero. Für Käufer muss klar bleiben, dass das eigene Theme der Weg zur eigenen Marke ist.
- Die Überführung ist eine Dienstleistung mit Personenzeit. Sie konkurriert um Kapazität mit WERK-Services und Produktentwicklung.
- Ändert sich das Bild (mehrere Produkte, eigener Vertrieb), müssen wir die Einordnung erneut entscheiden.

**Entscheidung offen:** Alex entscheidet über Annahme, Änderung oder Ablehnung dieses Vorschlags.
