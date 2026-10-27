# Draft Bingo

A drafting bingo game for you and your friends. Static site, no build step.

## Run it locally
Serve the folder (fonts won't load reliably from `file://`):

    python3 -m http.server

then open http://localhost:8000

## Deploy on GitHub Pages
1. Push this folder to a GitHub repo (`index.html` at the root).
2. Repo **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, folder `/ (root)`.
3. Your site goes live at `https://<username>.github.io/<repo>/`.

## Structure
- `index.html` – the whole app
- `game-photos/` – box art (filenames must match exactly, GitHub Pages is case-sensitive)
- `fonts/` – Jersey 10 and Limelight, with their OFL licences

Online play uses PeerJS (loaded from unpkg), so it needs an internet connection and HTTPS, which Pages provides.
