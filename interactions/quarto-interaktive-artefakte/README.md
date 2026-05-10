# Quarto-Erweiterung: 10 interaktive Spiele und Artefakte

Dieses Mini-Paket enthält 10 eigenständige HTML-Widgets für ein Quarto-Skript zum Thema iFrames, Spiele und KI-Tutor.

## Ordnerstruktur

```text
projektwurzel/
├─ _quarto.yml
├─ parts/
│  └─ 05-iframes-tutor-erweiterung.qmd
└─ interactions/
   ├─ iframe-debug-escape-room.html
   ├─ embed-entscheidungsspiel.html
   ├─ quarto-pfad-puzzle.html
   ├─ tutor-prompt-klinik.html
   ├─ misskonzept-detektiv.html
   ├─ widget-generator.html
   ├─ didaktik-bingo.html
   ├─ kursdesigner-simulation.html
   ├─ feedback-qualitaet-spiel.html
   └─ publish-readiness-check.html
```

## Wichtig in `_quarto.yml`

Damit Quarto die HTML-Dateien in den gerenderten Output kopiert, muss unter `project:` diese Zeile stehen:

```yaml
project:
  type: website
  output-dir: docs
  resources: ["interactions/*"]
```

Falls in Ihrem Projekt bereits `resources:` existiert, ergänzen Sie `"interactions/*"` in der bestehenden Liste.

## Einbau in ein `.qmd`-Kapitel

Wenn Ihr Kapitel im Ordner `parts/` liegt, verwenden Sie:

```html
<iframe src="../interactions/iframe-debug-escape-room.html"
        width="100%" height="760" frameborder="0"
        style="border: 1px solid #e6e6ea; border-radius: 12px;">
</iframe>
```

Wenn Ihr Kapitel in der Projektwurzel liegt, verwenden Sie stattdessen:

```html
<iframe src="interactions/iframe-debug-escape-room.html"
        width="100%" height="760" frameborder="0"
        style="border: 1px solid #e6e6ea; border-radius: 12px;">
</iframe>
```

## Hinweise

- Alle Widgets sind statische HTML-Dateien mit eingebettetem CSS und JavaScript.
- Sie speichern keine Daten dauerhaft.
- Sie benötigen keine externen Bibliotheken.
- Die Höhe der iFrames kann je nach Layout angepasst werden.
