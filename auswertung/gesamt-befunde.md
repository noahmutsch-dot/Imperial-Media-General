# Auswertung Gesamtanlage (Projekt Karlstadt / Laudenbach)

Alle 24 Reihen aus den Ordnern `DJI_202609141313_001` bis `DJI_202609141556_005` (Breisgau Power 1). R01 und R02 wurden erneut automatisch ausgewertet und mit den bestätigten Befunden verglichen.

## Clips je Reihe
| Reihe | Clip (nur Thermal) | Dauer | Flugrichtung |
|---|---|---|---|
| R01 | `DJI_20260914131956_0002_T.MP4` | 57 s | Ost → West |
| R02 | `DJI_20260914132335_0004_T.MP4` | 118 s | Ost → West |
| R03 | `DJI_20260914132640_0005_T.MP4` | 206 s | West → Ost |
| R04 | `DJI_20260914133116_0006_T.MP4` | 175 s | Ost → West |
| R05 | `DJI_20260914133447_0007_T.MP4` | 45 s | Ost → West |
| R06 | `DJI_20260914133627_0008_T.MP4` | 522 s | West → Ost |
| R07 | `DJI_20260914135259_0001_T.MP4` | 332 s | Ost → West |
| R08 | `DJI_20260914135903_0002_T.MP4` | 517 s | West → Ost |
| R09 | `DJI_20260914140815_0003_T.MP4` | 354 s | Ost → West |
| R10 | `DJI_20260914142434_0001_T.MP4` | 392 s | West → Ost |
| R11 | `DJI_20260914143207_0002_T.MP4` | 281 s | Ost → West |
| R12 | `DJI_20260914143706_0003_T.MP4` | 312 s | West → Ost |
| R13 | `DJI_20260914144306_0004_T.MP4` | 258 s | Ost → West |
| R14 | `DJI_20260914151946_0001_T.MP4` | 285 s | West → Ost |
| R15 | `DJI_20260914152517_0002_T.MP4` | 218 s | Ost → West |
| R16 | `DJI_20260914152930_0003_T.MP4` | 280 s | West → Ost |
| R17 | `DJI_20260914153504_0004_T.MP4` | 251 s | Ost → West |
| R18 | `DJI_20260914153936_0005_T.MP4` | 286 s | West → Ost |
| R19 | `DJI_20260914155845_0001_T.MP4` | 271 s | Ost → West |
| R20 | `DJI_20260914160352_0002_T.MP4` | 159 s | West → Ost |
| R21 | `DJI_20260914160658_0003_T.MP4` | 168 s | Ost → West |
| R22 | `DJI_20260914161007_0004_T.MP4` | 138 s | West → Ost |
| R23 | `DJI_20260914161228_0005_T.MP4` | 60 s | Ost → West |
| R24 | `DJI_20260914161407_0006_T.MP4` | 76 s | West → Ost |

## Vorgehen
- Telemetrie aus den MP4-Dateien (GPS, Höhe, Kamerawinkel, 30 Datensätze pro Sekunde) ausgelesen; Reihenreihenfolge und Flugrichtung daraus bestimmt.
- Layout des Tools über die bestätigten Gestelllücken von R02 auf GPS-Koordinaten gelegt (Restfehler < 0,6 m).
- Je Reihe: Reihenenden und Gestelllücken im Video erkannt und daraus Start und Gestellabstand (15,3–15,8 m) bestimmt.
- Frames (2 pro Sekunde) auf weiße/gelbe Einzelzellen durchsucht; ein Befund zählt nur, wenn er am Boden fest bleibt (mind. 4 Frames, über ≥ 1 s und deutliche Bildbewegung). Spiegelungen wandern mit der Kamera und fallen dadurch heraus.
- Filter: Kontrast zum Umfeld in alle Richtungen, kompakte Form (keine Längsstreifen), Randstreifen zum Gras ausgeschlossen. Danach alle Kandidaten einzeln gesichtet.

