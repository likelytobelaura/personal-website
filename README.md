# personal-website

Laura Bocek's personal site. The landing page (`index.html`) is a self-contained
8-bit rugby scene rendered on a `<canvas>` — no build step, no dependencies
(fonts load from Google Fonts).

## The scene

- Blue vs. red, blue attacking up the pitch from a **left-side scrum**.
- It's **blue's ball**: a 3-2-3 pack is bound down, the backs stand in an
  attacking line outside the scrum (9, 10, 12, 13, 11, 15), and the **fly-half
  (10)** already has it in hand.
- Move the cursor over the scene — the crowd is nudged aside and the fly-half
  **twists to track the pointer**.
- Click a nav button (`HOME` / `LINKEDIN` / `GITHUB` / `SUBSTACK`) and the
  fly-half **kicks the ball in an arc into that button**, which flashes on
  impact. Destinations aren't wired yet — the kick is animation only.
- Respects `prefers-reduced-motion` (no idle jitter, no screen shake).

## Run it locally

Just open the file:

```sh
open index.html
```

or serve the folder:

```sh
python3 -m http.server
```

## Deploy

No domain yet. When ready, GitHub Pages serves this repo as-is
(Settings → Pages → deploy from `main` / root), and a custom domain can be
pointed at it later.

## Next

- Wire the nav buttons to real URLs once the pages exist.
- Split `index.html` into `index.html` + `assets/` if the site grows past one page.
