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

## Genauigkeit
- Reihe und Gestell: sicher. Position innerhalb des Gestells: in der Regel ±1, bei schräger Kamera (Neigung -50° bis -70°) bis ±2. Ebene: aus der Lage im Gestellbild, meist sicher.
- Kachelzeile und -spalte sind grob geschätzt (±2).

## Kontrolle R01 und R02
Die bestätigten Befunde bleiben unverändert eingetragen. Die automatische Auswertung findet sie wieder (Abweichung höchstens 1 Position):
- R01: automatisch gefunden bei R01-028, R01-029, R01-040
- R02: automatisch gefunden bei R02-023, R02-024, R02-052, R02-074, R02-076, R02-093
- Abgleich: R01-029, R02-023, -024, -052, -076, -093 identisch; R01-027 ↔ 028, R01-039 ↔ 040, R02-073 ↔ 074 (je 1 Position Abweichung, bestätigter Wert bleibt).
- Nicht automatisch gefunden: R01-003 und der Streifen R01-006 (Anfangs- und Endbereich übersteuert), R02-066 (Zellpaar, zu länglich für den Formfilter), R02-067/070 (gelbe Zellen).
- Folgerung für R03–R24: Positionen dort sind ebenfalls auf etwa ±1 genau; Zellpaare, Streifen und schwache gelbe Zellen können fehlen.

