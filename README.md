# MA-Case-Study

Einfache, statische Web-App für eine M&A-Case-Study im Unterricht.

## Enthalten
- Flexible Gruppeneinteilung in **immer 4 Gruppen** (auch wenn Teilnehmerzahl nicht 20 ist)
- Geeignet für den Standardfall mit **20 Studierenden** in **4 Gruppen à 5 Personen**
- Integrierte Inhalte der alten Wintergerst-Lorch-Case-Study
- Gruppenmodus über URL (`?group=1` bis `?group=4`), damit Gruppen in unterschiedlichen Versionen arbeiten
- Auswahl der Peer-Referenz je Gruppe: `FY-1`, `FY0`, `LTM`, `NTM`
- Gruppennotizen je Gruppe separat im Browser gespeichert

## Nutzung
1. Lehrkraft öffnet die Seite ohne URL-Parameter und erstellt die 4 Gruppen.
2. Für Gruppenarbeit je Link verteilen: `?group=1`, `?group=2`, `?group=3`, `?group=4`.
3. Jede Gruppe arbeitet in ihrer eigenen Version und sieht nur ihren Gruppenbereich.

## Lokal starten
```bash
python3 -m http.server 8080
```
Dann im Browser öffnen: <http://localhost:8080>

## Deployment auf Vercel
1. Repository zu GitHub pushen.
2. In Vercel **Add New Project** wählen und das Repository importieren.
3. Framework Preset auf **Other** lassen.
4. Kein Build Command nötig, direkt deployen.

Die App nutzt nur `index.html` und `vercel.json` und ist direkt deploybar.
