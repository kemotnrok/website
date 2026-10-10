# Lagerverwaltung

## Thomas Korn

http://localhost:5249

## Projektbeschreibung

Die Anwendung dient dem Betrieb einer Lagerverwaltung, in der Produkte verschiedener Kategorien ein- und verkauft werden können.

### Hauptfunktionen

- Kategorien anlegen/bearbeiten/löschen
- Produkte anlegen/bearbeiten/löschen
- Produkte verkaufen
- Produkte nachbestellen
- Statistiken

## Technologien

| Technologie | Einsatzgebiet |
| --- | --- |
| C# | Programmlogik |
| ASP.NET Core | Webanwendung |
| Entity Framework Core | Datenbankzugriff |
| SQL Server | Datenbank |
| SQL Server Management Studio | Datenbankverwaltung |
| Razor Views | Benutzeroberfläche  |
| Bootstrap | Layout und Styling  |

## Projektstruktur (MVC)

### Model

Enthält die Datenmodelle der Anwendung

- Kategorie
- Produkt 
- Verkauf
- Nachbestellung

### View

Enthält CSHTML-Dateien für die Benutzeroberfläche

- Kategorie
    - Liste
    - Bearbeiten
- Produkte (Startseite)
    - Liste
    - Erstellen
    - Details
- Verkäufe
    - Liste
    - Erstellen
    - Details
    - Bearbeiten
- Nachbestellungen
    - Liste
    - Erstellen
    - Details
    - Bearbeiten

### Controller

Verarbeitet Benutzereingaben und steuert die Anwendung

- KategorieController
- ProduktController
- VerkaufController
- NachbestellungController

### DbContext

Verbindet die Anwendung mit der Datenbank und verwaltet die Entitäten


