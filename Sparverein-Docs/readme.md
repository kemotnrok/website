# Sparverein

## Thomas Korn

http://localhost:5152

## Projektbeschreibung

Die Anwendung verwaltet Mitglieder und Geldflüsse eines Sparvereins

### Hauptfunktionen

- Anlegen, Bearbeiten und Löschen von Vereinsmitgliedern
- Anlegen, Bearbeiten und Löschen von Zahlungen
- Suche und Filterung von Zalungen
- Statistiken von Zahlungen

## Technologien

| Technologie                  | Einsatzgebiet       |
| ---------------------------- | ------------------- |
| C#                           | Programmlogik       |
| ASP.NET Core MVC             | Webanwendung        |
| Entity Framework Core        | Datenbankzugriff    |
| SQL Server                   | Datenbank           |
| SQL Server Management Studio | Datenbankverwaltung |
| Razor Views                  | Benutzeroberfläche  |
| Bootstrap                    | Layout und Styling  |

## Projektstruktur (MVC)

### Model

Enthält die Datenmodelle der Anwendung

- Zahlung
- Vereinsmitglied

### View

Enthält CSHTML-Dateien für die Benutzeroberfläche

- Zahlungen 
    - Liste (**Startseite**)
    - Details
    - Bearbeiten
- Vereinsmitglieder 
    - Liste
    - Details
    - Bearbeiten
- Statistiken

### Controller

Verarbeitet Benutzereingaben und steuert die Anwendung

- ZahlungController
- VereinsmitgliedController
- StatistikController

### DbContext

Verbindet die Anwendung mit der Datenbank und verwaltet die Entitäten

## ER-Diagramm

```mermaid
flowchart TD
    A --- aa
    A --- ab
    A --- ac
    A --- ad
    B --- ba
    B --- bb
    B --- bc
    A -- 1 : n ---> B

    A[Vereinsmitglied]
    B[Zahlung]
    aa(Vorname)
    ab(Nachname)
    ac(IsAktiv)
    ad(Bild)
    ba(Zeitpunkt)
    bb(Betrag)
    bc(Beschreibung)
```
