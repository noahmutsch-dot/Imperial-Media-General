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
Bilder: `bilder/gesamt/Rxx.jpg` (Nummer `#` wie in der Tabelle; grün = eingetragen, gelb = unsicher/ohne Position).

| # | Reihe | Zeit im Video | Position | Ebene | Zeile / Spalte | Stufe |
|---|---|---|---|---|---|---|
| 13 | R03 | 20–22 s | R03-032 | 2 | 5 / 1 | 3 |
| 14 | R03 | 19–20 s | R03-033 | 2 | 5 / 1 | 3 |
| 15 | R03 | 17–19 s | R03-034 | 1 | 10 / 1 | 3 |
| 16 | R03 | 17–18 s | R03-035 | 2 | 4 / 0 | 3 |
| 19 | R03 | 56–57 s | R03-062 | 0 | 4 / 2 | 3 |
| 20 | R03 | 56–57 s | R03-062 | 2 | 4 / 2 | 3 |
| 21 | R03 | 55–58 s | R03-062 | 1 | 10 / 3 | 3 |
| 22 | R03 | 49–56 s | R03-063 | 1 | 10 / 2 | 3 |
| 23 | R03 | 48–54 s | R03-063 | 2 | 4 / 3 | 3 |
| 24 | R03 | 48–54 s | R03-063 | 0 | 4 / 3 | 3 |
| 25 | R03 | 48–54 s | R03-064 | 1 | 10 / 0 | 3 |
| 27 | R03 | 83–88 s | R03-095 | 2 | 6 / 2 | 3 |
| 28 | R03 | 81–88 s | R03-096 | 2 | 9 / 2 | 3 |
| 29 | R03 | 90–91 s | R03-101 | 2 | 3 / 3 | 3 |
| 30 | R03 | 94–96 s | R03-108 | 2 | 3 / 2 | 3 |
| 31 | R03 | 92–93 s | R03-108 | 2 | 4 / 4 | 3 |
| 33 | R03 | 126–128 s | R03-124 | 2 | 8 / 4 | 3 |
| 34 | R03 | 121–125 s | R03-125 | 2 | 8 / 1 | 3 |
| 35 | R03 | 165–167 s | R03-143 | 2 | 10 / 2 | 3 |
| 36 | R03 | 166–168 s | R03-146 | 2 | 6 / 0 | 3 |
| 37 | R03 | 165–169 s | R03-146 | 2 | 2 / 1 | 3 |
| 38 | R03 | 175–178 s | R03-156 | 0 | 6 / 1 | 3 |
| 39 | R03 | 175–178 s | R03-156 | 2 | 4 / 4 | 3 |
| 40 | R03 | 175–179 s | R03-157 | 1 | 10 / 1 | 3 |
| 41 | R04 | 96–97 s | R04-109 | 0 | 11 / 2 | 3 |
| 42 | R04 | 27–31 s | R04-182 | 0 | 10 / 0 | 3 |
| 43 | R04 | 29–31 s | R04-182 | 2 | 2 / 2 | 3 |
| 44 | R04 | 9–14 s | R04-201 | 0 | 8 / 4 | 3 |
| 45 | R04 | 11–13 s | R04-202 | 2 | 7 / 1 | 3 |
| 47 | R04 | 6–9 s | R04-207 | 1 | 8 / 3 | 3 |
| 48 | R05 | 29–40 s | R05-014 | 2 | 10 / 1 | 3 |
| 49 | R06 | 5–25 s | R06-011 | 2 | 9 / 1 | 1 |
| 50 | R06 | 10–24 s | R06-012 | 2 | 9 / 0 | 3 |
| 51 | R06 | 15–19 s | R06-013 | 2 | 9 / 3 | 3 |
| 52 | R06 | 5–39 s | R06-014 | 2 | 9 / 4 | 3 |
| 53 | R06 | 35–42 s | R06-017 | 2 | 10 / 2 | 3 |
| 57 | R06 | 33–62 s | R06-023 | 0 | 2 / 1 | 3 |
| 59 | R06 | 58–61 s | R06-032 | 1 | 8 / 2 | 3 |
| 60 | R06 | 203–214 s | R06-097 | 2 | 8 / 3 | 3 |
| 63 | R06 | 349–355 s | R06-199 | 2 | 0 / 4 | 3 |
| 64 | R06 | 350–355 s | R06-200 | 2 | 8 / 1 | 3 |
| 65 | R06 | 350–355 s | R06-200 | 1 | 7 / 2 | 3 |
| 66 | R06 | 346–357 s | R06-202 | 1 | 8 / 0 | 3 |
| 67 | R06 | 365–367 s | R06-217 | 1 | 10 / 2 | 3 |
| 68 | R06 | 383–387 s | R06-242 | 2 | 9 / 0 | 3 |
| 70 | R06 | 393–394 s | R06-251 | 2 | 4 / 1 | 3 |
| 71 | R06 | 404–408 s | R06-270 | 1 | 7 / 0 | 3 |
| 73 | R06 | 415–418 s | R06-282 | 2 | 10 / 4 | 3 |
| 75 | R06 | 430–440 s | R06-303 | 2 | 10 / 1 | 3 |
| 76 | R06 | 434–443 s | R06-310 | 0 | 10 / 2 | 3 |
| 77 | R06 | 472–478 s | R06-337 | 2 | 2 / 5 | 3 |
| 78 | R06 | 475–477 s | R06-338 | 1 | 0 / 0 | 3 |
| 79 | R06 | 469–472 s | R06-338 | 2 | 1 / 2 | 3 |
| 80 | R06 | 473–479 s | R06-338 | 1 | 0 / 3 | 3 |
| 81 | R06 | 480–482 s | R06-341 | 2 | 10 / 5 | 3 |
| 82 | R06 | 486–489 s | R06-350 | 0 | 7 / 0 | 3 |
| 83 | R06 | 490–493 s | R06-353 | 1 | 3 / 4 | 3 |
| 84 | R06 | 488–490 s | R06-354 | 1 | 3 / 1 | 3 |
| 86 | R07 | 159–162 s | R07-226 | 2 | 8 / 3 | 3 |
| 88 | R07 | 135–138 s | R07-256 | 2 | 11 / 2 | 3 |
| 90 | R07 | 118–121 s | R07-272 | 2 | 7 / 4 | 3 |
| 91 | R07 | 118–123 s | R07-273 | 1 | 3 / 1 | 3 |
| 92 | R07 | 120–123 s | R07-274 | 1 | 2 / 0 | 3 |
| 93 | R07 | 103–110 s | R07-287 | 2 | 8 / 3 | 3 |
| 94 | R07 | 101–106 s | R07-288 | 2 | 10 / 3 | 3 |
| 95 | R07 | 102–104 s | R07-289 | 2 | 10 / 5 | 3 |
| 96 | R07 | 101–105 s | R07-290 | 2 | 10 / 4 | 3 |
| 97 | R07 | 100–107 s | R07-291 | 2 | 10 / 3 | 3 |
| 98 | R07 | 103–107 s | R07-292 | 2 | 9 / 3 | 3 |
| 99 | R07 | 97–105 s | R07-293 | 2 | 8 / 4 | 3 |
| 100 | R07 | 99–103 s | R07-295 | 2 | 11 / 3 | 1 |
| 101 | R07 | 96–99 s | R07-299 | 1 | 8 / 1 | 3 |
| 102 | R07 | 97–98 s | R07-299 | 2 | 7 / 4 | 3 |
| 103 | R07 | 71–73 s | R07-321 | 2 | 5 / 1 | 3 |
| 104 | R07 | 74–75 s | R07-321 | 2 | 5 / 5 | 3 |
| 105 | R07 | 68–77 s | R07-322 | 2 | 5 / 2 | 3 |
| 106 | R07 | 68–70 s | R07-323 | 2 | 8 / 4 | 3 |
| 107 | R07 | 69–71 s | R07-323 | 1 | 10 / 4 | 3 |
| 108 | R07 | 71–73 s | R07-324 | 2 | 7 / 3 | 3 |
| 109 | R07 | 71–73 s | R07-324 | 1 | 7 / 4 | 3 |
| 110 | R07 | 73–75 s | R07-325 | 2 | 8 / 0 | 3 |
| 111 | R07 | 73–75 s | R07-325 | 1 | 8 / 0 | 3 |
| 112 | R07 | 62–72 s | R07-327 | 2 | 10 / 3 | 3 |
| 113 | R07 | 58–60 s | R07-331 | 2 | 3 / 1 | 3 |
| 114 | R07 | 59–60 s | R07-332 | 1 | 5 / 1 | 3 |
| 115 | R07 | 61–64 s | R07-332 | 2 | 2 / 2 | 3 |
| 116 | R07 | 61–63 s | R07-333 | 1 | 5 / 0 | 3 |
| 117 | R07 | 62–66 s | R07-333 | 2 | 2 / 0 | 3 |
| 118 | R07 | 64–65 s | R07-333 | 1 | 5 / 5 | 3 |
| 119 | R07 | 53–55 s | R07-336 | 1 | 10 / 3 | 3 |
| 120 | R07 | 57–59 s | R07-336 | 2 | 10 / 5 | 3 |
| 121 | R07 | 55–59 s | R07-337 | 1 | 10 / 2 | 3 |
| 122 | R07 | 57–58 s | R07-338 | 1 | 9 / 0 | 3 |
| 123 | R07 | 41–46 s | R07-347 | 1 | 2 / 5 | 3 |
| 124 | R07 | 39–46 s | R07-349 | 2 | 6 / 5 | 3 |
| 125 | R07 | 43–45 s | R07-350 | 2 | 5 / 3 | 3 |
| 126 | R07 | 0–5 s | R07-378 | 2 | 2 / 0 | 3 |
| 127 | R07 | 0–6 s | R07-378 | 2 | 8 / 5 | 3 |
| 129 | R08 | 262–266 s | R08-205 | 1 | 10 / 3 | 3 |
| 130 | R08 | 279–303 s | R08-217 | 1 | 4 / 4 | 3 |
| 131 | R08 | 278–301 s | R08-218 | 2 | 1 / 4 | 3 |
| 132 | R08 | 293–301 s | R08-218 | 1 | 4 / 4 | 3 |
| 133 | R08 | 280–298 s | R08-220 | 2 | 1 / 3 | 3 |
| 134 | R08 | 280–298 s | R08-220 | 1 | 4 / 4 | 3 |
| 135 | R08 | 311–317 s | R08-228 | 2 | 10 / 5 | 3 |
| 136 | R08 | 318–322 s | R08-238 | 0 | 1 / 3 | 3 |
| 138 | R08 | 327–342 s | R08-247 | 1 | 10 / 1 | 3 |
| 141 | R08 | 326–341 s | R08-249 | 2 | 5 / 0 | 3 |
| 142 | R08 | 345–348 s | R08-255 | 2 | 10 / 1 | 3 |
| 143 | R08 | 345–348 s | R08-255 | 2 | 9 / 5 | 3 |
| 144 | R08 | 343–346 s | R08-258 | 2 | 9 / 2 | 3 |
| 145 | R08 | 343–345 s | R08-259 | 2 | 10 / 0 | 3 |
| 146 | R08 | 346–353 s | R08-261 | 2 | 9 / 1 | 3 |
| 147 | R08 | 410–412 s | R08-308 | 1 | 3 / 5 | 3 |
| 148 | R08 | 427–433 s | R08-317 | 0 | 10 / 0 | 3 |
| 151 | R08 | 508–511 s | R08-370 | 0 | 4 / 5 | 3 |
| 157 | R10 | 175–190 s | R10-181 | 2 | 10 / 2 | 3 |
| 158 | R10 | 178–190 s | R10-186 | 0 | 1 / 3 | 3 |
| 159 | R10 | 245–253 s | R10-240 | 2 | 9 / 5 | 3 |
| 160 | R10 | 273–275 s | R10-256 | 2 | 10 / 3 | 3 |
| 161 | R10 | 320–322 s | R10-299 | 2 | 9 / 1 | 3 |
| 162 | R10 | 313–320 s | R10-301 | 1 | 0 / 3 | 3 |
| 165 | R10 | 324–336 s | R10-307 | 2 | 3 / 1 | 3 |
| 166 | R10 | 323–335 s | R10-308 | 2 | 4 / 0 | 3 |
| 168 | R10 | 388–391 s | R10-378 | 2 | 10 / 3 | 3 |
| 170 | R12 | 8–10 s | R12-003 | 2 | 7 / 3 | 3 |
| 171 | R12 | 7–11 s | R12-003 | 1 | 7 / 5 | 3 |
| 172 | R12 | 1–6 s | R12-005 | 1 | 6 / 3 | 3 |
| 173 | R12 | 0–6 s | R12-005 | 2 | 9 / 4 | 3 |
| 174 | R12 | 15–24 s | R12-017 | 2 | 7 / 0 | 3 |
| 175 | R12 | 15–23 s | R12-018 | 2 | 8 / 4 | 3 |
| 176 | R12 | 144–156 s | R12-165 | 0 | 0 / 4 | 3 |
| 177 | R12 | 276–283 s | R12-340 | 0 | 5 / 4 | 3 |
| 178 | R12 | 291–293 s | R12-350 | 2 | 3 / 4 | 3 |
| 179 | R12 | 289–290 s | R12-351 | 0 | 4 / 4 | 3 |
| 180 | R12 | 288–289 s | R12-352 | 0 | 4 / 3 | 3 |
| 186 | R13 | 157–171 s | R13-142 | 2 | 10 / 0 | 3 |
| 187 | R13 | 158–171 s | R13-142 | 2 | 4 / 3 | 3 |
| 188 | R13 | 159–171 s | R13-142 | 2 | 9 / 4 | 3 |
| 190 | R13 | 27–29 s | R13-341 | 0 | 5 / 5 | 3 |
| 192 | R14 | 71–76 s | R14-067 | 2 | 9 / 2 | 3 |
| 195 | R14 | 217–219 s | R14-282 | 2 | 7 / 1 | 3 |
| 216 | R15 | 53–57 s | R15-306 | 1 | 8 / 4 | 3 |
| 217 | R15 | 35–40 s | R15-340 | 0 | 8 / 2 | 3 |
| 218 | R15 | 15–16 s | R15-367 | 2 | 7 / 0 | 3 |
| 223 | R16 | 0–6 s | R16-001 | 1 | 9 / 2 | 3 |
| 224 | R16 | 8–19 s | R16-013 | 0 | 0 / 1 | 3 |
| 225 | R17 | 179–182 s | R17-094 | 2 | 10 / 0 | 3 |
| 226 | R17 | 149–151 s | R17-163 | 2 | 6 / 5 | 3 |
| 227 | R17 | 135–137 s | R17-183 | 1 | 7 / 4 | 3 |
| 228 | R17 | 122–124 s | R17-203 | 2 | 10 / 4 | 3 |
| 229 | R17 | 121–124 s | R17-205 | 2 | 10 / 1 | 3 |
| 230 | R17 | 90–94 s | R17-258 | 2 | 10 / 3 | 3 |
| 231 | R18 | 251–252 s | R18-335 | 0 | 7 / 2 | 3 |
| 232 | R18 | 259–262 s | R18-343 | 2 | 8 / 3 | 3 |
| 234 | R19 | 223–225 s | R19-096 | 0 | 2 / 2 | 3 |
| 235 | R19 | 203–205 s | R19-130 | 2 | 10 / 1 | 3 |
| 236 | R19 | 201–202 s | R19-136 | 2 | 10 / 3 | 3 |
| 237 | R19 | 187–189 s | R19-162 | 2 | 6 / 4 | 3 |
| 238 | R19 | 178–180 s | R19-180 | 1 | 9 / 2 | 3 |
| 239 | R19 | 127–133 s | R19-236 | 2 | 10 / 5 | 3 |
| 240 | R19 | 117–121 s | R19-250 | 2 | 10 / 5 | 3 |
| 241 | R19 | 109–112 s | R19-263 | 2 | 10 / 2 | 3 |
| 242 | R19 | 103–106 s | R19-271 | 2 | 5 / 3 | 3 |
| 243 | R19 | 89–93 s | R19-289 | 2 | 10 / 5 | 3 |
| 244 | R19 | 75–80 s | R19-299 | 2 | 5 / 4 | 3 |
| 245 | R19 | 29–42 s | R19-333 | 0 | 1 / 3 | 3 |
| 248 | R20 | 80–82 s | R20-138 | 0 | 2 / 4 | 3 |
| 249 | R20 | 116–122 s | R20-193 | 0 | 0 / 2 | 3 |
| 250 | R20 | 137–139 s | R20-235 | 1 | 6 / 4 | 3 |
| 253 | R21 | 144–145 s | R21-043 | 2 | 2 / 1 | 3 |
| 255 | R21 | 78–81 s | R21-133 | 1 | 7 / 1 | 3 |
| 256 | R21 | 78–81 s | R21-133 | 1 | 1 / 1 | 3 |
| 257 | R21 | 47–49 s | R21-181 | 0 | 1 / 0 | 1 |
| 258 | R22 | 4–10 s | R22-009 | 0 | 11 / 1 | 3 |
| 259 | R22 | 22–26 s | R22-030 | 2 | 7 / 0 | 3 |
| 260 | R22 | 31–33 s | R22-038 | 1 | 0 / 5 | 3 |
| 261 | R22 | 46–48 s | R22-062 | 1 | 10 / 2 | 3 |
| 262 | R22 | 48–50 s | R22-067 | 2 | 9 / 4 | 3 |
| 263 | R22 | 52–54 s | R22-074 | 1 | 0 / 4 | 3 |
| 264 | R22 | 59–61 s | R22-090 | 2 | 10 / 0 | 3 |
| 265 | R22 | 64–65 s | R22-099 | 0 | 11 / 4 | 3 |

