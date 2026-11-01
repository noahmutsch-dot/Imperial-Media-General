# PV Digitaler Zwilling

Einzelne statische Seite (`index.html`) zum Nachbilden von PV-Anlagen (Reihen, Module, Kacheln),
Markieren von Auffälligkeiten (Thermografie) und PDF-Export. Kein Build, kein Backend.

## Hosting (Hostinger)
`index.html` liegt im Repo-Root. In hPanel: Websites → Git → Repository verbinden, Branch wählen,
Installationspfad `public_html`. Danach genügt ein Deploy bei jedem Push.

## Hinweise
- Projekte und Hintergrundbilder werden im Browser (IndexedDB) des jeweiligen Geräts gespeichert, nicht auf dem Server.
- PDF-Export nutzt jsPDF per CDN (cdnjs), die Seite braucht dafür Internet.

## Projekt Karlstadt (Bestandsanlage Laudenbach)
Beim Öffnen wird die Anlage Laudenbach geladen (Quelle: Planunterlage Mai 2024, 3.496 kWp, 20.088 Module):
24 Reihen aus 372 Gestellen mit je 18 Positionen × 3 Module übereinander = 6.696 Positionen = 20.088 Module, auf dem Luftbild (in `index.html` eingebettet, keine separate Bilddatei nötig).
Gestelle je Reihe R01–R24: 3, 6, 10, 12, 2, 20, 21 (R07–R18), 19, 16, 13, 10, 6, 3.

- Reihen R01–R24 von Nord nach Süd, Positionen je Reihe von West nach Ost: `R05-023`. Ebene 1 = oben, 3 = unten.
- Suche: `R05-023` springt zur Position, `R05-G2` zum 2. Gestell der Reihe, `Reihe 12` zeigt die ganze Reihe.
- „Auffälligkeiten“ listet alle markierten Positionen, sortiert nach Schwere, Tipp springt hin.
- Die Gestellzahl je Reihe ist aus der Reihenlänge im Luftbild berechnet (Gestell ≈ 36 Bildpixel), nicht vor Ort gezählt; die Summe ergibt exakt die 372 Gestelle aus dem Plan. Einzelne Reihen können um ein Gestell abweichen.
- Das Projekt heißt „Projekt Karlstadt“. Markierungen werden automatisch im Browser gespeichert und beim Öffnen der Seite wieder geladen (gleicher Browser, gleiche Domain).
- Backup exportieren/importieren (Anlagenkonfiguration) sichert die Markierungen als Datei, auch für den Wechsel auf ein anderes Gerät.
- Das Luftbild ist standardmäßig gesperrt und wird beim Laden immer exakt zum Raster ausgerichtet.
