# hero-backgrounds

Animated canvas backgrounds for a hero section, in one small file. No dependencies, no network calls.

**[Live demo](https://holroydchase-afk.github.io/hero-backgrounds/)**

## Use

```html
<section id="hero"><h1>Your headline</h1></section>
<script src="hero-backgrounds.js"></script>
<script>
  HeroBG("#hero", { mode: "constellation", color: "#4A6B4C", speed: 1, density: 1 });
</script>
```

`HeroBG(el, options)` returns `{ setOptions, destroy }`.

| Option | Default | What it does |
|---|---|---|
| `mode` | `constellation` | Which background to draw |
| `color` | `#4A6B4C` | Accent colour |
| `speed` | `1` | `0` freezes, `2` is double |
| `density` | `1` | More or fewer elements |
| `mouse` | `true` | React to the pointer where the mode supports it |
| `background` | `null` | CSS colour behind the canvas |

## Modes

`constellation`, `neural`, `organic`, `flow`, `grid`, `dots`, `waves`, `threads`, `aurora`, `mesh`, `orb`. The list is also at `HeroBG.modes`.

## Performance and motion

Frames are drawn on `requestAnimationFrame`, which the browser syncs to the display and stops in hidden tabs. An `IntersectionObserver` also stops the loop while the element is scrolled off screen and restarts it when it returns. With `prefers-reduced-motion: reduce`, or `speed: 0`, it draws one still frame and no loop runs. Canvas resolution is capped at 2x.

## License

MIT. See [LICENSE](LICENSE).
