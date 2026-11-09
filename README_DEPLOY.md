# AquaGuard AI — Live Web Demo

A responsive, static, browser-based demonstration of the AquaGuard AI university water-monitoring concept.

## Preview locally
Open `index.html` in a modern browser. For best results, use a small local web server:
- VS Code: install/use Live Server, then right-click `index.html` → Open with Live Server.
- Or run `python -m http.server 8000` in this folder and visit `http://localhost:8000`.

## Deploy free with GitHub Pages
1. Create a public GitHub repository, for example `aquaguard-ai-demo`.
2. Upload **all files in this folder** (especially `index.html`) to the repository root.
3. Open repository **Settings → Pages**.
4. Under Build and deployment, choose **Deploy from a branch**.
5. Select branch `main`, folder `/ (root)`, then Save.
6. Wait for GitHub Pages to publish. Your public link will look like:
   `https://YOUR-GITHUB-USERNAME.github.io/aquaguard-ai-demo/`

Alternative: drag the folder into Netlify Drop at https://app.netlify.com/drop.

## What this demo contains
- Overview dashboard with five virtual meters and synthetic daily use charts.
- Candidate anomaly/event review with explanations and priority labels.
- Seven-day weekday-aware baseline forecast.
- Response-delay scenario calculator.
- Synthetic benchmark transparency and browser-side CSV validation/download.
- About, expected impact, limitations and future pilot information.

## Important accuracy note
This is a static frontend demonstration. It uses synthetic readings and illustrative candidate-event summaries. It does not connect to real campus sensors, run a production backend, or establish real-world leak detection accuracy. The CSV uploader validates a file in the browser for demonstration; it does not persist imported data into the dashboard. The benchmark labels are synthetic.

The charts use Chart.js from a public CDN and Google Fonts. An internet connection is required for those external assets; the core page and layout still load without them.
