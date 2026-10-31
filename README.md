# Centora – Deine Finanzen. Einfach. Transparent.

Statische, responsive Marketing-Website für **Centora**, eine fiktive Finanz-App zum Sparen, Planen und Investieren. Entstanden im **Webseiten-Projekt 2026** an der **DHBW Heidenheim**. Reines HTML und CSS, ohne JavaScript, mit automatischem Dark Mode.

![HTML5](https://img.shields.io/badge/HTML5-semantisch-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-Grid_%26_Flexbox-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-keins-lightgrey)
![Dark Mode](https://img.shields.io/badge/Dark_Mode-automatisch-0f1a16)
![Status](https://img.shields.io/badge/Status-Prototyp-0f3d2e)

> **Hinweis:** Centora ist keine echte Firma und keine echte App. Alle Zahlen, Preise, Zitate und Firmendaten (inkl. Impressum, HRB- und USt-ID) sind Platzhalter bzw. Beispieldaten. Das gilt auch für den Partner „TauRes“.

## Auf einen Blick

| Frage | Antwort |
|---|---|
| **Wer?** | Vier Studierende der DHBW Heidenheim · Kontakt: [daniel@rosenberger.click](mailto:daniel@rosenberger.click) |
| **Was?** | 8 HTML-Seiten, 1 Stylesheet, Bilder (PNG, JPG, SVG). Keine Skripte, kein Build. |
| **Wann?** | Letzte Aktualisierung: 31.10.2026 |
| **Wo?** | [github.com/DerEnedal/DHBW-Website-Projekt-2026](https://github.com/DerEnedal/DHBW-Website-Projekt-2026) (Branch `main`) |
| **Warum?** | Studienprojekt: Entwurf und Umsetzung einer vollständigen Produktwebsite, von der Gestaltung bis zum fertigen Code |

Ordnerstruktur und Dateibenennung stehen zusätzlich in **[`README_Ordnerstruktur.txt`](README_Ordnerstruktur.txt)** auf oberster Ebene.

## Inhaltsverzeichnis

1. [Projekt und Zweck](#1-projekt-und-zweck)
2. [Features und Seiten](#2-features-und-seiten)
3. [Verwendete Technologien](#3-verwendete-technologien)
4. [Voraussetzungen](#4-voraussetzungen)
5. [Installation und lokaler Start](#5-installation-und-lokaler-start)
6. [Ordnerstruktur](#6-ordnerstruktur)
7. [Design](#7-design)
8. [Konfiguration](#8-konfiguration)
9. [Deployment](#9-deployment)
10. [Kontakt](#10-kontakt)
11. [Lizenz](#11-lizenz)
12. [Anhang](#12-anhang)

## 1. Projekt und Zweck

**Centora** führt Konten, Depot, Verträge, Fixkosten und Sparziele in einer Übersicht zusammen. Die Website erklärt Funktionen, Sicherheitskonzept, Team und Preismodell und führt Besucherinnen und Besucher zum Download der App.

| Markenprinzip | Umsetzung auf der Website |
|---|---|
| **Einfach** | Kurze Headlines, wenig Fachsprache, ein Gedanke pro Banner |
| **Transparent** | Preise, Funktionen und Datenverarbeitung offen dargestellt |
| **Sicher** | Nur Lesezugriff, TLS-Verschlüsselung, Server in Frankfurt (EU) |

## 2. Features und Seiten

### Features

- **Responsive** für Desktop und Handy (Breakpoint 700 px)
- **Automatischer Dark Mode** nach Systemeinstellung
- **Interaktion ohne JavaScript:** Feature-Tabs, Umschalter Monatlich/Jährlich, aufklappbare FAQ, Kapitelnavigation
- **Preisübersicht** mit drei Plänen und Vergleichstabelle (auf schmalen Bildschirmen seitlich scrollbar)
- **Zentrales Design-System** über CSS-Variablen
- **Datenschutzfreundlich:** keine Cookies, keine Tracker, keine externen Schriften oder Skripte
- **Barrierefreiheits-Grundlagen:** semantisches HTML, Alt-Texte, Fokusrahmen bei Tabs und Umschaltern

Nicht enthalten: Mehrsprachigkeit (nur Deutsch), Kontaktformular mit Backend (Kontakt per `mailto:`), funktionierender Newsletter-Versand.

### Seiten

Jede Seite besteht aus **Bannern**. Ein Banner ist ein eigener `<section>`-Block mit genau einer Aufgabe.

| Seite | Datei | Banner | Inhalt |
|---|---|---|---|
| Startseite | `index.html` | 4 | Hero, drei Problemfelder, Feature-Tabs, Newsletter |
| Funktionen | `mega-menu/funktionen.html` | 9 | Hero mit Handy-Fächer, Kapitelnavigation, 7 Feature-Banner, Abschluss |
| Sicherheit | `mega-menu/sicherheit.html` | 8 | Drei Versprechen, Anmeldung, Geräte, Datenschutz, Datenfluss, FAQ |
| Über uns | `mega-menu/ueber-uns.html` | 6 | Teamfoto, Mission, Team, Zeitleiste, Partner |
| Jetzt starten | `mega-menu/jetzt-starten.html` | 5 | Download mit QR-Code, Pläne, Vergleichstabelle, FAQ |
| Impressum | `rechtliches/impressum.html` | – | Anbieterkennzeichnung |
| Datenschutz | `rechtliches/datenschutz.html` | – | Datenschutzerklärung (DSGVO) |
| AGB | `rechtliches/agb.html` | – | Allgemeine Geschäftsbedingungen |

## 3. Verwendete Technologien

| Bereich | Technologie |
|---|---|
| Markup | HTML5 (semantische Elemente) |
| Styling | CSS3: Custom Properties, Grid, Flexbox, `clamp()`, `:has()`, `:focus-visible`, `prefers-color-scheme` |
| Logik / Skripte | keine |
| Build-Tools / Paketmanager | keine |
| Schriften | Systemschriften, Georgia für Überschriften (keine Webfonts) |
| Grafiken | PNG, JPG, SVG, Inline-SVG für Symbole |
| Versionskontrolle | Git, GitHub |
| Hosting | beliebiges statisches Hosting, siehe [Deployment](#9-deployment) |

**Browser:** aktuelle Versionen von Chrome, Edge, Safari und Firefox (wegen `:has()` Firefox ab Version 121).

## 4. Voraussetzungen

Zum **Ansehen** genügt ein aktueller Browser.

Zum **Bearbeiten** werden benötigt:

- Texteditor oder IDE (z. B. VS Code)
- Git
- Optional für einen lokalen Webserver: Python 3 **oder** Node.js (nur für `npx serve`)

Das Projekt selbst braucht weder Node.js noch npm.

## 5. Installation und lokaler Start

Es gibt keine Abhängigkeiten und keinen Build-Schritt.

```bash
# Repository klonen
git clone https://github.com/DerEnedal/DHBW-Website-Projekt-2026.git

# In den Ordner wechseln
cd DHBW-Website-Projekt-2026

# Variante 1: Startseite direkt im Browser öffnen
open index.html            # macOS
# start index.html         # Windows

# Variante 2: lokalen Server starten (empfohlen)
python3 -m http.server 8000
# danach im Browser: http://localhost:8000
```

**Wichtig beim Bearbeiten von `style.css`:** Das Stylesheet ist mit Versionsparameter eingebunden (`style.css?v=8`). Nach einer Änderung die Nummer in **allen 8 HTML-Dateien** erhöhen, damit Browser nicht die alte Datei aus dem Cache laden.

## 6. Ordnerstruktur

```text
.
├── README.md
├── README_Ordnerstruktur.txt
├── index.html
├── mega-menu/
│   ├── funktionen.html
│   ├── sicherheit.html
│   ├── ueber-uns.html
│   └── jetzt-starten.html
├── rechtliches/
│   ├── impressum.html
│   ├── datenschutz.html
│   └── agb.html
├── assets/
│   ├── css/
│   │   └── style.css
│   ├── fonts/
│   └── images/
│       ├── favicon/
│       ├── logo/
│       ├── startseite/
│       ├── funktionen/
│       ├── sicherheit/
│       ├── ueber-uns/
│       └── jetzt-starten/
└── .gitignore
```

**Kurzregeln zur Benennung** (Details und Bildzuordnung in `README_Ordnerstruktur.txt`):

- Alles klein geschrieben, Wörter mit Bindestrich getrennt (`jetzt-starten.html`)
- Umlaute werden ausgeschrieben (`ueber-uns`, `app-geraete.png`)
- Bildordner: `assets/images/<seite>/banner-<nr>/`, die Nummer entspricht dem Kommentar `<!-- ===== Banner N ===== -->` im HTML
- Bilddateien: `app-<thema>.png` für App-Screenshots, `tab-<thema>.png` für die Startseiten-Tabs

## 7. Design

Das Design folgt einem ruhigen, editorialen Stil: viel Weißraum, große Serifen-Headlines, ein einziger grüner Akzent und App-Screenshots als Hauptmotiv. Alle Gestaltungswerte liegen als **CSS-Variablen** in `:root` am Anfang von `assets/css/style.css`. Eine Farbe wird einmal geändert und gilt überall.

### 7.1 Gestaltungsprinzipien

| Prinzip | Umsetzung |
|---|---|
| **Klarer Banner-Aufbau** | Überzeile (`.eyebrow`) → Headline → Einleitung (`.lead`) → Aktion oder zwei Kennzahlen |
| **Zweizeilige Headlines** | Links die Aussage, rechts die Pointe: „Alle Konten. / Ein Blick.“ |
| **Rhythmus** | Weiße und graue Bänder wechseln sich ab, Bild und Text spiegeln sich (`.feature-flip`) |
| **Produkt im Fokus** | Handy-Mockups mit grünem Kreis dahinter, unten bewusst abgeschnitten |
| **Wenig Text** | Pro Feature ein Satz und zwei Kennzahlen (`.feature-facts`) statt Fließtext |
| **Ein Akzent** | Grün für Hover, Überzeilen, Häkchen und Linien, sonst neutrale Flächen |
| **Weiche Formen** | Pillenförmige Buttons, Karten mit 14–28 px Radius, sehr dezente Schatten |
| **Projektkennzeichnung** | Rote DHBW-Leiste über dem Header macht den Studienprojekt-Charakter sichtbar |

### 7.2 Farben

**Light Mode**

| Variable | Wert | Verwendung |
|---|---|---|
| `--color-primary` | `#0f3d2e` | Text, Buttons (Dunkelgrün) |
| `--color-accent` | `#3a9d6b` | Hover, Eyebrow, Linien |
| `--color-accent-soft` | `#e8f4ee` | Kreis hinter den Handys |
| `--color-accent-light` | `#7fd8a6` | Akzent auf dunklen Flächen |
| `--color-bg` / `--color-surface` | `#ffffff` / `#f5f5f5` | Seite / graue Bänder |
| `--color-text-muted` | `#555555` | Fließtext |
| `--color-text-soft` | `#8a8a8a` | Kleine Hinweise |
| `--color-border` | `#e5e5e5` | Trennlinien |
| `--color-dark` | `#111111` | Dunkle Abschlussbanner |
| `--color-footer` | `#213f31` | Footer |
| `--color-dhbw` | `#e2001a` | DHBW-Hinweisleiste |

**Dark Mode („Waldgrün“)** – folgt der Systemeinstellung über `@media (prefers-color-scheme: dark)` und überschreibt die Variablen.

| Zweck | Wert |
|---|---|
| Seitenhintergrund | `#0f1a16` |
| Bänder / Karten | `#131f1a` / `#172520` |
| Text / Text gedämpft | `#f2f7f4` / `#a9b8b0` |
| Linien | `#2a3b34` |
| Buttons | `#21934b` |
| Dunkle Bänder / Footer | `#0b1510` / `#08100c` |

Elemente auf dunklen Flächen (`.cta-dark`, `.footer`, `.store-button`, `.plan-highlight`) behalten auch im Dark Mode ihre hellen Originalfarben.

### 7.3 Typografie

| Rolle | Schrift | Details |
|---|---|---|
| Überschriften `h1`, `h2` | Georgia, Fallback Times New Roman, serif | Gewicht 500, Zeilenhöhe ca. 1,0–1,1, leicht negatives Letter-Spacing |
| Fließtext, UI | `system-ui`, `-apple-system`, `Segoe UI`, `Roboto` | Fließtext in `#555555`, Einleitungen 1,15 rem |
| Zitate, Kennzahlen | Georgia | Kursiv bei Zitaten |

Headlines skalieren flüssig mit `clamp()`, z. B. `clamp(2rem, 3.5vw, 2.75rem)` für Abschnittsüberschriften. Es werden keine Webfonts geladen.

### 7.4 Layout und Abstände

- Inhaltsbreite: `.container` mit `max-width: 1100px` und 1 rem Seitenrand
- Raster: CSS Grid für Banner (meist zwei Spalten, 4–5 rem Abstand), Flexbox für Zeilen
- Vertikaler Rhythmus: Bänder mit 5–7 rem Innenabstand
- Sticky Footer: `body` als Flex-Spalte, `.main` mit `flex: 1`
- Icons: Inline-SVG im Linienstil (Strichstärke 1,8, runde Enden, `currentColor`)

### 7.5 Komponenten

| Klasse | Aufgabe |
|---|---|
| `.container` | Zentrierter Inhaltsbereich |
| `.band` | Vollbreite graue Fläche |
| `.feature` · `.feature-grey` · `.feature-flip` | Text-Bild-Banner, abwechselnd Weiß/Grau und gespiegelt |
| `.feature-image` | Handy mit grünem Kreis dahinter |
| `.eyebrow` · `.lead` | Grüne Überzeile und Einleitungstext |
| `.btn` · `.btn-lg` · `.btn-outline` | Pillenförmige Buttons, Hover wechselt auf Akzentgrün |
| `.link-arrow` · `.link-underline` | Textlinks als sekundäre Aktion |
| `.floating-card` · `.hero-badge` · `.qr-card` | Schwebende Info-Karten neben Handys |
| `.plan` · `.plan-highlight` | Preiskarten, mittlere Karte dunkel hervorgehoben |
| `.compare-table` | Vergleichstabelle mit hervorgehobener Plus-Spalte |
| `.faq` | Akkordeon mit `+` / `–` |
| `.cta-dark` | Dunkler Abschlussbanner |
| `.legal` | Typografie der Rechtstexte |
| `.sr-only` | Nur für Screenreader sichtbar |

### 7.6 Responsive Verhalten

Ein Breakpoint bei `max-width: 700px` (Block „Handy“ im CSS):

- Mehrspaltige Raster werden einspaltig, Navigation rutscht unter das Logo
- Handy-Fächer und Hero zeigen nur ein Handy, schwebende Karten und QR-Code entfallen
- Team-Raster und Datenfluss 2 × 2, Pläne untereinander
- Vergleichstabelle scrollt seitlich

### 7.7 Interaktion ohne JavaScript

| Element | Seite | Technik |
|---|---|---|
| Feature-Tabs (4) | Startseite | Unsichtbare Radio-Buttons + `:checked`, Fokus über `:focus-visible` |
| Monatlich / Jährlich | Jetzt starten | Radio-Buttons + `:checked`, Preise als `.price-monthly` / `.price-yearly` |
| Aufklappbare FAQ | Sicherheit, Jetzt starten | Natives `<details>` / `<summary>` |
| Kapitelnavigation | Funktionen | Sprunglinks auf Anker-IDs (`#konten`, `#depot` …) |

### 7.8 Barrierefreiheit

Umgesetzt:

- `lang="de"`, eine `h1` pro Seite, geordnete Überschriftenebenen
- Beschreibende `alt`-Texte, dekorative SVGs mit `aria-hidden="true"`
- Beschriftete Navigationen (`aria-label`), semantische Landmarken
- Newsletter-Feld mit `label.sr-only`
- Radio-Bedienelemente bleiben per Tastatur erreichbar (`opacity: 0` statt `display: none`)
- Native Elemente (`details`, `summary`, `label`) statt eigener Widgets

Verbesserungspotenzial:

- **Kontrast im Light Mode:** `--color-text-soft` (`#8a8a8a`, ca. 3,5 : 1), `--color-text-faint` (`#b0b0b0`, ca. 2,2 : 1) und der Akzent `#3a9d6b` (ca. 3,4 : 1) liegen unter den 4,5 : 1 von WCAG AA für normalen Text
- **Fokusstile** gibt es nur für Tabs und Abrechnungs-Umschalter, nicht für Buttons und Links

## 8. Konfiguration

Das Projekt benötigt **keine** `.env`-Datei, keine API-Keys, keine Datenbank und keinen Mailer. Die einzige Konfiguration ist das Design-System in den CSS-Variablen (siehe [Design](#7-design)).

## 9. Deployment

Die Website besteht nur aus statischen Dateien. Alle Pfade sind relativ, die Seite läuft daher auch in einem Unterverzeichnis. In den Projektdateien ist keine Deployment-Konfiguration hinterlegt. Mögliche Wege:

| Variante | Vorgehen |
|---|---|
| **GitHub Pages** | Repository → Settings → Pages → Source „Deploy from a branch“ → Branch `main`, Ordner `/ (root)` |
| **Netlify / Vercel** | Repository verbinden, kein Build-Befehl, Veröffentlichungsordner ist das Projektstammverzeichnis |
| **Manueller Upload** | Gesamten Ordner per FTP/SFTP auf den Webspace hochladen |

Live-URL: _noch nicht eingetragen_

## 10. Kontakt

### Projektteam

DHBW Heidenheim · Jahrgang 2026

| Name | Rolle | Verantwortlich für |
|---|---|---|
| Mustafa Gökmen | Idee und Produkt | Produktidee, Funktionsumfang |
| Beykan S. Caliskan | Design, UX und Planung| Gestaltung, Design-System, und Planung |
| Daniel Rosenberger | Entwicklung | Umsetzung in HTML und CSS |
| David Zenker | Finanzen | Finanzinhalte, Preismodell |

### Ansprechpartner

| Kanal | Adresse |
|---|---|
| **E-Mail (Projekt, Fragen, Support)** | [daniel@rosenberger.click](mailto:daniel@rosenberger.click) |
| **Fehler und Wünsche** | [GitHub Issues](https://github.com/DerEnedal/DHBW-Website-Projekt-2026/issues) |
| **Repository** | [github.com/DerEnedal/DHBW-Website-Projekt-2026](https://github.com/DerEnedal/DHBW-Website-Projekt-2026) |
| **Institution** | Duale Hochschule Baden-Württemberg (DHBW) Heidenheim |

**Beim Melden eines Fehlers bitte angeben:** betroffene Seite, Browser mit Version, Gerät (Desktop/Handy), Hell- oder Dunkelmodus und wenn möglich einen Screenshot.

## 11. Lizenz

**Vorläufig: Alle Rechte vorbehalten** (Proprietary / All rights reserved). Es handelt sich um ein Studienprojekt. Eine Weiterverwendung von Code, Texten und Grafiken bedarf der Zustimmung des Projektteams.

Marken und Logos Dritter (REWE, Amazon, Shell, Netflix, Spotify, Dropbox, Apple App Store, Google Play, DHBW) gehören den jeweiligen Inhabern und werden ausschließlich zu Demonstrationszwecken im Rahmen dieses Studienprojekts gezeigt.

## 12. Anhang

### Preismodell

| | **Free** | **Plus** *(beliebt)* | **Premium** |
|---|---|---|---|
| Preis monatlich | 0 € | 4,99 € | 9,99 € |
| Preis jährlich (–20 %) | 0 € | 3,99 € / Monat (47,88 € / Jahr) | 7,99 € / Monat (95,88 € / Jahr) |
| Konten verbinden | 2 | unbegrenzt | unbegrenzt |
| Fixkosten und Abos | ✓ | ✓ | ✓ |
| Depot-Übersicht | – | ✓ | ✓ |
| Sparziele | 1 | unbegrenzt | unbegrenzt |
| Aufrunden | – | ✓ | ✓ |
| Zinsrechner | ✓ | ✓ | ✓ |
| Versicherungsvergleich | – | ✓ | ✓ |
| Investitionsempfehlung | – | – | ✓ |
| Persönliche Beratung | – | – | 1 Termin / Monat |
| Export als PDF und CSV | – | – | ✓ |

### Design-System

Alle Farben und Schriften sind als **CSS-Variablen** in `:root` am Anfang von `assets/css/style.css` definiert.

**Farben (Light Mode)**

| Variable | Wert | Verwendung |
|---|---|---|
| `--color-primary` | `#0f3d2e` | Text, Buttons (Dunkelgrün) |
| `--color-accent` | `#3a9d6b` | Hover, Eyebrow, Linien |
| `--color-accent-soft` | `#e8f4ee` | Kreis hinter den Handys |
| `--color-accent-light` | `#7fd8a6` | Akzent auf dunklen Flächen |
| `--color-bg` / `--color-surface` | `#ffffff` / `#f5f5f5` | Seite / graue Bänder |
| `--color-text-muted` | `#555555` | Fließtext |
| `--color-text-soft` | `#8a8a8a` | Kleine Hinweise |
| `--color-border` | `#e5e5e5` | Trennlinien |
| `--color-dark` | `#111111` | Dunkle Abschlussbanner |
| `--color-footer` | `#213f31` | Footer |
| `--color-dhbw` | `#e2001a` | DHBW-Hinweisleiste |

**Farben (Dark Mode, „Waldgrün“)**

| Zweck | Wert |
|---|---|
| Seitenhintergrund | `#0f1a16` |
| Bänder / Karten | `#131f1a` / `#172520` |
| Text / Text gedämpft | `#f2f7f4` / `#a9b8b0` |
| Linien | `#2a3b34` |
| Buttons | `#21934b` |
| Dunkle Bänder / Footer | `#0b1510` / `#08100c` |

**Typografie:** Überschriften `h1`/`h2` in Georgia (Serif, Gewicht 500), Fließtext in Systemschrift (`system-ui`, `Segoe UI`, `Roboto`). Headlines skalieren flüssig mit `clamp()`.

**Layout:** `.container` mit `max-width: 1100px`, CSS Grid für Banner, Flexbox für Zeilen, Sticky Footer über Flex-Spalte am `body`.

**Wiederkehrende Bausteine**

| Klasse | Aufgabe |
|---|---|
| `.container` | Zentrierter Inhaltsbereich |
| `.band` | Vollbreite graue Fläche |
| `.feature` · `.feature-grey` · `.feature-flip` | Text-Bild-Banner, abwechselnd Weiß/Grau und gespiegelt |
| `.feature-image` | Handy mit grünem Kreis dahinter |
| `.eyebrow` · `.lead` | Grüne Überzeile und Einleitungstext |
| `.btn` · `.btn-lg` · `.btn-outline` | Pillenförmige Buttons |
| `.link-arrow` · `.link-underline` | Textlinks als sekundäre Aktion |
| `.floating-card` · `.hero-badge` · `.qr-card` | Schwebende Info-Karten neben Handys |
| `.plan` · `.plan-highlight` | Preiskarten |
| `.cta-dark` | Dunkler Abschlussbanner |
| `.legal` | Typografie der Rechtstexte |
| `.sr-only` | Nur für Screenreader sichtbar |

**Responsive:** Ein Breakpoint bei `max-width: 700px`. Raster werden einspaltig, die Navigation rutscht unter das Logo, Handy-Fächer zeigen nur ein Handy, schwebende Karten und QR-Code entfallen.

**Interaktion ohne JavaScript**

| Element | Seite | Technik |
|---|---|---|
| Feature-Tabs | Startseite | Unsichtbare Radio-Buttons + `:checked` |
| Monatlich / Jährlich | Jetzt starten | Radio-Buttons + `:checked` |
| Aufklappbare FAQ | Sicherheit, Jetzt starten | Natives `<details>` / `<summary>` |
| Kapitelnavigation | Funktionen | Sprunglinks auf Anker-IDs |

### Bekannte Einschränkungen

- Newsletter-Formular ohne Backend (`GET` an `#newsletter`), es werden keine Adressen gespeichert
- Download-Buttons verlinken auf die allgemeinen Startseiten von App Store und Google Play
- Plan-Buttons springen nur zum Download-Bereich, es gibt keinen Bestellprozess
- Rechtstexte und Firmendaten sind Muster und nicht rechtlich geprüft
- Nur ein Breakpoint (700 px), Tablets nutzen das Desktop-Layout
- Kontrast im Light Mode: `#8a8a8a` (ca. 3,5 : 1), `#b0b0b0` (ca. 2,2 : 1) und Akzent `#3a9d6b` (ca. 3,4 : 1) liegen unter den 4,5 : 1 von WCAG AA für normalen Text
- Fokusstile nur für Tabs und Abrechnungs-Umschalter, nicht für Buttons und Links
- Das Logo ist ein JPG, dessen weißer Hintergrund per `mix-blend-mode` ausgeblendet wird (ein SVG wäre robuster)

© 2026 Centora · Studienprojekt an der DHBW Heidenheim
