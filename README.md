# Copper Supply Globe

Interactive 3D globe dashboard showing port-to-port copper (concentrate and cathode) flows. Built with [globe.gl](https://globe.gl). Static site, no build step.

## Run locally
Open `index.html` in a browser, or run `python3 -m http.server` and visit http://localhost:8000.

## Publish with GitHub Pages
1. Create a new GitHub repository (e.g. `copper-supply-globe`).
2. Upload `index.html` and `README.md` (or push via git):
   ```bash
   git init && git add . && git commit -m "Copper supply globe"
   git branch -M main
   git remote add origin https://github.com/<your-username>/copper-supply-globe.git
   git push -u origin main
   ```
3. In the repo go to **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and Save.
4. After a minute your dashboard is live at `https://<your-username>.github.io/copper-supply-globe/`.

## Use your own data
Edit the `PORTS` (name → lat, lng, country) and `ROUTES` (from, to, kt per year, type) arrays at the top of the script in `index.html`. Current volumes are illustrative estimates, not official statistics.