## Genauigkeit (siehe auch Doppelte Prüfung)
- Reihe und Gestell: sicher. Position innerhalb des Gestells: in der Regel ±1, bei schräger Kamera (Neigung -50° bis -70°) bis ±2. Ebene: aus der Lage im Gestellbild, meist sicher.
- Kachelzeile und -spalte sind grob geschätzt (±2).

## Kontrolle R01 und R02
Die bestätigten Befunde bleiben unverändert eingetragen. Die automatische Auswertung findet sie wieder (Abweichung höchstens 1 Position):
- R01: automatisch gefunden bei R01-028, R01-029, R01-040
- R02: automatisch gefunden bei R02-023, R02-024, R02-052, R02-074, R02-076, R02-093
- Abgleich: R01-029, R02-023, -024, -052, -076, -093 identisch; R01-027 ↔ 028, R01-039 ↔ 040, R02-073 ↔ 074 (je 1 Position Abweichung, bestätigter Wert bleibt).
- Nicht automatisch gefunden: R01-003 und der Streifen R01-006 (Anfangs- und Endbereich übersteuert), R02-066 (Zellpaar, zu länglich für den Formfilter), R02-067/070 (gelbe Zellen).
- Folgerung für R03–R24: Positionen dort sind ebenfalls auf etwa ±1 genau; Zellpaare, Streifen und schwache gelbe Zellen können fehlen.

