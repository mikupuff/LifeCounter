# Commander Life

A life counter for Magic: The Gathering with commander damage and poison, made to run as a home-screen app on iPhone.

## Using it
- **Tap** the left or right half of your panel to change life by 1. **Hold** to change it by 10, repeating while you hold.
- The **small colored numbers** on your panel's edges show the commander damage you've taken from each player. Each one sits on the side facing that player, or in the corner for the player diagonal from you. Tap one to show that damage as the big number. Changing it also changes your life the opposite way. Tap it again to go back, or wait 7 seconds.
- **☣** opens your poison counter the same way. It doesn't change life.
- **⚙︎** in the middle opens settings: player count (2–4), starting life, the lethal limits for commander damage and poison, names, colors, a "who goes first" picker and reset.
- **🔥** next to a name is that player's win streak: games won in a row. It goes up when they're the last one standing and resets when someone else wins. The win screen also shows total wins. Clear them in settings.
- The screen stays on while the app is open.
- Your game is saved automatically, so closing the app doesn't lose it.

## Publishing it with GitHub Pages
1. Create a new public repository on GitHub, for example `mtg-life`.
2. Upload `index.html`, `sw.js`, `manifest.webmanifest`, `icon-180.png` and `icon-512.png` to it. Use **Add file → Upload files**, or push with git.
3. In the repository, go to **Settings → Pages**. Under "Build and deployment", choose **Deploy from a branch**, then pick `main` and `/ (root)`, and save.
4. After a minute or so the site is live at `https://<your-username>.github.io/mtg-life/`.

## Putting it on your iPhone
1. Open that URL in **Safari**.
2. Tap **Share**, then **Add to Home Screen**.
3. Open it from the new icon. It runs fullscreen and works offline after the first load.

## Testing it on your computer
```bash
python -m http.server 8417
```
Then open http://localhost:8417. Use your browser's device toolbar to see a phone-sized screen.
