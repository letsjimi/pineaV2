# Pinéa Linktree - Bilder-System

## Übersicht

Die Website unterstützt **optionale Bilder** für alle Überschriften und Links. Du musst keine Bilder hinzufügen - die Seite funktioniert auch ohne.

---

## Ordnerstruktur

```
pineaV2/
├── index.html
├── images/
│   └── logo.png
└── headings/          # <- Bilder für Überschriften und Links
    ├── 1.png          # Überschrift: Urlaub bei Pinéa
    ├── 1_1.png        # Link: Programm 2026
    ├── 1_2.png        # Link: Appartements
    ├── 1_3.png        # Link: Pinéa Programmgruppe e.V.
    ├── 2.png          # Überschrift: Programmarbeit unterstützen
    ├── 2_1.png        # Link: Spenden
    ├── 2_2.png        # Link: Mitgliedsantrag
    ├── 2_3.png        # Link: Zeugnis teilen
    ├── 2_4.png        # Link: Mitarbeit im Team
    └── 3.png          # Überschrift: Social Media
```

---

## Bildformat (Schema)

| Bildname | Was | Größe (empfohlen) |
|----------|-----|-------------------|
| `1.png` | Überschrift Kasten 1 | 600 x 120 px |
| `1_1.png` | 1. Link in Kasten 1 | 80 x 80 px (quadratisch) |
| `1_2.png` | 2. Link in Kasten 1 | 80 x 80 px (quadratisch) |
| `1_3.png` | 3. Link in Kasten 1 | 80 x 80 px (quadratisch) |
| `2.png` | Überschrift Kasten 2 | 600 x 120 px |
| `2_1.png` | 1. Link in Kasten 2 | 80 x 80 px (quadratisch) |
| `2_2.png` | 2. Link in Kasten 2 | 80 x 80 px (quadratisch) |
| `2_3.png` | 3. Link in Kasten 2 | 80 x 80 px (quadratisch) |
| `2_4.png` | 4. Link in Kasten 2 | 80 x 80 px (quadratisch) |
| `3.png` | Überschrift Kasten 3 | 600 x 120 px |

---

## Bildformate

- **Überschriften**: PNG, JPG, WebP - Breitformat für Header-Bilder
- **Link-Icons**: PNG mit transparentem Hintergrund empfohlen, oder JPG
- **Empfohlene Größen**:
  - Überschriften: 600 x 120 px (oder ähnliches Verhältnis)
  - Link-Icons: 80 x 80 px (quadratisch, wird als Kreis angezeigt)

---

## Wichtig

- **Bilder sind optional** - fehlende Bilder zeigen automatisch Icons an
- Wenn du ein Bild löschst, wird automatisch das Standard-Icon angezeigt
- Du kannst beliebig viele oder wenige Bilder hinzufügen
- Nur existierende Bilder werden angezeigt

---

## Beispiel

Wenn du nur `headings/1.png` und `headings/2.png` hast:
- ✅ "Urlaub bei Pinéa" zeigt dein Bild
- ✅ "Programmarbeit unterstützen" zeigt dein Bild
- ℹ️ "Social Media" zeigt das violette Icon (kein Bild vorhanden)
- ℹ️ Alle Links zeigen ihre Standard-Icons (keine Bilder vorhanden)

Wenn du `headings/1_1.png` hinzufügst:
- ✅ "Programm 2026" zeigt dein Bild statt des Kalender-Icons
