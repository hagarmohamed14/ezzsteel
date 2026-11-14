# Ezz Flat Steel Smart Factory Dashboard (demo)

A static website: no build step, no server code, no environment variables.

## Files
- `index.html` the whole dashboard (HTML, CSS, JavaScript)
- `assets/` photos and logos, loaded with relative paths (keep this folder next to `index.html`)

## Deploy (any static host)
- **Vercel:** drag the unzipped folder into vercel.com/new, or run `vercel` inside it. Framework preset: Other. No build command, output directory `.`
- **Netlify:** drag the unzipped folder onto app.netlify.com/drop.
- **GitHub Pages:** put the files at the repository root, then Settings > Pages > Deploy from branch.
- **Any web server:** upload both `index.html` and `assets/`.
- **Run locally:** open `index.html` in a browser, or run `python -m http.server 8000` in this folder and visit http://localhost:8000

Important: always upload the `assets` folder together with `index.html`. If images are missing, the folder was not uploaded or was renamed.

## Notes
- Page fonts (Barlow) load from Google Fonts when online; the page falls back to system fonts offline.
- All data is demonstration data kept in the browser (localStorage). Nothing is sent anywhere.
- Roles, cameras, GPS, meters and the customer portal are simulated. Real use needs server-side login and real integrations (SCADA, ERP, CCTV, GPS).
