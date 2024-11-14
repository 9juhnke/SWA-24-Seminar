# SWA Seminar 2024

This repository contains the architecture documentation for the SWA Seminar 2024.

---

## Übung Nr. 1 - Werkzeuge zur Dokumentation

#### 1. Entscheidet in eurer Gruppe mit welchen Werkzeugen ihr euren Architekturüberblick erstellen wollt.

Vorschlag (Sven): 
- **AsciiDoc** mit **Asciidoctor** für die Dokumentation
- **PlantUML** für Diagramme (integriert in Asciidoctor)
- **GitHub Actions** für automatisierte Builds
    - generiert HTML für GitHub Pages
    - erzeugt PDF als Download-Artifact

    Begründung:
    - alles ist Text → perfekte Versionierung in Git
    - paralleles Arbeiten durch Branching/Merging möglich
    - automatische Builds durch GitHub Actions
    - plattformunabhängig (Windows/Mac/Linux)
    - keine Lizenzkosten, keine proprietären Formate
    - professionelles PDF-Output für die Abgabe
    - ein Source-Format für HTML und PDF

#### 2. Legt euren Architekturüberblick als Dokument an und fügt die Arc42-Kapitel 1,2,3,5,6,7,9 und 10 mitsamt der Überschriften ein.

Vorschlag (Sven): 
- erledigt, Überschriften als Struktur in `src/` angelegt

    ```
    repository/
    ├── .github/
    │   └── workflows/
    │       └── docs.yml
    ├── src/
    │   ├── images/
    │   ├── diagrams/
    │   ├── index.adoc
    │   ├── 01_introduction.adoc
    │   ├── 02_constraints.adoc
    │   └── ...
    ├── .gitignore
    └── README.md
    ```

#### 3. Im Laufe dieses Seminars werdet ihr ein System als Lösung für unsere Architektur-Kata entwerfen. Gebt eurem System einen Arbeitstitel und nehmt ihn in den Titel des Dokuments auf.

Vorschlag (Sven):
- "**TravelHub** - Next Generation Trip Management Dashboard"
    
    Begründung:
    - beschreibt Kernfunktion: zentrale Integration aller Reisedaten
    - passt zur Hauptanforderung "integrate seamlessly with existing systems"
    - technisch passend: System ist tatsächlich ein Hub für verschiedene Dienste

#### 4. Stellt sicher, dass ihr euren Architekturüberblick als PDF-Datei exportieren könnt.

Vorschlag (Sven):
- **GitHub Actions**:
    - bei jedem Push wird automatisch gebaut
    - HTML-Version auf GitHub Pages: https://9juhnke.github.io/SWA-24-Seminar
    - PDF-Version als Download in GitHub Actions Artifacts
    - professionelles Layout durch angepasste AsciiDoc Themes

