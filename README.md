# MA-Case-Study

Einfache, statische Web-App für eine M&A-Case-Study mit:

- Gruppeneinteilung für **20 Studierende** in **4 Gruppen à 5 Personen**
- Ablauf für Bearbeitung der Case Study
- Abschlusspräsentation inkl. Q&A
- Vorschläge für Diskussionsfragen (z. B. Preiswirkung bei Finanzinvestor vs. Strategen)

## Lokaler Start

Da die App rein statisch ist, genügt ein einfacher Static-Server, z. B.:

```bash
python3 -m http.server 8080
```

Dann im Browser öffnen: <http://localhost:8080>

## Deployment auf Vercel

1. Repository zu GitHub pushen.
2. In Vercel "Add New Project" wählen und das Repo importieren.
3. Framework Preset auf **Other** lassen (kein Build Command erforderlich).
4. Deploy starten.

Die App nutzt nur `index.html` + `vercel.json` und ist direkt deploybar.