## Doppelte Prüfung der Positionen
- **Bild geprüft (63 Befunde):** Position durch Zählen der Modulstränge ab einer im selben Videobild sichtbaren Gestelllücke bestimmt; 37 strittige Fälle zusätzlich einzeln von Hand nachgezählt. Methode an R02 (bekannte Positionen) ohne Fehler getestet.
- **nur GPS (141 Befunde):** Im Videobild ist keine Gestelllücke zu sehen; Position aus GPS/Kameramodell. Abgleich an den geprüften Fällen zeigt Abweichungen von −4 bis +2 Positionen (meist ±1–2), ohne festes Muster. **Diese Positionen bitte prüfen** (im PDF orange markiert).
- **unklar (2 Befunde, #130, #153):** Lücke im Bild nicht eindeutig.
- PDF zum Prüfen: `Karlstadt-Thermografie.pdf` (Vektor, beliebig zoombar; Seite 1 Gesamtübersicht, danach je Reihe Detailplan, Tabelle und Videoausschnitte in voller Auflösung mit Positionsnummer/Ebene an jeder Zelle).

## Befunde R03 bis R24
Jede helle Zelle ist einzeln markiert (weiß = Stufe 3, gelb = Stufe 1).

| # | Reihe | Zeit im Video | Position(en) | Ebene(n) | Zellen weiß / gelb | Prüfung | Hinweis |
|---|---|---|---|---|---|---|---|
| 13 | R03 | 20–22 s | R03-031 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 14 | R03 | 19–20 s | R03-032 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 15 | R03 | 17–19 s | R03-034 | 1 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 16 | R03 | 17–18 s | R03-034 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 17 | R03 | 20–30 s | R03-036 | 0 | 0 / 1 | nur GPS (±1–3), prüfen | Position geschätzt |
| 18 | R03 | 28–31 s | R03-039, R03-040 | 1, 2 | 3 / 0 | Bild geprüft | Rand/Bewuchs |
| 19 | R03 | 56–57 s | R03-062, R03-063 | 0, 1, 2 | 7 / 0 | nur GPS (±1–3), prüfen |  |
| 20 | R03 | 56–57 s | R03-062, R03-063 | 0, 1, 2 | 6 / 0 | nur GPS (±1–3), prüfen |  |
| 21 | R03 | 55–58 s | R03-062, R03-063 | 0, 1, 2 | 6 / 0 | nur GPS (±1–3), prüfen |  |
| 22 | R03 | 49–56 s | R03-062, R03-063 | 0, 1, 2 | 7 / 0 | nur GPS (±1–3), prüfen |  |
| 23 | R03 | 48–54 s | R03-063, R03-064 | 0, 1, 2 | 7 / 0 | nur GPS (±1–3), prüfen |  |
| 24 | R03 | 48–54 s | R03-063, R03-064 | 0, 1, 2 | 7 / 0 | nur GPS (±1–3), prüfen |  |
| 25 | R03 | 48–54 s | R03-063, R03-064 | 0, 1, 2 | 7 / 0 | nur GPS (±1–3), prüfen |  |
| 28 | R03 | 81–88 s | R03-093 | 2 | 2 / 1 | Bild geprüft |  |
| 27 | R03 | 83–88 s | R03-095 | 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 29 | R03 | 90–91 s | R03-101 | 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 30 | R03 | 94–96 s | R03-106 | 2 | 2 / 0 | Bild geprüft |  |
| 31 | R03 | 92–93 s | R03-108 | 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 33 | R03 | 126–128 s | R03-123 | 2 | 1 / 0 | Bild geprüft |  |
| 34 | R03 | 121–125 s | R03-125 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 35 | R03 | 165–167 s | R03-142 | 2 | 1 / 0 | Bild geprüft |  |
| 37 | R03 | 165–169 s | R03-145 | 2 | 1 / 0 | Bild geprüft |  |
| 36 | R03 | 166–168 s | R03-146 | 2 | 1 / 2 | nur GPS (±1–3), prüfen |  |
| 38 | R03 | 175–178 s | R03-156 | 0 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 39 | R03 | 175–178 s | R03-156 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 40 | R03 | 175–179 s | R03-157 | 1 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 41 | R04 | 96–97 s | R04-109 | 0 | 2 / 0 | Bild geprüft |  |
| 42 | R04 | 27–31 s | R04-182 | 0 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 43 | R04 | 29–31 s | R04-182 | 2 | 1 / 0 | Bild geprüft |  |
| 44 | R04 | 9–14 s | R04-201, R04-202 | 0, 1, 2 | 3 / 2 | Bild geprüft |  |
| 45 | R04 | 11–13 s | R04-201, R04-202 | 1, 2 | 4 / 0 | nur GPS (±1–3), prüfen |  |
| 47 | R04 | 6–9 s | R04-207 | 1 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 48 | R05 | 29–40 s | R05-014 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 49 | R06 | 5–25 s | R06-011, R06-013 | 0, 2 | 1 / 1 | nur GPS (±1–3), prüfen |  |
| 50 | R06 | 10–24 s | R06-012 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 51 | R06 | 15–19 s | R06-013 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 52 | R06 | 5–39 s | R06-014 | 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 53 | R06 | 35–42 s | R06-017 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 57 | R06 | 33–62 s | R06-020, R06-021, R06-023, R06-025 | 0, 1, 2 | 3 / 4 | nur GPS (±1–3), prüfen |  |
| 59 | R06 | 58–61 s | R06-030, R06-032, R06-034, R06-035 | 1 | 2 / 6 | nur GPS (±1–3), prüfen |  |
| 60 | R06 | 203–214 s | R06-093 | 0, 2 | 3 / 1 | Bild geprüft |  |
| 63 | R06 | 349–355 s | R06-199 | 2 | 1 / 1 | Bild geprüft |  |
| 66 | R06 | 346–357 s | R06-199 | 1 | 1 / 0 | Bild geprüft |  |
| 64 | R06 | 350–355 s | R06-200 | 2 | 1 / 0 | Bild geprüft |  |
| 65 | R06 | 350–355 s | R06-200 | 1 | 1 / 0 | Bild geprüft |  |
| 67 | R06 | 365–367 s | R06-216 | 1 | 1 / 0 | Bild geprüft |  |
| 68 | R06 | 383–387 s | R06-241 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 70 | R06 | 393–394 s | R06-250 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 69 | R06 | 389–394 s | R06-250, R06-251 | 2 | 5 / 0 | Bild geprüft | Rand/Bewuchs |
| 71 | R06 | 404–408 s | R06-269 | 1 | 1 / 0 | Bild geprüft |  |
| 72 | R06 | 406–409 s | R06-270 | 1 | 1 / 0 | Bild geprüft | Position geschätzt |
| 73 | R06 | 415–418 s | R06-282 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 75 | R06 | 430–440 s | R06-303 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 76 | R06 | 434–443 s | R06-308 | 0 | 2 / 0 | Bild geprüft |  |
| 78 | R06 | 475–477 s | R06-336, R06-337 | 0, 1 | 2 / 2 | nur GPS (±1–3), prüfen |  |
| 77 | R06 | 472–478 s | R06-337, R06-338 | 1, 2 | 3 / 0 | nur GPS (±1–3), prüfen |  |
| 79 | R06 | 469–472 s | R06-338 | 1, 2 | 4 / 0 | nur GPS (±1–3), prüfen |  |
| 80 | R06 | 473–479 s | R06-338 | 0 | 0 / 1 | nur GPS (±1–3), prüfen |  |
| 81 | R06 | 480–482 s | R06-341 | 2 | 1 / 0 | Bild geprüft |  |
| 82 | R06 | 486–489 s | R06-350 | 0 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 83 | R06 | 490–493 s | R06-353 | 1 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 84 | R06 | 488–490 s | R06-354 | 1 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 85 | R06 | 498–501 s | R06-360 | 2 | 1 / 0 | nur GPS (±1–3), prüfen | Position geschätzt |
| 86 | R07 | 159–162 s | R07-226 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 88 | R07 | 135–138 s | R07-256 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 89 | R07 | 121–126 s | R07-270 | 2 | 1 / 0 | Bild geprüft | Position geschätzt |
| 90 | R07 | 118–121 s | R07-272 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 92 | R07 | 120–123 s | R07-272 | 1 | 1 / 0 | Bild geprüft |  |
| 91 | R07 | 118–123 s | R07-273 | 1 | 1 / 0 | Bild geprüft |  |
| 93 | R07 | 103–110 s | R07-287 | 2 | 0 / 1 | nur GPS (±1–3), prüfen |  |
| 94 | R07 | 101–106 s | R07-288, R07-289 | 2 | 3 / 0 | nur GPS (±1–3), prüfen |  |
| 95 | R07 | 102–104 s | R07-290, R07-291 | 2 | 2 / 0 | Bild geprüft |  |
| 96 | R07 | 101–105 s | R07-290, R07-291 | 2 | 2 / 0 | Bild geprüft |  |
| 97 | R07 | 100–107 s | R07-291 | 2 | 2 / 0 | Bild geprüft |  |
| 98 | R07 | 103–107 s | R07-291, R07-292 | 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 99 | R07 | 97–105 s | R07-291 | 2 | 1 / 0 | Bild geprüft |  |
| 100 | R07 | 99–103 s | R07-294, R07-295 | 2 | 0 / 2 | nur GPS (±1–3), prüfen |  |
| 101 | R07 | 96–99 s | R07-298, R07-299 | 1, 2 | 3 / 2 | nur GPS (±1–3), prüfen |  |
| 102 | R07 | 97–98 s | R07-298, R07-299 | 1, 2 | 4 / 2 | nur GPS (±1–3), prüfen |  |
| 103 | R07 | 71–73 s | R07-321 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 104 | R07 | 74–75 s | R07-322 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 105 | R07 | 68–77 s | R07-324 | 2 | 1 / 0 | Bild geprüft |  |
| 106 | R07 | 68–70 s | R07-324, R07-326 | 1, 2 | 3 / 2 | Bild geprüft |  |
| 107 | R07 | 69–71 s | R07-324 | 1, 2 | 3 / 1 | Bild geprüft |  |
| 108 | R07 | 71–73 s | R07-324, R07-325 | 1, 2 | 2 / 1 | Bild geprüft |  |
| 109 | R07 | 71–73 s | R07-324 | 1, 2 | 3 / 1 | Bild geprüft |  |
| 110 | R07 | 73–75 s | R07-324 | 1, 2 | 3 / 1 | Bild geprüft |  |
| 111 | R07 | 73–75 s | R07-324 | 1, 2 | 3 / 1 | Bild geprüft |  |
| 112 | R07 | 62–72 s | R07-326, R07-327 | 2 | 2 / 0 | Bild geprüft |  |
| 113 | R07 | 58–60 s | R07-331 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 114 | R07 | 59–60 s | R07-331, R07-332 | 1, 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 115 | R07 | 61–64 s | R07-331, R07-332 | 0, 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 116 | R07 | 61–63 s | R07-332, R07-333 | 1, 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 117 | R07 | 62–66 s | R07-333 | 0, 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 118 | R07 | 64–65 s | R07-333, R07-334 | 1, 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 119 | R07 | 53–55 s | R07-336 | 1, 2 | 1 / 1 | nur GPS (±1–3), prüfen |  |
| 120 | R07 | 57–59 s | R07-336 | 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 121 | R07 | 55–59 s | R07-337 | 1, 2 | 1 / 1 | nur GPS (±1–3), prüfen |  |
| 122 | R07 | 57–58 s | R07-337, R07-338 | 1, 2 | 1 / 2 | nur GPS (±1–3), prüfen |  |
| 123 | R07 | 41–46 s | R07-347 | 1 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 124 | R07 | 39–46 s | R07-349 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 125 | R07 | 43–45 s | R07-350 | 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 126 | R07 | 0–5 s | R07-378 | 0, 1, 2 | 3 / 2 | nur GPS (±1–3), prüfen |  |
| 127 | R07 | 0–6 s | R07-378 | 0, 1, 2 | 3 / 0 | nur GPS (±1–3), prüfen |  |
| 128 | R07 | 1–5 s | R07-378 | 0, 1 | 4 / 0 | nur GPS (±1–3), prüfen | Position geschätzt |
| 129 | R08 | 262–266 s | R08-205, R08-206 | 1, 2 | 3 / 0 | nur GPS (±1–3), prüfen |  |
| 130 | R08 | 279–303 s | R08-216, R08-217 | 1, 2 | 4 / 2 | unklar, prüfen |  |
| 131 | R08 | 278–301 s | R08-218 | 1, 2 | 4 / 0 | Bild geprüft |  |
| 132 | R08 | 293–301 s | R08-218, R08-221 | 0, 1, 2 | 5 / 2 | Bild geprüft |  |
| 133 | R08 | 280–298 s | R08-218, R08-219 | 0, 1, 2 | 3 / 1 | Bild geprüft |  |
| 134 | R08 | 280–298 s | R08-219, R08-220 | 1, 2 | 2 / 5 | Bild geprüft |  |
| 135 | R08 | 311–317 s | R08-229 | 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 136 | R08 | 318–322 s | R08-235 | 0 | 1 / 0 | Bild geprüft |  |
| 137 | R08 | 328–337 s | R08-245, R08-246 | 1, 2 | 3 / 1 | nur GPS (±1–3), prüfen | Rand/Bewuchs |
| 138 | R08 | 327–342 s | R08-247 | 1, 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 140 | R08 | 326–341 s | R08-247, R08-248 | 1, 2 | 3 / 3 | Bild geprüft | Rand/Bewuchs |
| 141 | R08 | 326–341 s | R08-248, R08-249 | 1, 2 | 3 / 0 | Bild geprüft |  |
| 139 | R08 | 327–342 s | R08-248, R08-249 | 1, 2 | 3 / 2 | Bild geprüft | Rand/Bewuchs |
| 144 | R08 | 343–346 s | R08-253, R08-254, R08-255 | 0, 2 | 3 / 1 | Bild geprüft |  |
| 142 | R08 | 345–348 s | R08-255, R08-256 | 2 | 3 / 0 | nur GPS (±1–3), prüfen |  |
| 143 | R08 | 345–348 s | R08-255, R08-256, R08-257 | 1, 2 | 5 / 0 | nur GPS (±1–3), prüfen |  |
| 145 | R08 | 343–345 s | R08-255, R08-256 | 2 | 2 / 0 | Bild geprüft |  |
| 146 | R08 | 346–353 s | R08-261, R08-262 | 2 | 2 / 1 | nur GPS (±1–3), prüfen |  |
| 147 | R08 | 410–412 s | R08-308, R08-309, R08-310 | 0, 1 | 1 / 2 | Bild geprüft |  |
| 148 | R08 | 427–433 s | R08-315, R08-316, R08-317 | 0 | 2 / 3 | nur GPS (±1–3), prüfen |  |
| 151 | R08 | 508–511 s | R08-370 | 0 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 153 | R10 | 86–90 s | R10-081, R10-082 | 2 | 3 / 0 | unklar, prüfen | Rand/Bewuchs |
| 154 | R10 | 86–90 s | R10-081, R10-082, R10-083 | 2 | 5 / 0 | nur GPS (±1–3), prüfen | Rand/Bewuchs |
| 155 | R10 | 85–89 s | R10-082, R10-083, R10-084, R10-085 | 1, 2 | 3 / 1 | nur GPS (±1–3), prüfen | Rand/Bewuchs |
| 156 | R10 | 85–89 s | R10-083, R10-084, R10-085, R10-086 | 1, 2 | 3 / 2 | nur GPS (±1–3), prüfen | Rand/Bewuchs |
| 157 | R10 | 175–190 s | R10-181, R10-182, R10-183 | 0, 2 | 1 / 3 | nur GPS (±1–3), prüfen |  |
| 158 | R10 | 178–190 s | R10-185, R10-186 | 0 | 2 / 1 | nur GPS (±1–3), prüfen |  |
| 159 | R10 | 245–253 s | R10-240 | 1, 2 | 1 / 1 | Bild geprüft |  |
| 160 | R10 | 273–275 s | R10-255, R10-256, R10-257 | 0, 2 | 2 / 2 | nur GPS (±1–3), prüfen |  |
| 161 | R10 | 320–322 s | R10-297, R10-298, R10-299 | 0, 2 | 0 / 8 | nur GPS (±1–3), prüfen |  |
| 162 | R10 | 313–320 s | R10-299, R10-300, R10-301, R10-302 | 1, 2 | 5 / 3 | nur GPS (±1–3), prüfen |  |
| 165 | R10 | 324–336 s | R10-307, R10-309 | 0, 2 | 2 / 5 | nur GPS (±1–3), prüfen |  |
| 166 | R10 | 323–335 s | R10-307, R10-308, R10-310 | 0, 2 | 2 / 3 | nur GPS (±1–3), prüfen |  |
| 168 | R10 | 388–391 s | R10-377, R10-378 | 2 | 2 / 1 | nur GPS (±1–3), prüfen |  |
| 170 | R12 | 8–10 s | R12-003 | 0, 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 171 | R12 | 7–11 s | R12-004 | 1 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 173 | R12 | 0–6 s | R12-004, R12-005, R12-008 | 0, 2 | 2 / 2 | nur GPS (±1–3), prüfen |  |
| 172 | R12 | 1–6 s | R12-005, R12-008 | 0, 1 | 2 / 3 | nur GPS (±1–3), prüfen |  |
| 174 | R12 | 15–24 s | R12-017 | 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 175 | R12 | 15–23 s | R12-017, R12-018 | 2 | 1 / 1 | Bild geprüft |  |
| 176 | R12 | 144–156 s | R12-165 | 0 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 177 | R12 | 276–283 s | R12-340, R12-341 | 0 | 1 / 4 | nur GPS (±1–3), prüfen |  |
| 178 | R12 | 291–293 s | R12-350, R12-351 | 0, 2 | 9 / 1 | nur GPS (±1–3), prüfen |  |
| 179 | R12 | 289–290 s | R12-350, R12-351, R12-352 | 0, 1, 2 | 8 / 3 | nur GPS (±1–3), prüfen |  |
| 180 | R12 | 288–289 s | R12-352, R12-353 | 0, 1, 2 | 5 / 0 | nur GPS (±1–3), prüfen |  |
| 186 | R13 | 157–171 s | R13-141, R13-142 | 2 | 3 / 2 | nur GPS (±1–3), prüfen |  |
| 187 | R13 | 158–171 s | R13-141, R13-142 | 2 | 3 / 0 | nur GPS (±1–3), prüfen |  |
| 188 | R13 | 159–171 s | R13-141, R13-142 | 2 | 3 / 0 | nur GPS (±1–3), prüfen |  |
| 185 | R13 | 156–170 s | R13-141, R13-142 | 1, 2 | 2 / 1 | nur GPS (±1–3), prüfen | Rand/Bewuchs |
| 190 | R13 | 27–29 s | R13-341 | 0 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 192 | R14 | 71–76 s | R14-067 | 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 193 | R14 | 213–220 s | R14-279, R14-280 | 1, 2 | 4 / 1 | nur GPS (±1–3), prüfen | Rand/Bewuchs |
| 194 | R14 | 218–219 s | R14-280, R14-281 | 1, 2 | 3 / 2 | nur GPS (±1–3), prüfen | Rand/Bewuchs |
| 195 | R14 | 217–219 s | R14-281, R14-282 | 1, 2 | 4 / 5 | nur GPS (±1–3), prüfen |  |
| 200 | R15 | 216–218 s | R15-001 | 2 | 1 / 0 | nur GPS (±1–3), prüfen | Position geschätzt |
| 205 | R15 | 216–218 s | R15-001 | 1 | 1 / 0 | nur GPS (±1–3), prüfen | Position geschätzt |
| 207 | R15 | 214–218 s | R15-001 | 0 | 1 / 0 | nur GPS (±1–3), prüfen | Position geschätzt |
| 216 | R15 | 53–57 s | R15-306 | 1 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 217 | R15 | 35–40 s | R15-341 | 0 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 218 | R15 | 15–16 s | R15-367 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 223 | R16 | 0–6 s | R16-001 | 0, 1 | 2 / 1 | nur GPS (±1–3), prüfen |  |
| 224 | R16 | 8–19 s | R16-013 | 0 | 2 / 1 | nur GPS (±1–3), prüfen |  |
| 225 | R17 | 179–182 s | R17-091, R17-092, R17-093 | 0, 1, 2 | 3 / 3 | Bild geprüft |  |
| 226 | R17 | 149–151 s | R17-164 | 2 | 1 / 0 | Bild geprüft |  |
| 227 | R17 | 135–137 s | R17-183, R17-185 | 1, 2 | 3 / 2 | Bild geprüft |  |
| 228 | R17 | 122–124 s | R17-203, R17-204 | 0, 2 | 1 / 3 | nur GPS (±1–3), prüfen |  |
| 229 | R17 | 121–124 s | R17-205, R17-206 | 2 | 3 / 0 | nur GPS (±1–3), prüfen |  |
| 230 | R17 | 90–94 s | R17-258 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 231 | R18 | 251–252 s | R18-335, R18-336 | 0 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 232 | R18 | 259–262 s | R18-342, R18-343, R18-344 | 2 | 1 / 4 | Bild geprüft |  |
| 233 | R19 | 249–250 s | R19-043, R19-044 | 1 | 1 / 2 | nur GPS (±1–3), prüfen | Position geschätzt |
| 234 | R19 | 223–225 s | R19-095, R19-096 | 0 | 3 / 0 | nur GPS (±1–3), prüfen |  |
| 235 | R19 | 203–205 s | R19-129 | 2 | 1 / 0 | Bild geprüft |  |
| 236 | R19 | 201–202 s | R19-136 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 237 | R19 | 187–189 s | R19-162 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 238 | R19 | 178–180 s | R19-180 | 1 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 239 | R19 | 127–133 s | R19-236, R19-237 | 2 | 5 / 0 | nur GPS (±1–3), prüfen |  |
| 240 | R19 | 117–121 s | R19-251 | 2 | 1 / 0 | Bild geprüft |  |
| 241 | R19 | 109–112 s | R19-263 | 2 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 242 | R19 | 103–106 s | R19-272 | 1, 2 | 2 / 1 | Bild geprüft |  |
| 243 | R19 | 89–93 s | R19-290 | 2 | 1 / 0 | Bild geprüft |  |
| 244 | R19 | 75–80 s | R19-299 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 245 | R19 | 29–42 s | R19-333 | 0 | 2 / 0 | nur GPS (±1–3), prüfen |  |
| 248 | R20 | 80–82 s | R20-138 | 0 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 249 | R20 | 116–122 s | R20-192, R20-193 | 0 | 3 / 0 | nur GPS (±1–3), prüfen |  |
| 250 | R20 | 137–139 s | R20-233 | 1 | 1 / 0 | Bild geprüft |  |
| 252 | R21 | 146–149 s | R21-037 | 2 | 1 / 0 | Bild geprüft | Position geschätzt |
| 253 | R21 | 144–145 s | R21-043 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 254 | R21 | 123–125 s | R21-072 | 2 | 3 / 0 | Bild geprüft | Position geschätzt |
| 255 | R21 | 78–81 s | R21-132 | 1 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 256 | R21 | 78–81 s | R21-133 | 1 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 257 | R21 | 47–49 s | R21-181 | 0, 1 | 2 / 1 | Bild geprüft |  |
| 258 | R22 | 4–10 s | R22-009, R22-010 | 1 | 1 / 4 | nur GPS (±1–3), prüfen |  |
| 259 | R22 | 22–26 s | R22-030 | 1, 2 | 1 / 1 | nur GPS (±1–3), prüfen |  |
| 260 | R22 | 31–33 s | R22-038 | 1 | 1 / 0 | Bild geprüft |  |
| 261 | R22 | 46–48 s | R22-062 | 1 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 262 | R22 | 48–50 s | R22-067 | 2 | 4 / 0 | nur GPS (±1–3), prüfen |  |
| 263 | R22 | 52–54 s | R22-072, R22-073 | 1 | 4 / 0 | Bild geprüft |  |
| 264 | R22 | 59–61 s | R22-090 | 2 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 265 | R22 | 64–65 s | R22-099 | 0 | 1 / 0 | nur GPS (±1–3), prüfen |  |
| 266 | R24 | 22–24 s | R24-018 | 1 | 1 / 0 | Bild geprüft | Position geschätzt |

## Verworfen
- Spiegelungsflecken (wandern mit der Kamera), Helligkeitssprünge der Kamera, warme Längsstreifen in Modulen (Strangmuster), helle Randstreifen zum Gras, Klemmen/Teile an Gestelllücken, Grasflächen neben den Gestellen (vor allem R15/R16 am Reihenanfang).

## Offene Punkte
- **R06:** Gemessen ca. 328 m Länge = 21 Gestelle à 15,6 m; im Tool hat R06 nur 20 Gestelle. Zuordnung vorläufig vom Westende aus; Befunde im östlichsten Gestell haben keine ID.
- **R15:** Westende im Video nicht sicher erkannt; Positionen in R15 sind unsicherer (±3). Zellen ohne bestimmbare Position wurden der nächstliegenden Position zugeordnet.
- **R03:** Westende nicht erkannt; Zuordnung über Ostende und Lücken.
- **R09, R11, R23:** sehr wenige/keine Befunde; bitte stichprobenartig prüfen.
