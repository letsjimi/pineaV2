# Pinéa Linktree - Bilder-System

## Übersicht

Die Website unterstützt **optionale Bilder** für alle Überschriften und Links. Du musst keine Bilder hinzufügen - die Seite funktioniert auch ohne.

---

## Aktuelle Ordnerstruktur

```
pineaV2/
├── index.html
├── images/
│   ├── logo.png          # Logo für hellen Modus
│   └── logo_blk.png      # Logo für dunklen Modus
└── headings/             # Bilder für Überschriften und Links
    ├── 1.png             # Überschrift: Urlaub in Pinéa
    ├── 1_1.png           # Link: Aktuelles Programm
    ├── 1_2.png           # Link: Programmbuchung 2026
    ├── 1_3.png           # Link: Spenden
    ├── 1_4.png           # Link: Mitgliedsantrag
    ├── 2.png             # Überschrift: Informationen
    ├── 2_1.png           # Link: Appartements
    ├── 2_2.png           # Link: Pinéa Programmgruppe e.V.
    ├── 2_3.png           # Link: Programm 2026
    ├── 2_4.png           # Link: Reisebüro
    └── 3.png             # Überschrift: Social Media
```

---

## Bild-Namen Schema

### Überschriften (Kasten)

| Bildname | Kasten | Beschreibung | Größe (empfohlen) |
|----------|--------|--------------|-------------------|
| `1.png` | Kasten 1 | Urlaub in Pinéa | 600 x 120 px |
| `2.png` | Kasten 2 | Informationen | 600 x 120 px |
| `3.png` | Kasten 3 | Social Media | 600 x 120 px |

### Links in Kasten 1 (Urlaub in Pinéa)

| Bildname | Position | Link | Größe (empfohlen) |
|----------|----------|------|-------------------|
| `1_1.png` | 1.1 | Aktuelles Programm | 80 x 80 px |
| `1_2.png` | 1.2 | Programmbuchung 2026 | 80 x 80 px |
| `1_3.png` | 1.3 | Spenden | 80 x 80 px |
| `1_4.png` | 1.4 | Mitgliedsantrag | 80 x 80 px |

### Links in Kasten 2 (Informationen)

| Bildname | Position | Link | Größe (empfohlen) |
|----------|----------|------|-------------------|
| `2_1.png` | 2.1 | Appartements | 80 x 80 px |
| `2_2.png` | 2.2 | Pinéa Programmgruppe e.V. | 80 x 80 px |
| `2_3.png` | 2.3 | Programm 2026 | 80 x 80 px |
| `2_4.png` | 2.4 | Reisebüro | 80 x 80 px |

### Social Media (ohne Bilder)

Social Media Links (Instagram, YouTube) haben feste Icons und benötigen keine Bilder.

---

## Bildformate

- **Dateiformat**: PNG mit transparentem Hintergrund empfohlen
- **Alternative**: JPG, WebP
- **Bildform**:
  - Überschriften: 
    - **Breitformat** (z.B. 600 x 120 px)
    - Bild wird links neben dem Text angezeigt (Layout: Bild links, Text rechts)
  - Link-Bilder: 
    - **Quadratisch** (z.B. 80 x 80 px)
    - **Rechteckig mit leicht abgerundeten Ecken** (6px Border-Radius)

---

## Farbpalette (für Bilder)

Die Website verwendet diese Farben:

| Farbe | HEX | Verwendung |
|-------|-----|------------|
| Creme | `#E5D2BA` | Haupttextfarbe |
| Warm Braun | `#694A42` | Hintergrund (Dark Mode) |
| Terrakotta | `#B88375` | Akzentfarbe, Buttons |
| Blau-Grau | `#455366` | Karten-Hintergrund |

---

## Bilder per GitHub hinzufügen

### Variante 1: Per Drag & Drop (einfach)

1. Gehe zu `https://github.com/letsjimi/pineaV2`
2. Klicke auf `headings/`
3. Klicke "Add file" → "Upload files"
4. Ziehe deine Bilder in den Bereich oder wähle sie aus
5. Scrolle nach unten und klicke "Commit changes"

### Variante 2: Terminal (für mehrere Bilder)

```bash
# In deinem lokalen pineaV2-Ordner
cd headings

# Bilder hinzufügen (z.B. von Downloads)
cp ~/Downloads/*.png .

# Oder neue Bilder erstellen mit einem Tool deiner Wahl

# Änderungen committen
cd ..
git add headings/
git commit -m "Neue Bilder hinzugefügt"
git push origin main
```

---

## Wichtige Hinweise

- **Bilder sind optional** - fehlende Bilder zeigen automatisch Icons an
- Wenn du ein Bild löschst, wird das Standard-Icon angezeigt
- Du kannst beliebig viele oder wenige Bilder hinzufügen
- Nur existierende Bilder werden angezeigt
- **Empfohlen**: Erstelle Bilder im Corporate Design (Creme/Terrakotta/Braun)
- **Achtung**: Stelle sicher, dass du die Berechtigung hast, die Bilder zu verwenden (keine urheberrechtlich geschützten Bilder ohne Lizenz)

---

## Beispiele

### Minimal-Setup (keine Bilder)

Keine Bilder im `headings/`-Ordner:
- Alle Kasten zeigen nur Text-Überschriften
- Alle Links zeigen Standard-Icons an
- Schlicht, funktional, schnell geladen

### Full-Setup (alle Bilder)

Alle Bilder vorhanden:
- Jede Überschrift hat ein individuelles Bild
- Jeder Link hat ein individuelles Bild
- Visuell ansprechend, aber mehr Pflegeaufwand

### Misch-Setup (empfohlen)

Nur einige Bilder:
- `1.png`, `2.png`, `3.png` → Überschriften mit Bild
- `1_1.png` → Aktuelles Programm mit Bild
- Andere Links zeigen Icons
- Guter Kompromiss aus Optik und Pflege

---

## Technische Details

- Bilder werden per `onerror` Event ausgeblendet, wenn sie fehlen
- Maximale Bildgröße für Links: 40 x 40 px Anzeige
- Überschriften-Bilder skalieren automatisch
- **Cache**: Nach dem Upload kann es 5-10 Minuten dauern, bis die Bilder auf der Website erscheinen (GitHub Pages Cache)

---

## Fehlerbehebung

| Problem | Lösung |
|---------|--------|
| Bild wird nicht angezeigt | Prüfe Dateinamen (z.B. `1_1.png` nicht `1_1.PNG`) |
| Bild ist verschoben | Nutze PNG mit transparentem Hintergrund |
| Bild wird nach Upload nicht angezeigt | Warte 5-10 Min. (GitHub Pages Cache) oder drücke Strg+F5 |
| Bild ist zu groß/klein | Optimiere auf 80x80 px (Links) oder 600x120 px (Überschriften) |
| Bild hat weißen Hintergrund | Speichere mit transparentem Hintergrund (PNG) |

---

*Letzte Aktualisierung: 2026*
