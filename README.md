# SAJON Publishing — Website & Design-System

Der Webauftritt des **Verlagsteils der Sajon GmbH**. Akademische, qualitativ hochstehende
Schriften: Editieren, Gestalten, Lektorieren, Konvertieren (E-Book) und Veröffentlichen.

**Live:** https://jonason92.github.io/sajon-publishing/ (GitHub Pages)

## Struktur

```
sajon-publishing/
├── index.html                  ← Startseite
├── leistungen.html             ← Leistungen (4 Kernleistungen + Workflow)
├── ueber-uns.html              ← Über uns (Geschichte, Team, Statistiken)
├── portfolio.html              ← Portfolio (8 Bücher, Filter-Tabs)
├── kontakt.html                ← Kontakt (Jonas, ORCID, Formular, Karte)
├── css/
│   └── sajon-design-system.css ← Zentrales Stylesheet
├── assets/
│   ├── narwhal.svg             ← Logo (Narwal)
│   └── covers/                 ← 27 Buchcover
└── README.md                   ← Diese Dokumentation
```

## Design-Token (Farben)

| Token | Wert | Verwendung |
| --- | --- | --- |
| `--emerald` | `#0d7a52` | Primär-Akzent (Smaragdgrün) |
| `--emerald-bright` | `#10b981` | Hover, aktiv, Sterne |
| `--emerald-dark` | `#0a5c3e` | dunkler Akzent |
| `--emerald-tint` | `#e6f3ee` | Hero-Hintergrund |
| `--ice` | `#cfe8f2` | Eisblauer Streifen |
| `--ice-deep` | `#7fb8cf` | Eisblau (dunkel) |
| `--ice-light` | `#e9f4f8` | Eisblau (hell) |
| `--ink` | `#16201a` | Text |
| `--ink-soft` | `#3d4a43` | Fließtext |
| `--muted` | `#6b7a71` | sekundärer Text |
| `--paper` | `#fbfaf7` | Hintergrund |
| `--paper-2` | `#f4f2eb` | Alternativ-Sektionen |
| `--line` | `#e2e6e0` | Trennlinien |
| `--card` | `#ffffff` | Karten |

## Typografie

| Token | Wert | Einsatz |
| --- | --- | --- |
| `--serif` | Georgia, Iowan Old Style, Palatino Linotype, Book Antiqua, serif | Überschriften (akademisch) |
| `--sans` | system-ui, Segoe UI, Roboto, sans-serif | Fließtext, UI |

## Design-Motive

- **Narwal** — Logo (`assets/narwhal.svg`), in Navigation und Hero.
- **Smaragdgrüner Balken** — Akzentfarbe für Buttons, Hover, Trennlinien, Prozess-Indikatoren.
- **Eisblauer Streifen** — dekorativer Divider (`.ice-stripe`) unter dem Hero.
- **Ornament-Sterne** (✻✻✻✻✻) — wiederkehrendes Motiv in Badges, Sektions-Köpfen und Footer.

## Komponenten (CSS-Klassen)

- `.site-header` / `.nav` / `.brand` / `.nav-links` — Navigation
- `.hero` / `.eyebrow` / `.ice-stripe` — Hero
- `.btn` `.btn-primary` `.btn-ghost` — Buttons
- `.grid` / `.card` / `.card-link` — Karten
- `.stats` / `.stat` — Statistiken
- `.workflow` / `.step` — Prozessschritte (Leistungen)
- `.tabs` / `.tab` / `.book` — Portfolio-Filter
- `.form` / `.two-col` — Kontaktformular
- `.site-footer` — Footer

## Logo (Narwal)

Das offizielle Logo ist der **originale Sajon-GmbH-Narwal** (`assets/logo.png`, Quelle:
`Logo_pic.PNG` aus dem Plattform-Repo). Das zuvor verwendete, selbst erstellte
Platzhalter-Logo bleibt aus historischen Gründen erhalten: `assets/narwhal.svg`.

## Verwendungsanleitung für andere SAJON-Sparten

1. `css/sajon-design-system.css` und `assets/narwhal.svg` in das neue Projekt kopieren.
2. Die Farb-Token `--emerald` / `--ice` bei Bedarf an die Sparten-Farbe anpassen
   (alle Komponenten folgen automatisch).
3. Eigene HTML-Seiten mit denselben Klassen (`.hero`, `.card`, `.btn`, …) aufbauen.

## Deploy (GitHub Pages)

Settings → Pages → Source: **Deploy from a branch** → `main` → **/ (root)**.

## Offene Punkte (zu ergänzen)

- Weitere Portfolio-Titel aus dem 55-Titel-Katalog.
