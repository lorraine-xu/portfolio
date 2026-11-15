# Lorraine Xu – personal site

Live at **https://lorraine-xu.github.io/portfolio/**

A static, single-page site: `index.html` plus `assets/` (video covers and computer-vision thumbnails).
No build step. Demo videos load only when a visitor presses play (YouTube via youtube-nocookie, PartSelect via Loom).
The CS180 project pages stay in the separate `lorraine-xu.github.io` repo; this site links to them.

## Preview locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Publishing

GitHub Pages serves the `main` branch root (Settings → Pages). Push to `main` and the site updates within a minute or two.

## Editing

All content is plain HTML in `index.html`, grouped by section (Research, Projects, Vision, Experience, Papers, About).
To add a project with a YouTube demo, copy one `<article class="proj">` block, set `data-yt` to the video ID,
and save the cover as `assets/yt-<ID>.jpg` (from https://i.ytimg.com/vi/<ID>/maxresdefault.jpg).
