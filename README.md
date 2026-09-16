# Pomodoro Focus Timer

A modern, self-contained Pomodoro timer with a dark, minimal interface. Built with pure HTML, CSS, and JavaScript — no frameworks, no dependencies, no build step.

## Features

- **Focus / Break modes** — 25-minute focus sessions and 5-minute breaks, toggled with a single click
- **Circular progress ring** — a gradient ring visibly counts down in sync with the timer
- **Start / Pause / Reset controls** — simple, predictable session management
- **Persistent session counter** — completed focus sessions are saved to `localStorage` and survive page refreshes
- **Dark mode UI** — clean typography, centered layout, subtle glow and shadow effects
- **Zero dependencies** — a single `index.html` file with embedded CSS and JS

## Usage

1. Open `index.html` in any modern web browser.
2. Choose **Focus** or **Break** mode using the toggle at the top.
3. Press **Start** to begin the countdown.
4. Use **Pause** to stop the countdown temporarily, or **Reset** to restart the current mode from its full duration.
5. When a focus session completes, the counter increments automatically and the timer switches to break mode (and vice versa).

## Project Structure

```
index.html   # Complete app — markup, styles, and logic in one file
```

## Technical Notes

- The countdown is driven by `setInterval`, ticking once per second.
- The circular progress ring is an SVG `<circle>` whose `stroke-dashoffset` is updated each tick to reflect remaining time.
- Session count is stored under the `pomodoro_sessions` key in `localStorage`.
- No external scripts, stylesheets, or fonts are loaded — the app works fully offline.

## Browser Support

Works in any modern browser with standard support for SVG, CSS gradients, and `localStorage` (Chrome, Firefox, Safari, Edge).

## License

Free to use, modify, and distribute.
