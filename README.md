# Timer

A quiet countdown timer. Set a length and a warning point: a soft chime rings
at the warning, and at zero a gentle two-note tone plays and a voice says
"The time is over."

Live at **[timer.actionsmatter.com](https://timer.actionsmatter.com)**.

## What it does

- Set the length and the warning point as `mm:ss`, `h:mm:ss`, or a plain number for minutes
- Light chime at the warning, spoken finish at zero
- Save common times and load them with one click
- Space starts and pauses, `R` resets

## How it works

One `index.html` file. No build step, no dependencies, no tracking, no network
calls except the webfont. The chime and the end tone are synthesized with the
Web Audio API, the spoken line uses the browser's own
`speechSynthesis`, and saved times live in `localStorage` — nothing leaves your
browser.

## Running it

Open `index.html`, or serve the folder:

```
python3 -m http.server 8000
```

## License

MIT — see [LICENSE](LICENSE).