## Nicht eingetragen: unsicher (bitte prüfen)
Weiße Zellen direkt neben Bewuchs oder am Gestellrand zum Gras. Verschattung durch Pflanzen oder Randeffekte sind möglich.

| # | Reihe | Zeit | Position (geschätzt) | Ebene |
|---|---|---|---|---|
| 18 | R03 | 28–31 s | R03-43 | 2 |
| 69 | R06 | 389–394 s | R06-249 | 2 |
| 137 | R08 | 328–337 s | R08-246 | 2 |
| 139 | R08 | 327–342 s | R08-247 | 2 |
| 140 | R08 | 326–341 s | R08-248 | 1 |
| 153 | R10 | 86–90 s | R10-81 | 2 |
| 154 | R10 | 86–90 s | R10-82 | 2 |
| 155 | R10 | 85–89 s | R10-83 | 2 |
| 156 | R10 | 85–89 s | R10-84 | 2 |
| 185 | R13 | 156–170 s | R13-141 | 1 |
| 193 | R14 | 213–220 s | R14-280 | 2 |
| 194 | R14 | 218–219 s | R14-281 | 2 |

## Nicht eingetragen: Position nicht bestimmbar
Echte helle Zellen, deren Position außerhalb des Layouts landet (meist Reihenanfang/-ende oder Reihen mit unsicherer Zuordnung).

