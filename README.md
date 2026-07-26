# franciscorau.com — portfolio

Hand-written HTML/CSS/JS. No build step, no dependencies, no external requests.

| Page | What it is |
|---|---|
| `index.html` | Landing — three pillars |
| `staffing-simulator.html` | Capacity / cohort funnel simulator |
| `daily-agent-report.html` | Performance analytics (p70 frontier benchmarking) |
| `wallboard.html` | Live ops TV board (supervisor edition) |
| `unit-economics.html` | Floor P&L / unit-economics model |

All contact-centre data is fictional; no employer or client data appears anywhere.

## Publish

```bash
git remote add origin https://github.com/FranciscoRau08/<repo>.git
git branch -M main && git push -u origin main
```

Then **Settings → Pages → Deploy from a branch → main / (root)**, and
**Settings → Pages → Custom domain → franciscorau.com** (the `CNAME` file is already committed).

DNS at the registrar — apex `A` records to GitHub Pages:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

plus `www` as a `CNAME` to `franciscorau08.github.io`. Enable **Enforce HTTPS** once the certificate is issued.

## Preview locally

```bash
python3 -m http.server 8899 --directory ~/Downloads/portfolio-site
# → http://localhost:8899
```
