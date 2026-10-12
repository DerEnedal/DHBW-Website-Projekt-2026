# Centora – Website-Projekt 2026

Statische Website für **Centora**, eine Finanz-App.
Webseiten-Projekt, DHBW Heidenheim, 1. Semester.

> Deine Finanzen. Einfach. Transparent.

## Vorgaben

- Nur **HTML** und **CSS**
- **Kein JavaScript**

## Ordnerstruktur

```
DHBW-Website-Projekt-2026/
├── index.html                  # Startseite (One-Pager)
├── funktionen/
│   ├── haushaltsplan.html
│   ├── portfolio.html
│   ├── sparziele.html
│   └── zinseszins-rechner.html
├── rechtliches/
│   ├── datenschutz.html
│   └── impressum.html
└── assets/
    ├── css/
    │   └── style.css           # Ein Stylesheet für alle Seiten
    ├── fonts/                  # Selbst gehostete Schriften
    └── images/
        ├── logo/               # Centora-Logo
        ├── icons/              # Icons (SVG)
        ├── illustrations/      # Grafiken, Diagramme
        └── screenshots/        # App-Screenshots
```

## Farben

| Name          | Hex       | Verwendung                         |
|---------------|-----------|------------------------------------|
| Dunkelgrün    | `#0F3D2E` | Text, Buttons, dunkle Flächen      |
| Akzentgrün    | `#3A9D6B` | Fortschrittsbalken, Zahlen, Punkte |
| Hellblau      | `#8FDCF2` | Icons, Illustrationen              |
| Mint          | `#EAF4F1` | Abschnitts-Hintergründe, Badges    |
| Hintergrund   | `#F6F9F8` | Seitenhintergrund                  |

## Regeln

- Dateinamen nur in Kleinbuchstaben, ohne Leerzeichen und Umlaute (`ueber-uns.html`)
- Relative Pfade verwenden (`assets/css/style.css`, in Unterordnern `../assets/css/style.css`)
- `.gitkeep`-Dateien halten leere Ordner im Repo und können gelöscht werden, sobald echte Dateien darin liegen
