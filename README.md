# Portfolio site — franciscorau

One self-contained `index.html`. No build step, no dependencies.

## Publish on GitHub Pages (5 minutes)

```bash
cd ~/Downloads/portfolio-site
git init && git add index.html README.md && git commit -m "Portfolio site"
# create the repo on github.com: FranciscoRau08/portfolio (public), then:
git remote add origin https://github.com/FranciscoRau08/portfolio.git
git branch -M main && git push -u origin main
```

Then on GitHub: repo → **Settings → Pages → Source: Deploy from a branch → main / (root)**.
Live a minute later at **https://franciscorau08.github.io/portfolio/**

## After it's live

1. LinkedIn → **Featured** → Add link → the Pages URL.
2. Add the URL to both CVs (contact line).
3. Optional: make the Weatherbot repo public and add a link to its card in
   `index.html` (it currently has no repo link because the repo is private).

## Preview locally

```bash
python3 -m http.server 8899 --directory ~/Downloads/portfolio-site
# → http://localhost:8899
```
