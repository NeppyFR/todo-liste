# Aufgaben (to-do list)

One-file German to-do list: `index.html`. No build step, no server code.

- Password: `cookiemonster:)`. Supabase checks it (project `todo`, account `aufgaben@example.com`); it isn't in the page source.
- Priorities 1 (Dringend) to 4 (Niedrig), or "Optional". Every task needs a deadline (Frist).
- Tasks are stored in the Supabase table `public.tasks`, so every device shows the same list.
  Row-level security limits them to the signed-in account. Other devices pick up changes when the page regains focus or every 30 s.
- The free Supabase project pauses after about a week without use; restore it from the Supabase dashboard (nothing is lost).
- To change the password: Supabase dashboard → Authentication → Users → `aufgaben@example.com`.

## Host on GitHub Pages

1. Create a new repository on GitHub and upload `index.html`.
2. Go to Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
3. After a minute the site is live at `https://<your-username>.github.io/<repo-name>/`.

## Run locally

Open `index.html` in a browser, or serve the folder (`python -m http.server`).
