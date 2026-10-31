# The Oven 🔥

A shelf of tiny browser games. **Adib bakes the ideas, Claude builds them.**

Every game is a single self-contained HTML file. No installs, no build step, no accounts. Open the page and press start.

**Play:** https://sakhadib.github.io/games/

## On the shelf

| Game | Type | Pitch |
|---|---|---|
| [The Shifting Dark](https://sakhadib.github.io/games/shifting-dark/) | 2D maze | Your torch shows almost nothing, and the maze rewrites itself wherever it isn't lit. Find the door before it moves. |

## How it works

1. **Bake** — Adib comes up with a game idea, rough or polished.
2. **Build** — Claude (Anthropic's AI) turns it into a small 2D or 3D game in plain HTML, CSS and JavaScript.
3. **Play** — The game lands on the shelf and goes live on GitHub Pages.

## Structure

```
index.html          ← the home page / game shelf
<game-name>/
  index.html        ← one game, fully self-contained
```

To add a game to the shelf, drop its folder in the repo and add an entry to the `GAMES` list near the bottom of `index.html`.

## Tech

- Canvas 2D for flat games, [Three.js](https://threejs.org/) from a CDN for 3D
- Keyboard and touch controls, so games work on phones too
- High scores saved in your browser with `localStorage`
- Sound made on the fly with the Web Audio API, so there are no asset files to load

## Credits

- Ideas and direction: [@sakhadib](https://github.com/sakhadib)
- Code: written by Claude, an AI model by [Anthropic](https://www.anthropic.com). Commits carry a `Co-Authored-By: Claude` line, so you can see exactly which work came from it.
