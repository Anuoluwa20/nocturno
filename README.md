# NOCTURNE

A 3D planner for apartments and workspaces: landing page, sign-up, onboarding, dashboard, layout and style pickers, 3D editor, budget, preview, walkthrough, export and settings.

## Run it
Serve the folder with any local web server (browsers block 3D textures from `file://`):

    npx serve .        # or: python3 -m http.server

then open the address it prints (for example http://localhost:3000).

Needs an internet connection for three.js (jsDelivr) and the fonts (Google Fonts: Newsreader, Instrument Sans).

## Files
- `index.html` — entry page; includes a static landing so it shows before scripts load
- `css/app.css` — design tokens and all styles
- `js/data.js` — furniture, materials, prices, styles, layouts
- `js/store.js` — saving (browser storage)
- `js/scene.js` — the three.js room: furniture, lighting, time of day, sketch view
- `js/app.js` — router, landing, sign-up, onboarding, dashboard, create flow, saved, settings
- `js/editor.js` — editor, budget, preview, walkthrough, share
- `img/` — images

Designs save in the browser's local storage. Prices are estimates, not live retail prices.
