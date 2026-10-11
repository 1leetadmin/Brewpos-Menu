# BrewPOS online menu

The page customers open (from a printed QR code) to build an order while they
queue. Their phone then shows a 3-digit order number and a QR code that staff
scan at the counter. The till never goes online. See `docs/ONLINE_MENU.md` in
BrewPOS-Android / BrewPOS-Local-install-LAN-v1.

- `index.html` + `assets/`: the page, built with `npm run build:phone-menu`
  (from BrewPOS-Android `main`). Replace both when the page is rebuilt.
- `menu.json`: the menu. **The one here is a demo** and orders made with it
  will not scan on a till. Replace it with the file from the till:
  Settings > Advanced > Online features > Online menu > Download menu file.
  Upload a new one whenever the menu or prices change.

Hosting: GitHub Pages (Settings > Pages > Deploy from a branch > main / root).
GitHub Pages needs this repository to be public on a free GitHub plan.