## Befunde R03 bis R24
Jede helle Zelle ist einzeln markiert (weiß = Stufe 3, gelb = Stufe 1). Ein Befund (#) fasst die Zellen zusammen, die gemeinsam im Bild stehen; nebeneinanderliegende Zellen, die im Bild verschmelzen, wurden in Einzelzellen aufgeteilt.
Bilder: `bilder/gesamt/Rxx.jpg` (grüne Kreise = Stufe 3, gelbe = Stufe 1).

| # | Reihe | Zeit im Video | Position(en) | Ebene(n) | Zellen weiß / gelb | Hinweis |
|---|---|---|---|---|---|---|
| 13 | R03 | 20–22 s | R03-031 | 2 | 1 / 0 |  |
| 14 | R03 | 19–20 s | R03-032 | 2 | 1 / 0 |  |
| 15 | R03 | 17–19 s | R03-034 | 1 | 1 / 0 |  |
| 16 | R03 | 17–18 s | R03-034 | 2 | 1 / 0 |  |
| 17 | R03 | 20–30 s | R03-036 | 0 | 0 / 1 | Position geschätzt (nächstliegende) |
| 18 | R03 | 28–31 s | R03-042, R03-043 | 1, 2 | 3 / 0 | Rand/Bewuchs, als Hotspot bestätigt |
| 19 | R03 | 56–57 s | R03-062, R03-063 | 0, 1, 2 | 7 / 0 |  |
| 20 | R03 | 56–57 s | R03-062, R03-063 | 0, 1, 2 | 6 / 0 |  |
| 21 | R03 | 55–58 s | R03-062, R03-063 | 0, 1, 2 | 6 / 0 |  |
| 22 | R03 | 49–56 s | R03-062, R03-063 | 0, 1, 2 | 7 / 0 |  |
| 23 | R03 | 48–54 s | R03-063, R03-064 | 0, 1, 2 | 7 / 0 |  |
| 24 | R03 | 48–54 s | R03-063, R03-064 | 0, 1, 2 | 7 / 0 |  |
| 25 | R03 | 48–54 s | R03-063, R03-064 | 0, 1, 2 | 7 / 0 |  |
| 27 | R03 | 83–88 s | R03-095 | 2 | 2 / 0 |  |
| 28 | R03 | 81–88 s | R03-095 | 2 | 2 / 1 |  |
| 29 | R03 | 90–91 s | R03-101 | 2 | 2 / 0 |  |
| 30 | R03 | 94–96 s | R03-107 | 2 | 2 / 0 |  |
| 31 | R03 | 92–93 s | R03-108 | 2 | 2 / 0 |  |
| 33 | R03 | 126–128 s | R03-124 | 2 | 1 / 0 |  |
| 34 | R03 | 121–125 s | R03-125 | 2 | 1 / 0 |  |
| 35 | R03 | 165–167 s | R03-143 | 2 | 1 / 0 |  |
| 36 | R03 | 166–168 s | R03-146 | 2 | 1 / 2 |  |
| 37 | R03 | 165–169 s | R03-146 | 2 | 1 / 0 |  |
| 38 | R03 | 175–178 s | R03-156 | 0 | 2 / 0 |  |
| 39 | R03 | 175–178 s | R03-156 | 2 | 1 / 0 |  |
| 40 | R03 | 175–179 s | R03-157 | 1 | 2 / 0 |  |
| 41 | R04 | 96–97 s | R04-109 | 0 | 2 / 0 |  |
| 42 | R04 | 27–31 s | R04-182 | 0 | 1 / 0 |  |
| 43 | R04 | 29–31 s | R04-182 | 2 | 1 / 0 |  |
| 44 | R04 | 9–14 s | R04-201, R04-202 | 0, 1, 2 | 3 / 2 |  |
| 45 | R04 | 11–13 s | R04-201, R04-202 | 1, 2 | 4 / 0 |  |
| 47 | R04 | 6–9 s | R04-207 | 1 | 1 / 0 |  |
| 48 | R05 | 29–40 s | R05-014 | 2 | 1 / 0 |  |
| 49 | R06 | 5–25 s | R06-011, R06-013 | 0, 2 | 1 / 1 |  |
| 50 | R06 | 10–24 s | R06-012 | 2 | 1 / 0 |  |
| 51 | R06 | 15–19 s | R06-013 | 2 | 1 / 0 |  |
| 52 | R06 | 5–39 s | R06-014 | 2 | 2 / 0 |  |
| 53 | R06 | 35–42 s | R06-017 | 2 | 1 / 0 |  |
| 57 | R06 | 33–62 s | R06-020, R06-021, R06-023, R06-025 | 0, 1, 2 | 3 / 4 |  |
| 59 | R06 | 58–61 s | R06-030, R06-032, R06-034, R06-035 | 1 | 2 / 6 |  |
| 60 | R06 | 203–214 s | R06-097 | 0, 2 | 3 / 1 |  |
| 63 | R06 | 349–355 s | R06-199 | 2 | 1 / 1 |  |
| 64 | R06 | 350–355 s | R06-200 | 2 | 1 / 0 |  |
| 65 | R06 | 350–355 s | R06-200 | 1 | 1 / 0 |  |
| 66 | R06 | 346–357 s | R06-202 | 1 | 1 / 0 |  |
| 67 | R06 | 365–367 s | R06-217 | 1 | 1 / 0 |  |
| 68 | R06 | 383–387 s | R06-241 | 2 | 1 / 0 |  |
| 69 | R06 | 389–394 s | R06-249, R06-250 | 2 | 5 / 0 | Rand/Bewuchs, als Hotspot bestätigt |
| 70 | R06 | 393–394 s | R06-250 | 2 | 1 / 0 |  |
| 71 | R06 | 404–408 s | R06-269 | 1 | 1 / 0 |  |
| 72 | R06 | 406–409 s | R06-270 | 1 | 1 / 0 | Position geschätzt (nächstliegende) |
| 73 | R06 | 415–418 s | R06-282 | 2 | 1 / 0 |  |
| 75 | R06 | 430–440 s | R06-303 | 2 | 1 / 0 |  |
| 76 | R06 | 434–443 s | R06-310 | 0 | 2 / 0 |  |
| 78 | R06 | 475–477 s | R06-336, R06-337 | 0, 1 | 2 / 2 |  |
| 77 | R06 | 472–478 s | R06-337, R06-338 | 1, 2 | 3 / 0 |  |
| 79 | R06 | 469–472 s | R06-338 | 1, 2 | 4 / 0 |  |
| 80 | R06 | 473–479 s | R06-338 | 0 | 0 / 1 |  |
| 81 | R06 | 480–482 s | R06-341 | 2 | 1 / 0 |  |
| 82 | R06 | 486–489 s | R06-350 | 0 | 1 / 0 |  |
| 83 | R06 | 490–493 s | R06-353 | 1 | 1 / 0 |  |
| 84 | R06 | 488–490 s | R06-354 | 1 | 1 / 0 |  |
| 85 | R06 | 498–501 s | R06-360 | 2 | 1 / 0 | Position geschätzt (nächstliegende) |
| 86 | R07 | 159–162 s | R07-226 | 2 | 1 / 0 |  |
| 88 | R07 | 135–138 s | R07-256 | 2 | 1 / 0 |  |
| 89 | R07 | 121–126 s | R07-270 | 2 | 1 / 0 | Position geschätzt (nächstliegende) |
| 90 | R07 | 118–121 s | R07-272 | 2 | 1 / 0 |  |
| 91 | R07 | 118–123 s | R07-273 | 1 | 1 / 0 |  |
| 92 | R07 | 120–123 s | R07-274 | 1 | 1 / 0 |  |
| 93 | R07 | 103–110 s | R07-287 | 2 | 0 / 1 |  |
| 94 | R07 | 101–106 s | R07-288, R07-289 | 2 | 3 / 0 |  |
| 95 | R07 | 102–104 s | R07-289, R07-290 | 2 | 2 / 0 |  |
| 96 | R07 | 101–105 s | R07-290, R07-291 | 2 | 2 / 0 |  |
| 98 | R07 | 103–107 s | R07-291, R07-292 | 2 | 2 / 0 |  |
| 97 | R07 | 100–107 s | R07-292 | 2 | 2 / 0 |  |
| 99 | R07 | 97–105 s | R07-293 | 2 | 1 / 0 |  |
| 100 | R07 | 99–103 s | R07-294, R07-295 | 2 | 0 / 2 |  |
| 101 | R07 | 96–99 s | R07-298, R07-299 | 1, 2 | 3 / 2 |  |
| 102 | R07 | 97–98 s | R07-298, R07-299 | 1, 2 | 4 / 2 |  |
| 103 | R07 | 71–73 s | R07-321 | 2 | 1 / 0 |  |
| 104 | R07 | 74–75 s | R07-322 | 2 | 1 / 0 |  |
| 105 | R07 | 68–77 s | R07-322 | 2 | 1 / 0 |  |
| 106 | R07 | 68–70 s | R07-323, R07-325 | 1, 2 | 3 / 2 |  |
| 107 | R07 | 69–71 s | R07-323 | 1, 2 | 3 / 1 |  |
| 108 | R07 | 71–73 s | R07-324, R07-325 | 1, 2 | 2 / 1 |  |
| 109 | R07 | 71–73 s | R07-324 | 1, 2 | 3 / 1 |  |
| 110 | R07 | 73–75 s | R07-325 | 1, 2 | 3 / 1 |  |
| 111 | R07 | 73–75 s | R07-325 | 1, 2 | 3 / 1 |  |
| 112 | R07 | 62–72 s | R07-327, R07-328 | 2 | 2 / 0 |  |
| 113 | R07 | 58–60 s | R07-331 | 2 | 1 / 0 |  |
| 114 | R07 | 59–60 s | R07-331, R07-332 | 1, 2 | 2 / 0 |  |
| 115 | R07 | 61–64 s | R07-331, R07-332 | 0, 2 | 2 / 0 |  |
| 116 | R07 | 61–63 s | R07-332, R07-333 | 1, 2 | 2 / 0 |  |
| 117 | R07 | 62–66 s | R07-333 | 0, 2 | 2 / 0 |  |
| 118 | R07 | 64–65 s | R07-333, R07-334 | 1, 2 | 2 / 0 |  |
| 119 | R07 | 53–55 s | R07-336 | 1, 2 | 1 / 1 |  |
| 120 | R07 | 57–59 s | R07-336 | 2 | 2 / 0 |  |
| 121 | R07 | 55–59 s | R07-337 | 1, 2 | 1 / 1 |  |
| 122 | R07 | 57–58 s | R07-337, R07-338 | 1, 2 | 1 / 2 |  |
| 123 | R07 | 41–46 s | R07-347 | 1 | 1 / 0 |  |
| 124 | R07 | 39–46 s | R07-349 | 2 | 1 / 0 |  |
| 125 | R07 | 43–45 s | R07-350 | 2 | 2 / 0 |  |
| 126 | R07 | 0–5 s | R07-378 | 0, 1, 2 | 3 / 2 |  |
| 127 | R07 | 0–6 s | R07-378 | 0, 1, 2 | 3 / 0 |  |
| 128 | R07 | 1–5 s | R07-378 | 0, 1 | 4 / 0 | Position geschätzt (nächstliegende) |
| 129 | R08 | 262–266 s | R08-205, R08-206 | 1, 2 | 3 / 0 |  |
| 130 | R08 | 279–303 s | R08-216, R08-217 | 1, 2 | 4 / 2 |  |
| 131 | R08 | 278–301 s | R08-218 | 1, 2 | 4 / 0 |  |
| 132 | R08 | 293–301 s | R08-218, R08-221 | 0, 1, 2 | 5 / 2 |  |
| 133 | R08 | 280–298 s | R08-220, R08-221 | 0, 1, 2 | 3 / 1 |  |
| 134 | R08 | 280–298 s | R08-221, R08-222 | 1, 2 | 2 / 5 |  |
| 135 | R08 | 311–317 s | R08-229 | 2 | 2 / 0 |  |
| 136 | R08 | 318–322 s | R08-238 | 0 | 1 / 0 |  |
| 137 | R08 | 328–337 s | R08-245, R08-246 | 1, 2 | 3 / 1 | Rand/Bewuchs, als Hotspot bestätigt |
| 139 | R08 | 327–342 s | R08-246, R08-247 | 1, 2 | 3 / 2 | Rand/Bewuchs, als Hotspot bestätigt |
| 140 | R08 | 326–341 s | R08-246, R08-247 | 1, 2 | 3 / 3 | Rand/Bewuchs, als Hotspot bestätigt |
| 138 | R08 | 327–342 s | R08-247 | 1, 2 | 2 / 0 |  |
| 141 | R08 | 326–341 s | R08-248, R08-249 | 1, 2 | 3 / 0 |  |
| 142 | R08 | 345–348 s | R08-255, R08-256 | 2 | 3 / 0 |  |
| 143 | R08 | 345–348 s | R08-255, R08-256, R08-257 | 1, 2 | 5 / 0 |  |
| 144 | R08 | 343–346 s | R08-256, R08-257, R08-258 | 0, 2 | 3 / 1 |  |
| 145 | R08 | 343–345 s | R08-258, R08-259 | 2 | 2 / 0 |  |
| 146 | R08 | 346–353 s | R08-261, R08-262 | 2 | 2 / 1 |  |
| 147 | R08 | 410–412 s | R08-308, R08-309, R08-310 | 0, 1 | 1 / 2 |  |
| 148 | R08 | 427–433 s | R08-315, R08-316, R08-317 | 0 | 2 / 3 |  |
| 151 | R08 | 508–511 s | R08-370 | 0 | 1 / 0 |  |
| 153 | R10 | 86–90 s | R10-081, R10-082 | 2 | 3 / 0 | Rand/Bewuchs, als Hotspot bestätigt |
| 154 | R10 | 86–90 s | R10-081, R10-082, R10-083 | 2 | 5 / 0 | Rand/Bewuchs, als Hotspot bestätigt |
| 155 | R10 | 85–89 s | R10-082, R10-083, R10-084, R10-085 | 1, 2 | 3 / 1 | Rand/Bewuchs, als Hotspot bestätigt |
| 156 | R10 | 85–89 s | R10-083, R10-084, R10-085, R10-086 | 1, 2 | 3 / 2 | Rand/Bewuchs, als Hotspot bestätigt |
| 157 | R10 | 175–190 s | R10-181, R10-182, R10-183 | 0, 2 | 1 / 3 |  |
| 158 | R10 | 178–190 s | R10-185, R10-186 | 0 | 2 / 1 |  |
| 159 | R10 | 245–253 s | R10-241 | 1, 2 | 1 / 1 |  |
| 160 | R10 | 273–275 s | R10-255, R10-256, R10-257 | 0, 2 | 2 / 2 |  |
| 161 | R10 | 320–322 s | R10-297, R10-298, R10-299 | 0, 2 | 0 / 8 |  |
| 162 | R10 | 313–320 s | R10-299, R10-300, R10-301, R10-302 | 1, 2 | 5 / 3 |  |
| 165 | R10 | 324–336 s | R10-307, R10-309 | 0, 2 | 2 / 5 |  |
| 166 | R10 | 323–335 s | R10-307, R10-308, R10-310 | 0, 2 | 2 / 3 |  |
| 168 | R10 | 388–391 s | R10-377, R10-378 | 2 | 2 / 1 |  |
| 170 | R12 | 8–10 s | R12-003 | 0, 2 | 2 / 0 |  |
| 171 | R12 | 7–11 s | R12-004 | 1 | 2 / 0 |  |
| 173 | R12 | 0–6 s | R12-004, R12-005, R12-008 | 0, 2 | 2 / 2 |  |
| 172 | R12 | 1–6 s | R12-005, R12-008 | 0, 1 | 2 / 3 |  |
| 174 | R12 | 15–24 s | R12-017 | 2 | 2 / 0 |  |
| 175 | R12 | 15–23 s | R12-017, R12-018 | 2 | 1 / 1 |  |
| 176 | R12 | 144–156 s | R12-165 | 0 | 1 / 0 |  |
| 177 | R12 | 276–283 s | R12-340, R12-341 | 0 | 1 / 4 |  |
| 178 | R12 | 291–293 s | R12-350, R12-351 | 0, 2 | 9 / 1 |  |
| 179 | R12 | 289–290 s | R12-350, R12-351, R12-352 | 0, 1, 2 | 8 / 3 |  |
| 180 | R12 | 288–289 s | R12-352, R12-353 | 0, 1, 2 | 5 / 0 |  |
| 186 | R13 | 157–171 s | R13-141, R13-142 | 2 | 3 / 2 |  |
| 187 | R13 | 158–171 s | R13-141, R13-142 | 2 | 3 / 0 |  |
| 188 | R13 | 159–171 s | R13-141, R13-142 | 2 | 3 / 0 |  |
| 185 | R13 | 156–170 s | R13-141, R13-142 | 1, 2 | 2 / 1 | Rand/Bewuchs, als Hotspot bestätigt |
| 190 | R13 | 27–29 s | R13-341 | 0 | 1 / 0 |  |
| 192 | R14 | 71–76 s | R14-067 | 2 | 2 / 0 |  |
| 193 | R14 | 213–220 s | R14-279, R14-280 | 1, 2 | 4 / 1 | Rand/Bewuchs, als Hotspot bestätigt |
| 194 | R14 | 218–219 s | R14-280, R14-281 | 1, 2 | 3 / 2 | Rand/Bewuchs, als Hotspot bestätigt |
| 195 | R14 | 217–219 s | R14-281, R14-282 | 1, 2 | 4 / 5 |  |
| 200 | R15 | 216–218 s | R15-001 | 2 | 1 / 0 | Position geschätzt (nächstliegende) |
| 205 | R15 | 216–218 s | R15-001 | 1 | 1 / 0 | Position geschätzt (nächstliegende) |
| 207 | R15 | 214–218 s | R15-001 | 0 | 1 / 0 | Position geschätzt (nächstliegende) |
| 216 | R15 | 53–57 s | R15-306 | 1 | 1 / 0 |  |
| 217 | R15 | 35–40 s | R15-341 | 0 | 1 / 0 |  |
| 218 | R15 | 15–16 s | R15-367 | 2 | 1 / 0 |  |
| 223 | R16 | 0–6 s | R16-001 | 0, 1 | 2 / 1 |  |
| 224 | R16 | 8–19 s | R16-013 | 0 | 2 / 1 |  |
| 225 | R17 | 179–182 s | R17-093, R17-094, R17-095 | 0, 1, 2 | 3 / 3 |  |
| 226 | R17 | 149–151 s | R17-164 | 2 | 1 / 0 |  |
| 227 | R17 | 135–137 s | R17-183, R17-185 | 1, 2 | 3 / 2 |  |
| 228 | R17 | 122–124 s | R17-203, R17-204 | 0, 2 | 1 / 3 |  |
| 229 | R17 | 121–124 s | R17-205, R17-206 | 2 | 3 / 0 |  |
| 230 | R17 | 90–94 s | R17-258 | 2 | 1 / 0 |  |
| 231 | R18 | 251–252 s | R18-335, R18-336 | 0 | 2 / 0 |  |
| 232 | R18 | 259–262 s | R18-342, R18-343, R18-344 | 2 | 1 / 4 |  |
| 233 | R19 | 249–250 s | R19-043, R19-044 | 1 | 1 / 2 | Position geschätzt (nächstliegende) |
| 234 | R19 | 223–225 s | R19-095, R19-096 | 0 | 3 / 0 |  |
| 235 | R19 | 203–205 s | R19-130 | 2 | 1 / 0 |  |
| 236 | R19 | 201–202 s | R19-136 | 2 | 1 / 0 |  |
| 237 | R19 | 187–189 s | R19-162 | 2 | 1 / 0 |  |
| 238 | R19 | 178–180 s | R19-180 | 1 | 1 / 0 |  |
| 239 | R19 | 127–133 s | R19-236, R19-237 | 2 | 5 / 0 |  |
| 240 | R19 | 117–121 s | R19-250 | 2 | 1 / 0 |  |
| 241 | R19 | 109–112 s | R19-263 | 2 | 2 / 0 |  |
| 242 | R19 | 103–106 s | R19-271 | 1, 2 | 2 / 1 |  |
| 243 | R19 | 89–93 s | R19-289 | 2 | 1 / 0 |  |
| 244 | R19 | 75–80 s | R19-299 | 2 | 1 / 0 |  |
| 245 | R19 | 29–42 s | R19-333 | 0 | 2 / 0 |  |
| 248 | R20 | 80–82 s | R20-138 | 0 | 1 / 0 |  |
| 249 | R20 | 116–122 s | R20-192, R20-193 | 0 | 3 / 0 |  |
| 250 | R20 | 137–139 s | R20-235 | 1 | 1 / 0 |  |
| 252 | R21 | 146–149 s | R21-036 | 2 | 1 / 0 | Position geschätzt (nächstliegende) |
| 253 | R21 | 144–145 s | R21-043 | 2 | 1 / 0 |  |
| 254 | R21 | 123–125 s | R21-072 | 2 | 3 / 0 | Position geschätzt (nächstliegende) |
| 255 | R21 | 78–81 s | R21-132 | 1 | 1 / 0 |  |
| 256 | R21 | 78–81 s | R21-133 | 1 | 1 / 0 |  |
| 257 | R21 | 47–49 s | R21-181 | 0, 1 | 2 / 1 |  |
| 258 | R22 | 4–10 s | R22-009, R22-010 | 1 | 1 / 4 |  |
| 259 | R22 | 22–26 s | R22-030 | 1, 2 | 1 / 1 |  |
| 260 | R22 | 31–33 s | R22-039 | 1 | 1 / 0 |  |
| 261 | R22 | 46–48 s | R22-062 | 1 | 1 / 0 |  |
| 262 | R22 | 48–50 s | R22-067 | 2 | 4 / 0 |  |
| 263 | R22 | 52–54 s | R22-074, R22-075 | 1 | 4 / 0 |  |
| 264 | R22 | 59–61 s | R22-090 | 2 | 1 / 0 |  |
| 265 | R22 | 64–65 s | R22-099 | 0 | 1 / 0 |  |
| 266 | R24 | 22–24 s | R24-019 | 1 | 1 / 0 | Position geschätzt (nächstliegende) |

## Verworfen
- Spiegelungsflecken (wandern mit der Kamera), Helligkeitssprünge der Kamera, warme Längsstreifen in Modulen (Strangmuster), helle Randstreifen zum Gras, Klemmen/Teile an Gestelllücken, Grasflächen neben den Gestellen (vor allem R15/R16 am Reihenanfang).

## Offene Punkte
- **R06:** Gemessen ca. 328 m Länge = 21 Gestelle à 15,6 m; im Tool hat R06 nur 20 Gestelle. Zuordnung vorläufig vom Westende aus; Befunde im östlichsten Gestell haben keine ID.
- **R15:** Westende im Video nicht sicher erkannt; Positionen in R15 sind unsicherer (±3). Zellen ohne bestimmbare Position wurden der nächstliegenden Position zugeordnet.
- **R03:** Westende nicht erkannt; Zuordnung über Ostende und Lücken.
- **R09, R11, R23:** sehr wenige/keine Befunde; bitte stichprobenartig prüfen.
