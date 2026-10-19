# Portfolio

So schätzen wir unser Portfolio ein – nach Product-Persona-Fit, Umsatzpotenzial, Skalierbarkeit und Differenzierung – und so lassen wir die Produkte im Use-Case zusammenspielen.

## Unser Portfolio im Überblick

| Angebot | Product-Persona-Fit | Umsatzpotenzial je Kunde | Skalierbarkeit | Differenzierung | Priorität |
|---|---:|---:|---:|---:|---:|
| **[WERK Agent](../products/werk-agent/)** | sehr hoch | hoch | mittel bis hoch | hoch | 1 |
| **[WERK Cloud](../products/werk-cloud/)** | hoch als Plattform, mittel als Einzelprodukt | hoch | mittel | mittel bis hoch | 2 |
| **[ZERO workload.zero](../products/workload-zero/)** | hoch | niedrig bis mittel (Solo), mittel (Teams) | sehr hoch | mittel bis hoch | 3 |
| **[WERK Einsatz](../products/werk-einsatz/)** | potenziell hoch | mittel bis hoch | hoch | mittel | erst validieren |
| **KETTE [Die Kette](../products/die-kette/)** | hoch bei Teams mit Claude Code, mittel bei Einzelnen | niedrig (Einzelne), mittel (Teams), hoch (Überführung) | sehr hoch als Paket, niedrig als Überführung | hoch | Einführung, Verkaufsstart 01.11.2026 |
| **[Unsere Services](../go-to-market/services.md)** | hoch | hoch | niedrig | abhängig von Expertise | unterstützend |

Die Details je Angebot beschreiben wir in den jeweiligen Produktordnern.

KETTE ist seit [ADR 0003](../decisions/0003-kette-eigene-marke.md) eigene Marke mit eigenem Markt. Die Zeile zu Die Kette ist eine Einschätzung ohne Marktbeleg, es gibt noch keine Verkäufe. Sie steht für die ganze Produktwelt KETTE: Die Kette, Agenten-Pack, Design-Review-Pack und Überführung.

---

## Wie unsere Produkte zusammenspielen

Ihren vollen Wert entfalten unsere Produkte im Zusammenspiel. Sechs zentrale Anwendungsfälle:

### 1. Produktionsqualität verbessern

**Problem:** Qualitätsabweichungen werden erst spät erkannt. Prozess-, Labor- und Maschinendaten sind nicht miteinander verbunden.

**So lösen wir das:**
- WERK Agent analysiert Zusammenhänge.
- WERK Cloud stellt Daten und Modelle sicher bereit.
- Wir integrieren die Datenquellen.
- Maßnahmen dokumentieren wir nachvollziehbar.

### 2. Stillstände reduzieren

**Problem:** Störungsursachen werden manuell und wiederholt untersucht.

**So lösen wir das:**
- WERK Agent analysiert Ereignisse vor dem Stillstand.
- Wir kombinieren die Ergebnisse mit dem Anlagenwissen der Mitarbeiter.
- Wir bauen wiederverwendbare Analysemuster auf.
- WERK Cloud übernimmt Betrieb und Governance.

### 3. Serviceeinsätze schneller abrechnen

**Problem:** Einsatzplanung, Dokumentation und Abrechnung sind voneinander getrennt.

**So lösen wir das:**
- WERK Einsatz plant und dokumentiert den Einsatz.
- Leistungsnachweise werden digital freigegeben.
- Rechnungsdaten entstehen direkt oder gehen ans ERP.
- WERK Agent unterstützt bei komplexen Maschinenstörungen.

### 4. Sichere KI in der Produktion einführen

**Problem:** Fachbereiche möchten KI einsetzen, IT und Datenschutz benötigen Kontrolle.

**So lösen wir das:**
- WERK Cloud stellt freigegebene Modelle bereit.
- Wir definieren Rollen, Rechte und Datenzugriffe.
- WERK Agent liefert einen konkreten fachlichen Anwendungsfall.
- Wir übernehmen Architektur, Einführung und Schulung.

### 5. Verwaltung rund um Projektarbeit vereinfachen

**Problem:** Freelancer und Dienstleister nutzen mehrere Werkzeuge für Projekte, Zeiten, Rechnungen, Kunden und den CV.

**So lösen wir das:**
- workload.zero verbindet den gesamten Ablauf: workstream.zero, backoffice.zero und jobsearch.zero auf einer Datenbasis.
- Projektinformationen werden nur einmal gepflegt.
- Timesheets, Rechnungen und CV entstehen aus denselben Daten.
- Freelancer und Teams gewinnen Zeit für abrechenbare Arbeit und neue Projekte.

### 6. Business-Apps konsistent und geprüft bauen (KETTE)

**Problem:** Teams bauen mit KI schnell Oberflächen, aber jede sieht anders aus. Figma und Code laufen auseinander, und keiner prüft unabhängig.

**So lösen wir das:**
- Die Kette liefert Tokens, Figma-Dateien, Komponenten, Fachkomponenten und Seitenvorlagen aus einer Quelle.
- Agenten führen jede Änderung durch einen Loop mit unabhängigen Prüfungen.
- Wer klein einsteigen will, beginnt mit dem Agenten-Pack oder dem Design-Review-Pack.
- Wer schon ein Design System hat, bekommt eine Überführung statt eines Neubaus.
- ZERO ist der laufende Beleg: workload.zero und seine Landingpages laufen auf KETTE.
