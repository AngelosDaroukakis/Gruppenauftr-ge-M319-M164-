# Codera Battle – Gruppenauftrag (M319 / M164)

## Titel
Codera Battle – rundenbasiertes Kampfsystem mit Datenbankanbindung

## Kurzbeschreibung
*Codera Battle ist ein Gruppenprojekt, in dem ein CLI-basiertes Kampfsystem in Go entwickelt und mit einer PostgreSQL-Datenbank über Docker verbunden wird.*

---

## 1. Projektübersicht

Codera Battle ist ein Gruppenauftrag, der die Module M319 (Programmieren in Go) und M164 (Datenbanken) kombiniert. Ziel ist die Entwicklung eines rundenbasierten Kampfsystems in Go sowie die Umsetzung einer relationalen Datenbank mit PostgreSQL.

Jede Person hat eine feste Rolle und trägt Verantwortung in beiden Modulen. Die Zusammenarbeit ist so aufgebaut, dass das gesamte System modular entwickelt und später zusammengeführt wird.

---

## 2. Rollenverteilung

- **Masato – Arkan Dokumentar**  
  Verantwortlich für Dokumentation, Strukturierung der Projektunterlagen, Diagramme (C4, Activity), Git-History-Übersicht und technische Nachvollziehbarkeit.

- **Angelos – Daten Druide**  
  Verantwortlich für Datenbankdesign, ERD-Erstellung, SQL-Logik, JOIN-Abfragen, Seed-Daten sowie Docker-Setup der PostgreSQL-Instanz.

- **Lazar – Code Kleriker**  
  Verantwortlich für die Implementierung der Go-Logik, Kampfsystem, Helden-Pakete, RNG-Mechaniken, Logging, Goroutines und technische Integration.

---

## 3. Spielsystem (M319)

Das Projekt basiert auf einem rundenbasierten Kampfsystem in der CLI.

Der Entropie-Drache ist ein fixer Gegner und darf nicht verändert werden. Jeder Spieler entwickelt einen eigenen Helden als separates Go-Paket mit individuellen Stats, Fähigkeiten und Ausrüstung.

Der Kampf wird über Zufall (RNG) gesteuert, inklusive Trefferchance, Schaden und kritischen Treffern.

Zusätzlich muss jede Person folgende technische Anforderungen umsetzen:
- Logging
- GORM Datenbankanbindung
- Goroutines mit Mutex
- Godoc Dokumentation
- Unit Tests

---

## 4. Datenbank (M164)

Jede Person betreibt eine eigene PostgreSQL-Instanz über Docker.

Gemeinsam wird ein ERD erstellt und in ein relationales Schema umgesetzt. Danach werden die Tabellen per DDL erstellt und mit Seed-Daten befüllt.

Anschliessend werden SQL-Abfragen mit JOINs und Filtern umgesetzt. Die Datenbank wird als SQL-Dump exportiert und wieder importiert.

---

## 5. Abgabeanforderungen

Die Abgabe erfolgt über ein Git-Repository mit vollständiger Commit-History.

Enthalten sein müssen:
- Vollständige Git-History (klare Zuordnung der Beiträge)
- Gruppendokumentation
- C4-Diagramme
- Activity-Diagramme
- Unit Tests
- Godoc Dokumentation
- SQL-Skripte (DDL, Seed, Queries, Dump)

Fehlende oder nicht nachvollziehbare Beiträge können zu Notenabzug für die gesamte Gruppe führen.
