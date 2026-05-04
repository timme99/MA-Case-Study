# MA-Case-Study

Simple, static web app for an M&A case study in class.

## Included
- Flexible group setup with **always 4 groups** (even if there are not exactly 20 participants)
- Suitable for the standard setup with **20 students** in **4 groups of 5 people**
- Integrated content from the former Wintergerst-Lorch case study
- Group mode via URL (`?group=1` to `?group=4`) so groups can work in separate versions
- Per-group peer reference selection: `FY-1`, `FY0`, `LTM`, `NTM`
- Group notes are stored separately per group in the browser
- Results section with checklist for linked result sheets per group
- Simplified discussion questions (e.g., pricing impact: strategic buyer vs. financial investor)
- Additional hint boxes for unclear points in plain language

## Usage
1. Instructor opens the page without URL parameters and sets up the 4 groups.
2. Share one link per group: `?group=1`, `?group=2`, `?group=3`, `?group=4`.
3. Each group works in its own version and only sees its own group area.

## Run locally
```bash
python3 -m http.server 8080
```
Then open in your browser: <http://localhost:8080>

## Deploy on Vercel
1. Push the repository to GitHub.
2. In Vercel, choose **Add New Project** and import the repository.
3. Leave Framework Preset as **Other**.
4. No build command needed; deploy directly.

The app only uses `index.html` and `vercel.json` and can be deployed directly.
