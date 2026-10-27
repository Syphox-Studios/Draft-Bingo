# Draft Bingo V1.1

Draft Bingo is a game where you and your friends will first draft the games that you will be playing then draft goals for them games. There are 18 games included in this at the moment with plans to add many more. Each game has at least 15 goals with plans to also make more for each game. 

There are currently 4 Gamemodes:
1. **Traditional Lockout**: Once a square is claimed its locked for all other players. It's first to complete one line unless no lines are available then its first to have over half the goals.
2. **BINGO**: First to complete the designated number of lines.
3. **Blackout**: First to complete every square on the board.
4. **Timed Race**: A time limit is given, it is whoever completes the most goals within that given time. Lockout and Non-Lockout versions are avaliable.

If you have more than 2 players then there is another setting called play mode, the 2 options are below:
1. Free For All: Everyone playing is their own team.
2. Teams: Players are split in 2 random teams, teammates share a color and any can pick the games and goals.

To **Play** click on this link: [syphox-studios.github.io/Draft-Bingo/](https://syphox-studios.github.io/Draft-Bingo/)

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