| # | Reihe | Zeit | Ebene |
|---|---|---|---|
| 17 | R03 | 20–30 s | 0 |
| 72 | R06 | 406–409 s | 1 |
| 85 | R06 | 498–501 s | 2 |
| 89 | R07 | 121–126 s | 2 |
| 128 | R07 | 1–5 s | 1 |
| 200 | R15 | 216–218 s | 2 |
| 205 | R15 | 216–218 s | 1 |
| 207 | R15 | 214–218 s | 0 |
| 233 | R19 | 249–250 s | None |
| 252 | R21 | 146–149 s | 2 |
| 254 | R21 | 123–125 s | 2 |
| 266 | R24 | 22–24 s | 1 |

## Verworfen
- Spiegelungsflecken (wandern mit der Kamera), Helligkeitssprünge der Kamera, warme Längsstreifen in Modulen (Strangmuster), helle Randstreifen zum Gras, Klemmen/Teile an Gestelllücken, Grasflächen neben den Gestellen (vor allem R15/R16 am Reihenanfang).

## Offene Punkte
- **R06:** Gemessen ca. 328 m Länge = 21 Gestelle à 15,6 m; im Tool hat R06 nur 20 Gestelle. Zuordnung vorläufig vom Westende aus; Befunde im östlichsten Gestell haben keine ID.
- **R15:** Westende im Video nicht sicher erkannt; Positionen in R15 sind unsicherer (±3).
- **R03:** Westende nicht erkannt; Zuordnung über Ostende und Lücken.
- **R09, R11, R23:** sehr wenige/keine Befunde; bitte stichprobenartig prüfen.
