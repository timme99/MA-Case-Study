# MA-Case-Study

Statische Web-App für die Organisation einer M&A-Case-Study im Unterricht.

## Enthalten
- Feste Einteilung in **4 Gruppen** (auch wenn Teilnehmerzahl nicht 20 ist)
- Integrierte Inhalte der alten Wintergerst-Lorch-Case-Study
- Gruppenmodus über URL (`?group=1` bis `?group=4`), damit Gruppen in unterschiedlichen Versionen arbeiten
- Auswahl der Peer-Referenz je Gruppe: `FY-1`, `FY0`, `LTM`, `NTM`
- Gruppennotizen je Gruppe separat im Browser gespeichert

## Nutzung
1. Lehrkraft öffnet die Seite ohne URL-Parameter, erstellt die 4 Gruppen.
2. Für Gruppenarbeit je Link verteilen: `?group=1`, `?group=2`, `?group=3`, `?group=4`.
3. Jede Gruppe arbeitet in ihrer eigenen Version und sieht nur ihren Gruppenbereich.

## Lokal starten
```bash
python3 -m http.server 8080
```
Dann: <http://localhost:8080>

## Vercel Deployment
1. Repo nach GitHub pushen.
2. In Vercel: **Add New Project** und Repository importieren.
3. Framework Preset: **Other**.
4. Kein Build Command nötig, direkt deployen.
