# lizhongc.github.io

Source files for my personal academic homepage, written in [jemdoc](http://jemdoc.jaboc.net/)
and served via GitHub Pages.

🔗 **Live site:** https://lizhongc.github.io

## How it works

The site is generated from a single jemdoc source file:

```
index.jemdoc  ──(jemdoc generator)──►  index.html  ──(git push)──►  GitHub Pages
```

- **`index.jemdoc` is the source of truth.** Edit the content there.
- **`index.html` is generated** — do not edit it by hand; it is overwritten on
  every build.
- Styling lives in `jemdoc.css`.

## Build locally

Requires **Python 3**. From the repository root:

```bash
python3 jemdoc3.py index.jemdoc
```

This regenerates `index.html`. Commit and push to publish.

> `jemdoc3.py` is a Python 3 port of the upstream `jemdoc.py` (which targets
> Python 2 and is kept only for reference). LaTeX equation support is optional and
> requires `latex` and `dvipng` to be installed.

## Repository structure

| Path | Description |
| --- | --- |
| `index.jemdoc` | Page content (jemdoc markup) — **edit this** |
| `index.html` | Generated output — do not edit |
| `jemdoc.css` | Stylesheet |
| `jemdoc3.py` | jemdoc generator (Python 3) |
| `jemdoc.py` | Original jemdoc generator (Python 2, reference only) |
| `lizhong.png` | Name logo shown beside the title |
| `2024new.jpg` | Profile photo |
| `Academic_CV.pdf` | Curriculum vitae |
| `master_thesis.pdf` | Master's thesis |
| `*_presentation.pdf`, `*_EuroBioc.pdf` | Talk slides linked from the site |

## Credits & license

Built with [jemdoc](http://jemdoc.jaboc.net/) by Jacob Mattingley, licensed under
the GNU GPLv3; `jemdoc3.py` is a local Python 3 port of it. All other content
(text, images, documents) is personal site material.
