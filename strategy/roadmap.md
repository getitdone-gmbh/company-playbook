# Roadmap & Priorisierung

Unser Handlungsplan in fünf Phasen, unsere Prioritäten und das Gesamtbild.

## Unser Handlungsplan

### Phase 1: Marken und Botschaften schärfen

1. Wir dokumentieren WERK, ZERO (workload.zero, ersetzt WORK, siehe ADR 0002) und KETTE (siehe ADR 0003) als verbindliche Produktwelten.
2. Wir legen Claims und Kernbotschaften fest.
3. Wir definieren Designsysteme.
4. Wir legen die Absenderlogik „by Get IT Done" fest.
5. Wir prüfen Domains und Produktnamen.
6. Wir richten die Get-IT-Done-Website auf die drei Produktwelten aus.

### Phase 2: WERK Agent kommerzialisieren

1. drei priorisierte Produktions-Use-Cases auswählen
2. standardisiertes Pilotangebot definieren
3. Demo mit realistischen Produktionsdaten aufbauen
4. ROI-Logik entwickeln
5. Security- und Architekturunterlagen erstellen
6. Zielaccount-Liste aufbauen
7. erste Referenzkunden systematisch dokumentieren

### Phase 3: WERK Cloud fokussieren

1. WERK Cloud als Betriebsplattform für WERK Agent definieren
2. Kernfunktionen und Nicht-Ziele dokumentieren
3. LLM-Governance und Sicherheitsmodell aufbauen
4. relevante industrielle Konnektoren priorisieren
5. Managed-Service-Pakete und SLAs definieren
6. erst danach eigenständige Plattformvermarktung prüfen

### Phase 4: workload.zero umstellen, validieren und skalieren

1. Workbase in einem Schritt auf workload.zero umstellen (Apps, MCP-Connector, E-Mail-Absender, Rechnungsvorlagen, Theme, Weiterleitung von workbase.itdone.de)
2. Domains sichern und Marken anmelden (DPMA, EUIPO; Klassen 9, 35, 42)
3. je Produkt eine eigene Landingpage mit eigenem SEO-Fokus aufbauen
4. die drei Referenzabläufe (Dienstleister, Vermittler, Professional) durchgängig schließen
5. CV-Automatisierung als Differenzierungsmerkmal ausbauen
6. E-Rechnung und DATEV deutlich kommunizieren
7. Self-Service-Onboarding optimieren und Preisbereitschaft je Paket testen
8. Aktivierung, Cross-Selling zwischen den Produkten und Kündigungsrate messen

### Phase 4a: KETTE als eigene Marke einführen

1. KETTE als eigene Marke mit eigenem Markt, eigener Botschaft und eigenem Vertrieb aufstellen ([ADR 0003](../decisions/0003-kette-eigene-marke.md))
2. Warteliste auf kette.itdone.de bis zum Verkaufsstart führen
3. Verkaufsstart am 01.11.2026: Die Kette (eine Person / Team), Agenten-Pack und Design-Review-Pack
4. Überführung bestehender Design Systems auf Anfrage anbieten, immer beginnend mit der Bestandsaufnahme
5. öffentliche Storybooks und den Prototyp als Beleg aktuell halten
6. erste Verkäufe, Anfragen und Rückmeldungen messen, bevor wir weitere KETTE-Produkte ableiten
7. Markenprüfung und Domainstrategie für KETTE klären, Benennung der Storybooks unter KETTE entscheiden (offene Frage in ADR 0003)

### Phase 5: WERK Einsatz prüfen

1. zehn bis fünfzehn Interviews mit Serviceleitern durchführen
2. drei konkrete Prozesse beobachten
3. Zahlungsbereitschaft und Integrationsanforderungen prüfen
4. workload.zero-Technologie gegen Industrieanforderungen bewerten
5. Pilot mit einem Maschinen- oder Anlagenbauer durchführen
6. erst bei nachgewiesenem Bedarf als Produkt ausgründen

