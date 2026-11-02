# The Oven 🔥

A shelf of tiny browser games. **Adib bakes the ideas, Claude builds them.**

Every game is a single self-contained HTML file. No installs, no build step, no accounts. Open the page and press start.

**Play:** https://sakhadib.github.io/games/

## On the shelf

| Game | Type | Pitch |
|---|---|---|
| [The Shifting Dark](https://sakhadib.github.io/games/shifting-dark/) | 2D maze | Your torch shows almost nothing, and the maze rewrites itself wherever it isn't lit. Find the door before it moves. |
| [Pocket Snake](https://sakhadib.github.io/games/pocket-snake/) | 2D arcade | Classic snake on a little black-and-white phone screen. Eat dots, chase the runaway mouse, and don't bite yourself. |
| [Pocket Strike](https://sakhadib.github.io/games/pocket-strike/) | 2D shooter | A side-scrolling space shooter on a monochrome LCD. Saucers, asteroids, power-ups, and a boss at the end of every stage. |
| [Pocket Bounce](https://sakhadib.github.io/games/pocket-bounce/) | 2D platformer | An endless bouncing-ball runner. The road builds itself as you go; shrink to squeeze through tunnels, grow to float and smash walls. |
| [Sky Stacker](https://sakhadib.github.io/games/sky-stacker/) | 2D arcade | Time the swinging crane and drop each floor. Chain perfect drops, fight the wind, and fill your tower with tiny residents. |
| [Roll Rush](https://sakhadib.github.io/games/roll-rush/) | 2D arcade | The platforms rise and the ceiling is spikes. Roll down, chain freefall combos, grab power-ups, and dive through six zones. |
| [Balloon Bow](https://sakhadib.github.io/games/balloon-bow/) | 2D archery | Old-school archery in a classic desktop window. Aim, charge, run for arrow packs, and don't let 10 balloons escape. |
| [Night Landing](https://sakhadib.github.io/games/night-landing/) | 2D arcade | Your UFO sinks lower every pass over a dark city. Drop one bomb at a time, clear the skyline, and land. |
| [Coop Catch](https://sakhadib.github.io/games/coop-catch/) | 2D arcade | Hens on a rail lay eggs; run with your basket to catch them, dodge rotten eggs, and grab booster eggs. Five lives. |
| [Light Fingers](https://sakhadib.github.io/games/light-fingers/) | 2D stealth | Steal every coin in a dark apartment while a policeman sweeps his torch. In the light you're slowed. Run, hide in wardrobes, don't get caught. |

## How it works

1. **Bake** — Adib comes up with a game idea, rough or polished.
2. **Build** — Claude (Anthropic's AI) turns it into a small 2D or 3D game in plain HTML, CSS and JavaScript.
3. **Play** — The game lands on the shelf and goes live on GitHub Pages.

## Structure

```
index.html            ← the home page / game shelf (static cards, search, filters)
<game-name>/
  index.html          ← one game, fully self-contained
assets/shots/         ← 1200×630 screenshots used on the shelf and for link previews
assets/site.css       ← shared style for the text pages
contributing.html     ← contribution rules
terms.html, privacy.html, 404.html
sitemap.xml, manifest.webmanifest
```

## Bake your own

Want your game on the shelf? Read the [contribution rules](https://sakhadib.github.io/games/contributing.html), then:

1. [Fork this repo](https://github.com/sakhadib/games/fork).
2. Add your game as `your-game/index.html`, plus a screenshot at `assets/shots/your-game.jpg`.
3. Add a card at the end of the shelf in `index.html`, and list the game in `sitemap.xml` and the table above.
4. Open a pull request with a short pitch and a screenshot.

## Tech

- Canvas 2D for flat games, [Three.js](https://threejs.org/) from a CDN for 3D
- Keyboard and touch controls, so games work on phones too
- High scores saved in your browser with `localStorage`
- Sound made on the fly with the Web Audio API, so there are no asset files to load

## Credits

- Ideas and direction: [Sakhawat Adib](https://portfolio.sakhawatadib.com) ([@sakhadib](https://github.com/sakhadib))
- Code: written by Claude, an AI model by [Anthropic](https://www.anthropic.com). Commits carry a `Co-Authored-By: Claude` line, so you can see exactly which work came from it.

See also: [Terms](https://sakhadib.github.io/games/terms.html) · [Privacy](https://sakhadib.github.io/games/privacy.html)
