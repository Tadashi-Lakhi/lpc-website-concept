# Lusaka Press Club — Website Concept

A multi-page static site design concept for Lusaka Press Club, built for presenting to the Executive Committee.

**This is a design concept, not the official Lusaka Press Club website.** Contact details, event dates, and committee names are placeholders — replace them before any real launch.

## Pages

| Page | File |
|---|---|
| Home | `index.html` |
| About | `about.html` |
| Advocacy | `advocacy.html` |
| Membership | `membership.html` |
| Events | `events.html` |
| Newsroom | `newsroom.html` |
| Contact | `contact.html` |

## Host it on GitHub Pages (for presenting)

1. Create a new repository on GitHub (e.g. `lpc-website-concept`) and push this folder to it:
   ```bash
   git init
   git add .
   git commit -m "LPC website concept"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/lpc-website-concept.git
   git push -u origin main
   ```
2. On GitHub, go to **Settings → Pages**.
3. Under **Source**, choose the `main` branch and `/ (root)` folder, then **Save**.
4. GitHub will publish the site at:
   `https://YOUR-USERNAME.github.io/lpc-website-concept/`
   (takes 1–2 minutes to go live after the first push)

Share that link directly in the presentation — it works on any device, no download needed.

## Local preview (no GitHub required)

Just double-click `index.html` to open it in a browser, or run a local server from this folder:
```bash
python3 -m http.server 8000
```
then visit `http://localhost:8000`.

## Structure

```
/
├── index.html
├── about.html
├── advocacy.html
├── membership.html
├── events.html
├── newsroom.html
├── contact.html
├── assets/
│   ├── css/style.css     ← all styling, shared across every page
│   └── js/main.js        ← mobile nav, scroll reveal, form handling
└── README.md
```

## Before a real launch

- Replace the membership and contact forms' demo handler in `assets/js/main.js` with a real endpoint (e.g. [Formspree](https://formspree.io)).
- Add real Executive Committee names on `about.html`.
- Replace placeholder address, phone and email in the footer and `contact.html`.
- Swap the map placeholder on `contact.html` for a real embedded map.
- Replace news thumbnail gradients with real photography.
