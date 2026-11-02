# Auswertung R02 (Projekt Karlstadt)

Quelle: `DJI_20260914132335_0004` (Ordner `DJI_202609141313_001`), Flug von Ost nach West, 117,6 s (`_S` kombiniert, `_T` nur Thermal, `_V` normal). Thermalvideo ohne Radiometrie (Farbbild).
R02 hat 6 Gestelle, 108 Positionen, IDs 55 bis 162 (ID = 54 + Positionsnummer).

## Positionszuordnung
Gestelllücken im Bild bei ca. 18 s (R02-090|091), 45 s (072|073), 68 s (054|055), 81 s (036|037) und 96 s (018|019). Die Drohne fliegt nicht gleichmäßig, die Zeit-Position-Beziehung ist nicht linear. Positionen sind durch Zählen der Modulreihen ab der nächsten Gestelllücke bestimmt, Genauigkeit ±1 Position; die Positionen wurden vom Auftraggeber anhand der Kontrollbilder bestätigt.
Ebenen: rechts im Bild = Nord = Ebene 0, links = Ebene 2. Kachelzeile 0 = Nordseite; Kachelspalte 0 = Westseite.
Stufen: weiß = 3, gelb/orange (schwächer) = 1.

## Befunde
| Nr | Zeit | Position | Ebene | Zeile / Spalte | Stufe | Begründung | Bild |
|---|---|---|---|---|---|---|---|
| 1 | 12–21 s | R02-093 | 2 | Zeile 10, Spalte 0 | 3 | einzelne weiße Zelle, über ca. 15 Frames fest | `chk_t18.0.jpg` |
| 2 | 12–21 s | R02-093 | 2 | Zeile 1, Spalte 2 | 3 | einzelne weiße Zelle, über ca. 18 Frames fest | `chk_t18.0.jpg` |
| 3 | 12–21 s | R02-093 | 2 | Zeile 2, Spalte 2 | 1 | orange Nachbarzelle von Nr. 2 | `chk_t18.0.jpg` |
| 4 | 42–46 s | R02-073 | 1 | Zeile 8, Spalte 3 | 3 | einzelne weiße Zelle, ca. 8 Frames | `chk_t45.0.jpg` |
| 5 | 37,5–45,5 s | R02-076 | 0 | Zeile 6, Spalte 3 | 3 | einzelne weiße Zelle, ca. 17 Frames | `chk_t45.0.jpg` |
| 6 | 50–54 s | R02-070 | 2 | Zeile 5 und 3, Spalte 0 | 1 | zwei gelbliche Zellen | `chk_t51.0.jpg`, `chk_t54.0.jpg` |
| 7 | 52,5–57,5 s | R02-066 | 1 | Zeile 3, Spalte 2 (weiß) und Zeile 2, Spalte 2 (gelb) | 3 / 1 | weißes Zellpaar, ca. 11 Frames | `chk_t54.0.jpg` |
| 8 | 51,5–55,5 s | R02-067 | 0 | Zeile 11, Spalte 2 und 4 | 1 | zwei gelbe Zellen untereinander | `chk_t54.0.jpg` |
| 9 | 67,5–71,5 s | R02-052 | 0 | Zeile 11, Spalte 2 (weiß) und Zeile 10, Spalte 2 (gelb) | 3 / 1 | weiße Zelle mit gelber Nachbarzelle, am Rand zu Ebene 1 | `chk_t68.0.jpg` |
| 10 | 89–94 s | R02-023 | 2 | Zeile 5, Spalte 1 (weiß); Zeile 6, Spalte 1 (gelb); Zeile 1, Spalte 3 (weiß) | 3 / 1 / 3 | weiße Zellen, ca. 10 Frames | `chk_t93.0.jpg` |
| 11 | 88,5–92,5 s | R02-024 | 1 | Zeile 11, Spalte 3 | 3 | einzelne weiße Zelle | `chk_t90.5.jpg` |
| 12 | 89–92 s | R02-024 | 1 | Zeile 1 und 2, Spalte 1 | 3 | Zellpaar | `chk_t90.5.jpg` |

**Unsicher:** Zeile und Spalte der Zellen sind nur grob geschätzt (±2); Positionen ±1.

## Nicht eingetragen
- Mehrere orange, rundliche Flecken in der rechten Spalte bei ca. 90–93 s (R02-024, ca. 5 Stück, `chk_t90.5.jpg`): schwächer als gelbe Zellen, Einstufung offen.

## Verworfen
- Heller Fleck oben rechts: in fast jedem Frame an derselben Bildstelle, wandert mit der Kamera mit (Spiegelung). Echte Zellen im selben Bildbereich wären nur an ihrer Bewegung erkennbar.
- Warme Flecken bei ca. 25–28,5 s und 66 s: in den Frames 3 s davor und danach nicht vorhanden, daher kein fester Befund (vermutlich Helligkeitsanpassung der Kamera).
- Kein Streifen wie in R01 gefunden.
- Übersichten: `bilder/kontakt_R02_1.jpg`, `bilder/kontakt_R02_2.jpg`.
