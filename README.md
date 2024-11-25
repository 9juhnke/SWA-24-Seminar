# SWA Seminar 2024

This repository contains the architecture documentation for the SWA Seminar 2024.

[Latest Release](https://github.com/9juhnke/SWA-24-Seminar/releases/tag/latest)

---


## Übung Nr. 2 - Vermitteln des Systemzwecks

### 1. Bringt euer System mit einem Produktkarton auf den Punkt.

Vorschlag (Sven):

Vorderseite: 

**TravelHub - Ihr persönlicher Reise-Assistent**
_Alle Ihre Reisen. Ein Dashboard. Überall verfügbar._

Rückseite:

**Was ist TravelHub?**
TravelHub ist Ihr digitales Reise-Cockpit, das alle Ihre Reisebuchungen intelligent zusammenführt. Egal ob Geschäftsreise oder Urlaub – behalten Sie stets den Überblick über Ihre Flüge, Hotels und Mietwagen.

**Hauptfunktionen:**
- Automatische Synchronisation mit Ihren Vielflieger-, Hotel- und Mietwagenkonten
- Intelligente Gruppierung Ihrer Buchungen nach Reisen
- Teilen Sie Ihre Reisepläne in sozialen Medien
- Verfügbar auf allen Ihren Geräten

**Für wen ist TravelHub?**
- Vielreisende, die den Überblick behalten möchten
- Geschäftsreisende mit komplexen Reiseplänen
- Urlauber, die ihre Reisedaten zentral verwalten möchten

### 2. Ergänzt euren Produktkarton in eurem Architekturüberblick. In welchem Kapitel wäre er am Besten aufgehoben?

Vorschlag (Sven): 
- erledigt, in die Einführung, direkt nach der "Aufgabenstellung", als prägnante Zusammenfassuung

### 3. Entwerft drei Personas fur euer System, an denen ihr spätere Architekturentscheidungen oder Qualitätsziele / -szenarien ausrichten wollt.

Vorschlag (Sven):
- verschiedene wichtige Nutzungsszenarien abdecken:
  - Geschäftsreisende: Sarah Chen, 42 Jahre, Senior Consultant
  - Familienreisende:  Marcus Weber, 35 Jahre, Projektmanager
  - Individualreisende: Emma Schmidt, 28 Jahre, freiberufliche Fotografin

### 4. Ergänzt auch eure Personas in eurem Architekturüberblick. In welchem Kapitel wären sie am Besten aufgehoben?

Vorschlag (Sven): 
- erledigt, in die Einführung, vor "Stakeholder" da sie Nutzergruppen detailliert beschreiben, bevor abstraktere Stakeholder-Rollen genannt werden


## Übung Nr. 1 - Werkzeuge zur Dokumentation

### 1. Entscheidet in eurer Gruppe mit welchen Werkzeugen ihr euren Architekturüberblick erstellen wollt.

Vorschlag (Sven): 
- **AsciiDoc** mit **Asciidoctor** für die Dokumentation
- **PlantUML** für Diagramme (integriert in Asciidoctor) oder besser **Mermaid** falls möglich
- **GitHub Actions** für automatisierte Builds
    - erzeugt PDF als Download-Artifact

    Begründung:
    - alles ist Text → perfekte Versionierung in Git
    - paralleles Arbeiten durch Branching / Merging möglich
    - automatische Builds durch GitHub Actions
    - plattformunabhängig (Windows / Mac / Linux)
    - keine Lizenzkosten, keine proprietären Formate
    - professionelles PDF-Output für die Abgabe
    - ein Source-Format für PDF

### 2. Legt euren Architekturüberblick als Dokument an und fügt die Arc42-Kapitel 1,2,3,5,6,7,9 und 10 mitsamt der Überschriften ein.

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

### 3. Im Laufe dieses Seminars werdet ihr ein System als Lösung für unsere Architektur-Kata entwerfen. Gebt eurem System einen Arbeitstitel und nehmt ihn in den Titel des Dokuments auf.

Vorschlag (Sven):
- "**TravelHub** - Next Generation Trip Management Dashboard"
    
    Begründung:
    - beschreibt Kernfunktion: zentrale Integration aller Reisedaten
    - passt zur Hauptanforderung "integrate seamlessly with existing systems"
    - technisch passend: System ist tatsächlich ein Hub für verschiedene Dienste

### 4. Stellt sicher, dass ihr euren Architekturüberblick als PDF-Datei exportieren könnt.

Vorschlag (Sven):
- **GitHub Actions**:
    - bei jedem Push auf Main wird automatisch gebaut
    - PDF-Version als Download in [Releases, Latest](https://github.com/9juhnke/SWA-24-Seminar/releases/tag/latest)

