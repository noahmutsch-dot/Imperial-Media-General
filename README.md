# PV Digitaler Zwilling

Einzelne statische Seite (`index.html`) zum Nachbilden von PV-Anlagen (Reihen, Module, Kacheln),
Markieren von Auffälligkeiten (Thermografie) und PDF-Export. Kein Build, kein Backend.

## Hosting (Hostinger)
`index.html` liegt im Repo-Root. In hPanel: Websites → Git → Repository verbinden, Branch wählen,
Installationspfad `public_html`. Danach genügt ein Deploy bei jedem Push.

## Hinweise
- Projekte und Hintergrundbilder werden im Browser (IndexedDB) des jeweiligen Geräts gespeichert, nicht auf dem Server.
- PDF-Export nutzt jsPDF per CDN (cdnjs), die Seite braucht dafür Internet.
