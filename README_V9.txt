AMSTERDAMSE HUISENTREES — Karte V9 | Stand 21. Oktober 2026

Paket: Veröffentlichung auf GitHub Pages / Einbindung auf studioelan.ch.

INHALT
- index.html — MapLibre-Karte mit Typologiefilter und Buchring
- entrances.geojson — Kartendaten (352 Datensaetze)
- photos/ — 345 lokal gehostete JPGs, davon sechs neue
- pruefbericht_v9.csv — Kontrollliste inkl. Koordinaten und Fotoreferenzen
- neue_6_koordinaten_pruefen.csv — die sechs ergaenzten Eintraege
- .nojekyll — GitHub Pages ohne Jekyll

DATENSTAND
- 346 alte + 6 neue Eingänge = 352 Kartenpunkte
- 100 verschiedene fuer das Buch ausgewaehlte Eingangsadressen, aber 102
  markierte Karten-Features, weil die Ausgangsdaten zwei doppelte Punkte enthalten.
  Doppelte Marker koennen deckungsgleich sein und sind optisch nicht doppelt sichtbar.
- 351 der 352 Features verweisen auf ein vorhandenes Foto. Oud-Zuid hat kein Bild.
- Keizersgracht 329 ist C1.
- Bei Klassifikationskonflikten wurde die Typologie aus dem Buch-PDF uebernommen.

POSITIONEN — VOR LIVE-SCHALTUNG KURZ PRUEFEN
IDs 348 und 351 sind anhand direkter Nachbaradressen angenaehert, weil keine
exakten amtlichen Hauskoordinaten in diesem Arbeitsdurchlauf abgerufen werden
konnten. Sie liegen nahe beim richtigen Gebaeude, nicht garantiert metergenau.
  348 Isaac Titsinghkade 203, B1: 4.930565, 52.372530
  351 Postjeskade 71B, C4: 4.852240, 52.363155

Die restlichen vier neuen Standorte beruhen auf standort- oder gebaeudeweisen
Adressdaten oder auf einem georeferenzierten Bild des Hauses. Auch diese Punkte
sollten auf der live Karte kurz angesehen werden.

VEROEFFENTLICHUNG
1. Bestehendes GitHub-Repository lokal sichern/klonen (GitHub Desktop).
2. Alle Dateien aus diesem ZIP ins Repository-Stammverzeichnis kopieren.
3. Aeltere V8-Dateien und Bilddateien nicht versehentlich zurueckkopieren.
4. In GitHub Desktop Changes pruefen > Commit > Push origin.
5. In Settings > Pages sicherstellen: Deploy from a branch, main, /root.
6. Nach kurzer Zeit Pages-URL oeffnen, Bilder, Typologiefilter und Buchring testen.
7. Bestehendes Squarespace-Embed zeigt bei unveraenderter GitHub-Pages-URL
   die neue Karte ohne Anpassung des Embed-Codes.

ABHAENGIGKEITEN
MapLibre aus unpkg.com, Basiskarte aus OpenFreeMap. Internetverbindung erforderlich.
