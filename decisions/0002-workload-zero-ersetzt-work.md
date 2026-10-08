# ADR 0002: ZERO ersetzt WORK, Workbase wird zur Suite workload.zero

- **Status:** akzeptiert
- **Datum:** 2026-10-08
- **Betroffene Bereiche:** Markenarchitektur, Produkte, Go-to-Market, Design
- **Ersetzt teilweise:** [ADR 0001](./0001-markenarchitektur-werk-work.md) (der Teil zu WORK; WERK bleibt unverändert)

## Kontext

Mit ADR 0001 haben wir WERK und WORK getrennt. WORK war als Marke für IT-Freelancer gedacht, mit Workbase als einzigem Produkt. Workbase ist inzwischen deutlich breiter als ein Freelancer-Werkzeug: Es deckt kaufmännische Verwaltung, Projektarbeit, Recruiting, Karriere und Vertrieb ab und richtet sich an Dienstleister, Vermittler, Freelancer, Projektteams und Unternehmen mit Teams.

Die Marke WORK und der Name Workbase bilden das nicht ab. Workbase ist außerdem noch keine bekannte Marke, eine Umbenennung kostet uns also kaum Markenbekanntheit.

## Entscheidung

Wir ersetzen die Produktwelt **WORK** durch **ZERO** mit der Dachmarke **workload.zero**, der modularen Business-Suite für Unternehmen, Teams und Professionals. Workbase geht vollständig darin auf. Die Umstellung erfolgt in einem Schritt.

**WERK** (WERK Agent, WERK Cloud, perspektivisch WERK Einsatz) bleibt vorerst unverändert.

### Produkte von workload.zero

| Produkt | Bisher | Arbeitsbereich |
|---|---|---|
| **backoffice.zero** | Workbase (Zeiten, Personal, Abrechnung) | Kaufmännische Verwaltung, WFM, HRIS, Billing |
| **workstream.zero** | Workbase (Projekte, Ressourcen, Zusammenarbeit) | Projektmanagement und Ressourcenplanung |
| **vacancy.zero** | Arbeitsname sourcing.zero | Recruiting, Kandidaten-CRM, ATS/Placement |
| **jobsearch.zero** | Workbase (Profile, CV) | Talent- und Karriereplattform, CV-Builder |
| **coldcall.zero** | Arbeitsname acquisition.zero | Sales-CRM, Pipeline, Kundengewinnung |

### Namens- und Domainregeln

- Alle Produkte tragen die Form `<name>.zero`. Wo der Name das nervigste Problem der Zielgruppe benennt (vacancy, coldcall), ist er gleichzeitig das Versprechen. Wo der Arbeitsbereich klarer ist, benennt er den Bereich (backoffice, workstream, jobsearch).
- `.zero` ist keine echte Domain-Endung. Die Web-Adresse lautet `<name>zero.de` (zusätzlich .io, .com sofern verfügbar).
- Jedes Produkt bekommt eine eigene Domain und eine eigene Landingpage. Die Suite läuft unter workloadzero.de.
- Markenauftritt: **workload.zero by Get IT Done**, Produkte als "backoffice.zero · part of workload.zero".

## Begründung

- Die Suite-Positionierung (ERP-, CRM-, Projekt-, Personal- und Talentfunktionen auf einer Datenbasis) passt zum tatsächlichen Funktionsumfang besser als "Betriebssystem für IT-Freelancer".
- Die `.zero`-Familie lässt sich um weitere Arbeitsbereiche erweitern, ohne die Markenarchitektur erneut anzufassen.
- "zero" transportiert das gemeinsame Versprechen: weniger manueller Aufwand durch Automatisierung.

**Erwogene Alternativen:**
- *Workbase behalten und erweitern:* verworfen, der Name trägt keine Suite und ist nicht bekannt.
- *Schrittweise Umbenennung:* verworfen, zwei parallele Marken würden Kunden verwirren.
- *Alternative Dachmarke "Zero by Get IT Done":* als Rückfalloption notiert.

## Konsequenzen

**Positiv:**
- eine Dachmarke mit klarem Versprechen und erweiterbarer Produktfamilie
- eigene Landingpages je Produkt ermöglichen gezieltes SEO und eigene Zielgruppenansprache
- WERK bleibt fokussiert und wird nicht berührt

**Negativ / Risiken:**
- "Workload" ist in der IT (Kubernetes, Zero Trust) belegt; SEO für die Dachmarke ist schwerer
- das Suite-Versprechen ist größer als der heutige PSA-Kern; Gaps (ERP-Abschluss, ATS, durchgängige Automatisierung) müssen sichtbar geschlossen werden
- Aufwand für die Umstellung: Apps im App Store, MCP-Connector, E-Mail-Absender, Rechnungsvorlagen, Design-Theme, Weiterleitung von workbase.itdone.de
- Markenprüfung (DPMA, EUIPO, WIPO, Klassen 9, 35, 42) und Domainsicherung stehen noch aus
- die Zielgruppe reicht jetzt bis zu Unternehmen mit Teams; die Abgrenzung zu WERK erfolgt über den Markt (Dienstleistung und Wissensarbeit vs. Industrie), nicht mehr über "Freelancer vs. Unternehmen"
