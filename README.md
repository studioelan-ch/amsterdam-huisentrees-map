# Amsterdamse Huisentrees – MapLibre-Karte

Quelle: `Entrances — Classified by Type.kmz` (hochgeladen am 20.10.2026)

## Inhalt
- **346** Hauseingänge mit ursprünglichen Koordinaten und Adressen.
- Typen aus der KMZ: A1 (42), A3 (71), A4 (39), B1 (57), B2 (39), B3 (38), B4 (15), C1 (15), C3 (17), C4 (13).
- Schwarz-weisse Karte ohne Kartentexte, POI-Symbole oder My-Maps-Banner.
- Schwarze Punkte; Hover-Ring; Klick öffnet Adresse und Typ, optional Google-My-Maps-Foto. An 9 Doppelpositionen kann zwischen überlappenden Einträgen gewechselt werden.
- `index.html`: eigenständige Seite. Alle Hauseingänge sind darin bereits eingebettet. **Für die Darstellung müssen MapLibre (CDN) und OpenFreeMap (Kartendaten) über das Internet erreichbar sein.**
- `entrances.geojson`: separat exportierte Standorte, z. B. für spätere Aktualisierungen.

## Einbindung in Squarespace
1. `index.html` bei einem statischen Hoster veröffentlichen, z. B. GitHub Pages oder Cloudflare Pages. Den Online-Link prüfen.
2. In Squarespace auf der Projektseite einen **Code-Block** hinzufügen:

```html
<iframe
  title="Amsterdamse Huisentrees – interaktive Karte"
  src="https://EURE-ADRESSE-ZUR-KARTE/index.html"
  style="display:block;width:100%;height:650px;border:0;"
  loading="lazy"
  allowfullscreen>
</iframe>
```

3. Höhe nach Bedarf einstellen, für Mobilgeräte ggf. separat anpassen.

## Kartenstil ändern
Im `index.html` unter `const style`:
- Hintergrund `#ffffff`
- Wasser `#c7c7c7`
- Gebäude `#e5e5e5`
- Strassenlinien `#ececec`
- Punkte unter `id:'markers'` `#111111`

**Keine Beschriftungen:** Der Basisstil enthält absichtlich keine `symbol`-Layer. Die Attributions-/Lizenzhinweise zu OpenFreeMap/OpenStreetMap bleiben sichtbar.

## Bilder
Das KMZ verweist auf extern bei Google My Maps gespeicherte Fotos. Diese Links wurden in die Daten übernommen, **können aber ausserhalb von Google My Maps fehlschlagen**. In diesem Fall zeigt die Infokarte ausschliesslich Adresse und Typ. Für stabile Bilder sollten eigene, veröffentlichte Bild-URLs eingesetzt werden.

## Datennutzung und Lizenz
- Die MapLibre-Bibliothek ist Open Source.
- Kartengrundlage: OpenFreeMap/OpenStreetMap, Internet erforderlich. Nutzungsbedingungen und faire Verwendung vor umfangreicher Veröffentlichung prüfen. Attribution nicht entfernen.
- Die Karte zeigt sämtliche 346 Adressen/Standorte eurer KMZ. **Bitte vor einer öffentlichen Veröffentlichung prüfen, ob alle Wohnadressen und Bilder öffentlich sein sollen.**
- Es wurde kein Google-My-Maps-API-Key benötigt.
- Wenn keine Standortdaten automatisch zwischen My Maps und dieser Datei synchronisiert werden, muss die Karte bei späteren Ergänzungen neu exportiert / aktualisiert werden.

## Prüfung
- 346 Punkte mit Koordinaten aus der Originaldatei extrahiert.
- 10 Klassifikations-Codes übernommen.
- Laufzeitdarstellung benötigt Zugriff auf externe CDN- und Vektor-Kacheldienste; diese konnte in der isolierten Arbeitsumgebung **nicht live getestet** werden.
