# workload.zero

**Marke:** [ZERO](../../brands/zero/) · **Priorität:** 3 (eigenständiges SaaS) · **Website:** workloadzero.de (bis zur Umstellung [workbase.itdone.de](https://workbase.itdone.de))

> **workload.zero: die modulare Business-Suite für Unternehmen, Teams und Professionals.**

workload.zero verbindet Arbeit, Menschen und Geschäftsprozesse auf einer gemeinsamen, KI-gestützten Plattform. Das Versprechen: weniger manueller Aufwand rund um die eigentliche Arbeit. Die Suite ist aus Workbase hervorgegangen ([ADR 0002](../../decisions/0002-workload-zero-ersetzt-work.md)). Wir führen sie als eigenständiges digitales SaaS-Geschäft, organisatorisch und finanziell so, dass es unser beratungsintensives WERK-Geschäft nicht ausbremst.

---

## Unsere fünf Produkte

| Produkt | Softwarearten | Zielgruppen |
|---|---|---|
| **backoffice.zero** | ERP-Teilumfang für Dienstleister, WFM, grundlegendes HRIS, Billing/Invoicing | Soloselbständige, Freelancer, Agenturen, Beratungen, IT-Dienstleister, Unternehmen mit Teams |
| **workstream.zero** | Projektmanagement, Kollaboration, Ressourcenmanagement; mit backoffice.zero zusammen PSA | Selbständige mit Projekten, Projektteams, Agenturen, Beratungen, interne Softwareteams |
| **vacancy.zero** | Recruiting mit Kandidaten-CRM, Sourcing, CV-Analyse, Matching; ATS bei vollständigem Prozess | Recruiter, Personal- und Freelancervermittler, In-house-Recruiting |
| **jobsearch.zero** | Talent-/Karriereplattform, CV-Builder, Profil, Job- und Projektmatching | Professionals, Jobsuchende, Freelancer, Consultants |
| **coldcall.zero** | Sales-CRM, Pipeline-Management, Vertriebsaktivitäten | besonders Vermittler und Dienstleister |

Die Produkte sind einzeln nutzbar und arbeiten auf einer gemeinsamen Datenbasis. Gemeinsame Plattformfunktionen: Kontakte, Dokumente, E-Mail, Dashboard, Benachrichtigungen, Rollen, Passkeys, API-Keys, Onboarding, KI inklusive MCP, Import und Schnittstellen.

**Der Kern heute** ist Professional Services Automation (PSA): Ressourcenplanung, Projektarbeit, Zeiterfassung, Abrechnung und Wirtschaftlichkeit, getragen von workstream.zero und backoffice.zero.

## Typische Kombinationen

| Zielgruppe | Produkte |
|---|---|
| Angestellte und Jobsuchende | jobsearch.zero |
| Freelancer und Soloselbständige | backoffice.zero + jobsearch.zero, bei eigener Projektorganisation zusätzlich workstream.zero |
| Agenturen, Beratungen, IT-Dienstleister | workstream.zero + backoffice.zero, bei Personalbedarf vacancy.zero |
| Personal- und Freelancervermittler | vacancy.zero + coldcall.zero, für die eigene Verwaltung backoffice.zero |
| Interne Projekt- und Softwareteams | workstream.zero, Zeiten und Personal über backoffice.zero |

## Was uns stark macht

- **XRechnung und ZUGFeRD:** öffentliche Auftraggeber und zunehmend Unternehmen verlangen strukturierte E-Rechnungen.
- **DATEV-Export:** reduziert Reibung mit Steuerberatern und macht backoffice.zero zu einem Geschäftswerkzeug statt nur zu einem Produktivitätstool.
- **Automatisch aktueller Projekt-CV:** unser potenzielles Alleinstellungsmerkmal. Er entsteht aus Projekten, Rollen, Technologien und Zeiträumen und verbindet workstream.zero, jobsearch.zero und vacancy.zero über dieselben Profildaten.

```text
Projekt gewinnen (coldcall.zero)
      ↓
Arbeit planen und dokumentieren (workstream.zero)
      ↓
Leistung abrechnen (backoffice.zero)
      ↓
Erfahrung automatisch im CV ergänzen (jobsearch.zero)
      ↓
nächstes Projekt oder passende Besetzung finden (vacancy.zero)
```

## Referenzabläufe als Maßstab

Drei Abläufe sollen zuerst vollständig durchlaufbar werden:

1. **Dienstleister:** Verkaufschance → Angebot → Auftrag → Ressourcenplanung → Leistung → Freigabe → Rechnung → Zahlung.
2. **Vermittler:** Kundenbedarf → Kandidatensuche → Vorstellung → Auswahl → Vertrag/Einsatz → Nachweis → Kundenabrechnung und ggf. Freelancer-Vergütung.
3. **Professional:** Profil → passende Gelegenheit → freigegebener CV → Bewerbung/Anfrage → Rückmeldung → Zusage.

## Größte Gaps (P1)

- gemeinsame Stammdaten, durchgängige Workflows, Freigaben und Automatisierung über alle Produkte
- Angebote, Aufträge, Verträge und Übergabe der Konditionen (coldcall.zero + backoffice.zero)
- kaufmännischer Abschluss: Eingangsrechnungen, Zahlungen, Mahnwesen, Liquidität, Buchhaltungs- und Bankanbindung (backoffice.zero)
- vollständiger Bewerbungs- und Vermittlungsprozess bis Placement (vacancy.zero)
- Talentseite mit Gelegenheiten, Bewerbungen, Freigaben und Status (jobsearch.zero)
- Management externer Einsätze: Besetzung, Kapazitäten, Raten, Auslastung, Marge

## Wie wir den Markt sehen

| Was für uns spricht | Was wir im Blick behalten |
|---|---|
| ein Produkt je Problem, eigene Landingpage je Zielgruppe | "Workload" ist in der IT belegt, SEO für die Dachmarke schwerer |
| Self-Service und kurze Kaufentscheidung im Solo-Segment | Suite-Versprechen größer als der heutige PSA-Kern |
| Cross-Selling über die gemeinsame Datenbasis | starker Wettbewerb je Kategorie (PM, CRM, ATS, Buchhaltung) |
| standardisierbares Produkt | niedrige Zahlungsbereitschaft bei Solos, Kündigung zwischen Projekten |
| gute SEO- und Content-Möglichkeiten | hohe Bedeutung von Supporteffizienz |

## Wie wir monetarisieren

| Paket | Zielgruppe | Möglicher Umfang |
|---|---|---|
| **Free / Trial** | Interessenten | ein Produkt, begrenzter Umfang oder Testzeitraum |
| **Solo** | einzelne Professionals | backoffice.zero + jobsearch.zero |
| **Pro** | professionelle Freelancer | zusätzlich workstream.zero, E-Rechnung, DATEV, Automationen |
| **Team** | Dienstleister, Agenturen, Vermittler | Nutzer, Rollen, Freigaben, Planung, Reporting, weitere Produkte je Bedarf |

workload.zero betreiben wir nur dann dauerhaft als eigenständiges Geschäft, wenn Kundengewinnung weitgehend digital funktioniert, der Supportaufwand niedrig bleibt, Aktivierung und Nutzung messbar steigen und wiederkehrende Umsätze die Produktpflege rechtfertigen.

## Wie workload.zero ins Portfolio passt

Der Fit zu unserem industriellen WERK-Geschäft ist **gering**; durch die Markenarchitektur ist das kein Problem.

- **Kein direkter Fit:** andere Märkte, Käufer, Vertriebskanäle und Kaufzyklen.
- **Gemeinsamer Fit auf Unternehmensebene:** technische Komponenten, Cloud-/Betriebsplattform, Authentifizierung, Abrechnungslogik, Produktentwicklungskompetenz, Design- und Engineering-Ressourcen.

## Wie wir workload.zero einschätzen

| Kriterium | Einschätzung |
|---|---|
| Problemstärke | hoch (je Produkt ein klar benannter Schmerz) |
| Zahlungsbereitschaft | Solo niedrig bis mittel, Teams mittel |
| Erklärungsbedarf | je Produkt niedrig, als Suite mittel |
| Vertriebszyklus | Solo kurz, Teams mittel |
| Skalierbarkeit | hoch |
| Cross-Sell mit WERK | niedrig |
| Fit zur Marke ZERO | sehr hoch |
