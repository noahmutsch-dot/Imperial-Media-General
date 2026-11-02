# Auswertung R01 (Projekt Karlstadt)

Quelle: `DJI_20260914131956_0002` (Ordner `DJI_202609141313_001`), Flug von Ost nach West, 57 s.
Hotspot-Erkennung auf dem Thermalvideo (`_T`), normales Video (`_V`) zur Gegenprüfung; Kombination `_S`.

## Videos
| Datei | Rolle | Auflösung | Dauer |
|---|---|---|---|
| `_S` | Thermal und normal nebeneinander | 1920×1080 | 57,0 s |
| `_T` | nur Thermal | 1280×1024 | 57,1 s |
| `_V` | nur normal | 3840×2160 | 57,1 s |

Das Thermalvideo ist ein Farbbild (HEVC, automatische Kontrastspreizung), **nicht radiometrisch**. Es zählt nur der Vergleich mit der Umgebung.

## Positionszuordnung
Gestelllücken im Bild: ca. 12–18 s (zwischen R01-036 und -037) und ca. 27–33 s (zwischen R01-018 und -019). Start am Ostende (R01-054), Westende bei ca. 54 s (R01-001). Die Drohne fliegt nicht gleichmäßig (30–40 s fast Stillstand), deshalb ist Zeit → Position nicht linear; Positionen sind durch Zählen der Modulreihen ab Gestelllücke bzw. Reihenende bestimmt, Genauigkeit ±1 bis 2 Positionen. Keine GPS-Daten (.SRT) vorhanden.
Ebenen: Flug nach Westen, Kamera nach unten, also rechts im Bild = Nord = Ebene 0, links = Ebene 2.

## Befunde
Stufe 3 = sehr auffällig; im Zweifel niedrigere Stufe (1).

| Nr | Zeit im Video | Position | Ebene | Kachelzeile / -spalte | Stufe | Begründung | Bild |
|---|---|---|---|---|---|---|---|
| P1 | 6,5–17 s | R01-039 | 2 (Rand zu 1) | Zeile ca. 0, Spalte ca. 2 | 3 | Einzelne sehr helle Zelle, bleibt über ca. 20 Frames an derselben Zelle | `bilder/count_P1_t12.0.jpg` |
| P2 | 18–25,5 s | R01-029 | 0 | Zeile ca. 7, Spalte ca. 2 | 3 | Einzelne sehr helle Zelle, über ca. 15 Frames verfolgt | `bilder/count_P2_t18.5.jpg` |
| P3 | 23–27,5 s | R01-027 | 1 | Zeile ca. 7, Spalte ca. 2 | 3 | Einzelne sehr helle Zelle, über ca. 10 Frames verfolgt | `bilder/count_P3_t23.5.jpg` |
| P4 | 52–56,5 s | R01-003 | 2 (Rand zu 1) | Zeile ca. 0, Spalte ca. 2 | 3 | Einzelne sehr helle Zelle (vom Auftraggeber bestätigt), über ca. 9 Frames verfolgt | `bilder/Bsp_A_t53.0.jpg` |
| A | 52–54 s | R01-006 | 1 | alle 12 Zeilen; Spalte 0 (Stufe 3), Spalte 1 (Stufe 1, Zweifel) | 3 / 1 | Heller Streifen quer über das Modul, bleibt in den Frames 52–54 s am selben Modul | `bilder/Bsp_A_t53.0.jpg` |

**Unsicher:** Die Kachelzeile/-spalte der Punkte ist nur grob geschätzt (Spalte jeweils auf 2 gesetzt, wo keine bessere Angabe möglich war). Position ±1–2.

## Verworfene Kandidaten
- Sonnenspiegelung am unteren Bildrand, ca. 5–41 s (im normalen Video sichtbar): kein Befund.
- Warme Module ohne einzelne helle Zelle (z. B. 1,0 s, Bilder B und C; 33,5 s Bild D; 5,0 s Bild H): als warmes Modul, nicht als Hotspot gewertet (`bilder/Bsp_B_t1.0.jpg`, `Bsp_C_t1.0.jpg`, `Bsp_D_t33.5.jpg`, `Bsp_H_t5.0.jpg`).
- Übersteuerte Phasen bei 0,5–5 s und 33–34,5 s: nicht auswertbar.
- Übersicht: `bilder/kontakt_R01.jpg`.
