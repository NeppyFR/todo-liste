# Aufgaben (to-do list)

One-file German to-do list: `index.html`. No build step, no server code.

- Password: `cookiemonster:)` (a plain client-side check, not real security; anyone who reads the page source can see it).
- Priorities 1 (Dringend) to 4 (Niedrig), or "Optional". Every task needs a deadline (Frist).
- Tasks are stored in the browser's `localStorage`: they stay on that device and in that browser only.
  Clearing browsing data deletes them. Safari can also wipe them if the site isn't opened for about a week.
  Use "Sicherung herunterladen" / "Sicherung laden" at the bottom to back up or move tasks.

## Host on GitHub Pages

1. Create a new repository on GitHub and upload `index.html`.
2. Go to Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
3. After a minute the site is live at `https://<your-username>.github.io/<repo-name>/`.

## Run locally

Open `index.html` in a browser, or serve the folder (`python -m http.server`).