---

## Unsere Prioritäten

### Priorität 1: WERK Agent als Leitprodukt etablieren
WERK Agent hat für uns den stärksten strategischen Fit, ein relevantes Problem, hohe potenzielle Vertragswerte und eine klare Verbindung zu unseren bestehenden Kompetenzen.

### Priorität 2: WERK Cloud als Enabler positionieren
WERK Cloud ermöglicht zunächst den sicheren Betrieb von WERK Agent und weiteren industriellen Anwendungen. Eine zu breite Plattformpositionierung vermeiden wir bewusst.

### Priorität 3: workload.zero als eigenständiges SaaS steuern
workload.zero führen wir mit eigenem Marketingbudget, eigenen Kennzahlen, eigenem Onboarding, getrennter Vertriebslogik und klaren Profitabilitätszielen.

### Priorität 4: WERK Einsatz erst validieren
Die Idee ist attraktiv, aber der Markt ist wettbewerbsintensiv. Einen Produktstart machen wir von Kundeninterviews und einem Pilotkunden abhängig.

### KETTE als eigenständiges Self-Service-Geschäft führen
KETTE ist eigene Marke ([ADR 0003](../decisions/0003-kette-eigene-marke.md)). Wir führen sie mit eigenen Kennzahlen und eigenem Vertrieb als Self-Service mit wenig Personenzeit. Die Überführung bieten wir nur im Rahmen der verfügbaren Kapazität an. ZERO läuft auf KETTE und bleibt ihre wichtigste Referenz.

### Priorität 5: Dienstleistungen produktnah ausrichten
Beratung, Entwicklung und Betrieb sollen den Verkauf und die Nutzung unserer eigenen Produkte beschleunigen.

---

## Unser Gesamtbild

| Einheit | Potenzial | Rolle / Bedingung |
|---|---|---|
| **Get IT Done** | stark als Produktentwickler, Integrator und Betreiber | Wir achten darauf, uns nicht zu breit darzustellen und nicht zu viele Initiativen parallel zu fahren |
| **WERK** | sehr stark als vertikale Produktmarke für industrielle Arbeit | Erfolgsbedingung: konkrete Use Cases, messbare Ergebnisse, industrielle Glaubwürdigkeit |
| **WERK Agent** | sehr hoch | unser Leitprodukt und Türöffner in Produktionsunternehmen |
| **WERK Cloud** | hoch | technische und kommerzielle Bindungsschicht für unsere WERK-Produkte |
| **workload.zero** | gut als modulare Suite, ausgehend vom PSA-Kern | eigenständiges digitales Geschäftsmodell unter ZERO; Bedingung: Suite-Versprechen durch durchgängige Abläufe einlösen |
| **KETTE** | gut als Self-Service-Geschäft, noch ohne Verkäufe | eigene Marke für Design-System-Infrastruktur, ZERO läuft darauf als Referenz; Bedingung: Verkäufe ab 01.11.2026 belegen die Nachfrage, die Überführung bindet nicht mehr Kapazität als verfügbar |
| **WERK Einsatz** | hoch, aber noch nicht bewiesen | möglicher nächster vertikaler Baustein nach Marktvalidierung |

---

## Unser Fazit

Unsere Architektur ist schlüssig:

```text
Get IT Done
├── WERK – industrielle Software
├── ZERO – workload.zero, Business-Suite für Unternehmen, Teams und Professionals
└── KETTE · Design-System-Infrastruktur, verkettet von Agenten
```

Sie erlaubt uns, drei unterschiedliche Märkte zu bedienen, ohne Zielgruppen, Botschaften und Vertriebsmodelle miteinander zu vermischen.

Unsere stärkste Gesamtpositionierung lautet:

> **Wir entwickeln und betreiben digitale Produkte für industrielle Unternehmen, Dienstleister und Professionals.**
