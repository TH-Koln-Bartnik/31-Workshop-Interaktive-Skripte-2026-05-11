# Interaktive Skripte mit KI erstellen

Werkstatt-Skript zum Workshop am 11.05.2026 an der TH Köln (hdw nrw, 26-157-P-Z).
Referent: Prof. Dr. Roman Bartnik.

Dieses Repository ist gleichzeitig **Lehrmaterial** und **Vorlage** —
die Teilnehmenden bauen im Workshop ein Skript dieser Art selbst auf.

## Schnellstart (für Lesende)

Online-Version: <https://th-koln-bartnik.github.io/interaktive-skripte-2026/>

## Schnellstart (für die Workshop-Vorbereitung)

```bash
# Build
quarto render

# Preview
quarto preview

# Publish nach GitHub Pages
quarto publish gh-pages
```

## Struktur (Lakens-Konvention)

```
.
├── _quarto.yml             # Buch-Konfiguration
├── _brand.yml              # TH Köln Farben & Typografie
├── styles.scss             # SCSS-Ergänzungen (TH-Köln-Brand)
├── references.bib          # Zotero-Export
├── index.qmd               # Landing Page mit Lernzielen
├── parts/                  # Workshop-Kapitel 1–6
├── appendix/               # Quickstart, Troubleshooting, Tutor-Prompt
├── images/                 # Logos, Screenshots, statische Grafiken
├── interactions/           # HTML-Widgets (Lernspiel, Memory)
├── include/                # Wiederverwendbare qmd-Partials
└── data/                   # CSV/JSON-Daten für interaktive Charts
```

## Lizenz

Inhalte: CC BY-SA 4.0. Code: MIT.
