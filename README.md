# Hoop Duel

One-on-one full-court basketball as an installable web app (PWA). Highest score at the buzzer wins; a tie goes to overtime, where the next basket wins.

**Play:** https://matdata-eu.github.io/game-basket-duel/

## Modes
- **Pick your team**: BB Bulldogs ([Boortmeerbeek & Berg Bulldogs](https://www.bbbulldogs.be/)) is the default, with the club logo on the shirt. Pink Flamingos, Teal Sharks and Gold Hornets are the other kits. Against a bot, the bot takes a contrasting kit.
- **Bot**: you (teal) against a bot (pink) on Easy, Medium or Hard. Harder bots react faster, move quicker, time their shots better, steal and block more.
- **2 Players**: two people on one device. Keyboard: P1 `A D` move, `W` jump, `S` shoot. P2 `← →` move, `↑` jump, `↓` shoot. On a touchscreen each player gets buttons on their side.

## How to play
- Hold **Shoot** to rise up and release at the top of the jump. The meter next to you shows the timing. Close to the rim it becomes an automatic layup.
- Shots taken beyond the three-point line count for 3.
- Without the ball, **Shoot** near the ball handler tries a steal and **Jump** contests or blocks shots.
- 12-second shot clock; `P` or `Esc` pauses.

## Install
Open the game in Chrome, Edge or Safari and choose "Install" or "Add to Home Screen". After the first load it works offline.

## Run locally
No build step. Serve the folder over `localhost` or HTTPS, for example:

```sh
python3 -m http.server 8000
```

Files: `index.html` (the whole game), `manifest.webmanifest`, `sw.js` (offline cache), `icons/`. Pushes to `main` deploy to GitHub Pages through `.github/workflows/pages.yml`.

## Support
Found a bug or have an idea? [Open an issue](https://github.com/Matdata-eu/game-basket-duel/issues).

## Credits
- Game, graphics and sound effects: made from scratch in code (canvas drawing, Web Audio), no third-party assets.
- Fonts: [Bungee](https://fonts.google.com/specimen/Bungee) by David Jonathan Ross and [Barlow Condensed](https://fonts.google.com/specimen/Barlow+Condensed) by Jeremy Tribby, both under the SIL Open Font License, loaded from Google Fonts.
- BB Bulldogs logo and colours belong to [Boortmeerbeek & Berg Bulldogs](https://www.bbbulldogs.be/) and are not covered by the MIT license.
- Built by [Matdata](https://matdata.eu) with [Claude Code](https://claude.com/claude-code).

## License
[MIT](LICENSE), except the BB Bulldogs logo (see Credits).
