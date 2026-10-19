# ADR 0003: KETTE wird eigene Marke neben WERK und ZERO

- **Status:** akzeptiert
- **Datum:** 2026-10-19
- **Betroffene Bereiche:** Markenarchitektur, Produkte, Go-to-Market, Design
- **Vorgeschichte:** Der erste Vorschlag dieses ADR sah Die Kette als "Fundament" unter Get IT Done vor. Er ist unten als verworfene Alternative festgehalten.

## Kontext

Unsere Markenarchitektur kannte bisher zwei Produktwelten: **WERK** für industrielle Arbeit und **ZERO** mit der Suite workload.zero für Dienstleistung, Projekt- und Wissensarbeit ([ADR 0001](./0001-markenarchitektur-werk-work.md), [ADR 0002](./0002-workload-zero-ersetzt-work.md)).

Mit **Die Kette** kommt ein Angebot dazu, das in keine der beiden Welten passt:

- Die Kette ist unsere Design-System-Infrastruktur: Prototyp → Tokens → Figma → Komponenten → Fachkomponenten → Seitenvorlagen → Apps, gepflegt und geprüft von Agenten.
- Sie ist das technische Fundament hinter workload.zero. Alle .zero-Produkte und ihre Landingpages bauen darauf auf.
- Gleichzeitig verkaufen wir Die Kette eigenständig: als Paket für Einzelne und Teams auf [kette.itdone.de](https://kette.itdone.de), als kleinere Pakete (Agenten-Pack, Design-Review-Pack) und als Dienstleistung, die ein bestehendes Design System in Die Kette überführt ([/ueberfuehrung](https://kette.itdone.de/ueberfuehrung)).
- Ihre Käufer sind weder Werksleitungen (WERK) noch Dienstleister, die eine Business-Suite suchen (ZERO), sondern Entwickler, Produktteams, Agenturen und Firmen mit bestehendem Design System.

Ohne Einordnung bliebe offen, unter welchem Absender Die Kette auftritt, wer für sie verantwortlich ist und ob sie die Grenzen zwischen WERK und ZERO verwischt.

## Entscheidung

**KETTE wird eigene Marke neben WERK und ZERO.** Damit erweitern wir unsere Produktpalette um eine dritte Produktwelt für Design-System-Infrastruktur. Das erste und zentrale Produkt heißt **Die Kette**. Details unter [`brands/kette/`](../brands/kette/).

```text
Get IT Done GmbH
│
├── WERK    Produktwelt für industrielle Arbeit
├── ZERO    Produktwelt workload.zero
└── KETTE   Produktwelt für Design-System-Infrastruktur
    ├── Die Kette            komplette Design-System-Infrastruktur (eine Person / Team)
    ├── Agenten-Pack
    ├── Design-Review-Pack
    ├── Überführung          Dienstleistung, auf Anfrage
    ├── öffentliche Storybooks und Prototyp als Schaufenster
    └── weitere KETTE-Produkte
```

**Schreibweise:** Die Marke heißt **KETTE**, in Versalien wie WERK und ZERO. Das Produkt heißt **Die Kette**.

## Begründung

- **Wir erweitern unsere Produktpalette.** Alex hat entschieden, KETTE als eigene Marke zu führen. Aus der Kette entstehen schon heute mehrere verkaufbare Angebote (Die Kette, Agenten-Pack, Design-Review-Pack, Überführung). Eine eigene Marke gibt diesen Angeboten und künftigen KETTE-Produkten ein gemeinsames Dach.
- **Eigener Markt.** KETTE spricht Entwickler, Produktteams, Agenturen und Firmen mit bestehendem Design System an. Das ist ein dritter Markt mit eigenen Käufern, eigener Botschaft und eigenem Vertrieb. Das entspricht unserem Leitgedanken: getrennte Märkte, Botschaften und Vertriebssysteme.
- **Klare Grenzen zu WERK und ZERO.** workload.zero verkauft eine Business-Suite, KETTE verkauft die Infrastruktur, mit der man solche Apps baut. WERK bleibt unberührt.
- **ZERO als Referenz und Beweis.** ZERO läuft auf KETTE. Jede .zero-Oberfläche belegt, was KETTE leistet, ohne dass ZERO seine Botschaft erweitern muss.
- **Markenneutral nach innen.** KETTE trägt heute ZERO und kann über Themes auch WERK-Oberflächen tragen. Als eigene Marke behält sie diese Offenheit.

**Erwogene Alternativen:**

- *Die Kette als Fundament direkt unter Get IT Done (ursprünglicher Vorschlag "Fundament"):* verworfen. Der Vorschlag sah eine Ebene "Fundament" ohne eigene Dachmarke vor, Markenauftritt "Die Kette by Get IT Done", weil Die Kette damals ein Produkt war und eine dritte Dachmarke als zu viel Markenpflege galt. Alex will die Produktpalette erweitern. Dafür braucht es eine Marke, unter der weitere Produkte wachsen können, nicht eine Infrastrukturebene ohne eigenen Auftritt.
- *Unter ZERO, etwa als weiteres .zero-Produkt:* verworfen. Die Kette ist kein Arbeitsbereich der Business-Suite, ihre Käufer sind andere, und das .zero-Namenssystem verspricht "ein Problem auf null". Die Kette würde die Suite-Botschaft verwässern.
- *Unter WERK, etwa neben WERK Cloud:* verworfen. Kein Bezug zu industrieller Arbeit, die Kriterien für WERK-Produkte erfüllt Die Kette nicht.
- *Rein intern als Technologie, ohne Verkauf:* verworfen. Die Kette wird bereits eigenständig angeboten, die Warteliste läuft.

## Konsequenzen

**Positiv:**

- KETTE bekommt einen klaren Absender, eine eigene Botschaft und Platz für weitere Produkte.
- WERK und ZERO bleiben unverändert und fokussiert.
- ZERO wird zum laufenden Beleg für KETTE, KETTE zum sichtbaren Beleg für unsere Produktentwicklungskompetenz.

**Negativ / Risiken:**

- Eine dritte Marke bedeutet mehr Markenpflege: eigene Botschaften, eigene Kennzahlen, eigener Auftritt. Wir müssen darauf achten, uns nicht zu breit darzustellen (siehe [Roadmap](../strategy/roadmap.md), Gesamtbild).
- Der Look von Die Kette ist heute workload.zero. Für Käufer muss klar bleiben, dass das eigene Theme der Weg zur eigenen Marke ist.
- Die Überführung ist eine Dienstleistung mit Personenzeit. Sie konkurriert um Kapazität mit WERK-Services und Produktentwicklung.
- Markenprüfung und Domainstrategie für KETTE stehen noch aus. Heute läuft der Auftritt auf Subdomains von itdone.de.

## Offene Frage: Benennung von Storybooks und Produkten unter KETTE

Nicht entschieden. Wir halten die Frage hier fest, die Entscheidung trifft Alex.

Sollen die öffentlichen Storybooks und Produkte künftig unter KETTE benannt werden? Ein möglicher Schnitt:

| Heute | Vorschlag | Begründung |
|---|---|---|
| Get IT Done · Components | **KETTE · Components** | die Komponenten-Library ist eine Station der Kette und gehört zur Marke KETTE |
| ZERO · Components | bleibt **ZERO · Components** | Fachkomponenten von ZERO, fachlich an die Suite gebunden |
| ZERO · Pages | bleibt **ZERO · Pages** | Seitenvorlagen von ZERO, fachlich an die Suite gebunden |

Zu klären ist dabei auch, ob die Domains (components.itdone.de) und Paketnamen folgen oder nur der sichtbare Titel wechselt.
