Costrequest — Price Compare Prototype
A working prototype for the Costrequest concept: a cost-comparison shopping app
that lets a user build a cart, see it priced across multiple supermarkets side
by side, spot the cheapest store instantly, and print/save the order — plus a
second module surfacing related financial services (banking costs, MMF rates,
government securities, SACCO dividends).
What's in here
`index.html` — the full prototype. Single file, no build step, no dependencies.
`assets/` — logo files (PNG and SVG versions of the Costrequest mark).
Running it locally
No server or install required — just open `index.html` in a browser.
If you'd rather serve it locally:
```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```
Deploying (free, via GitHub Pages)
Push this repo to GitHub (see commands below).
In the repo on GitHub: Settings → Pages → Deploy from branch → main → / (root).
GitHub will publish it at `https://<your-username>.github.io/<repo-name>/`.
Pushing this repo to GitHub
```bash
# Create an empty repo on GitHub first (no README/license — this repo already has one),
# then from inside this project folder:

git remote add origin https://github.com/<your-username>/costrequest-prototype.git
git branch -M main
git push -u origin main
```
Current state / what's mocked
Product catalog and store prices (`Carrefour`, `Naivas`, `Quickmart`,
`Chandarana`) are hardcoded sample data in `index.html`.
The Financial Services tab (banking costs, MMF rates, T-bills/bonds, SACCO
dividends) is also sample data, intended to later be wired to live feeds.
No backend — this is a front-end-only prototype for validating the concept
and UX before investing in real data integrations.
Suggested next steps
Replace hardcoded product/price data with a real feed or admin-editable source.
Connect banking, MMF, and T-bill data to live sources.
Decide on a backend (for saved carts, user accounts, price history) if the
concept moves past prototype stage.
