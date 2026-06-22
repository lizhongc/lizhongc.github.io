# lizhongc.github.io

Source files for my personal academic homepage, written in [jemdoc](http://jemdoc.jaboc.net/)
and served via GitHub Pages.

🔗 **Live site:** https://lizhongc.github.io

## How it works

The site is generated from a single jemdoc source file:

- **`index.jemdoc` is the source of truth.** Edit the content there.
- **`index.html` is generated** — do not edit it by hand; it is overwritten on
  every build.
- Styling lives in `jemdoc.css`.

## Build locally

Requires **Python 3**. From the repository root:

```bash
python3 jemdoc3.py index.jemdoc
```

> `jemdoc3.py` is a Python 3 port of the upstream `jemdoc.py` (which targets
> Python 2 and is kept only for reference). LaTeX equation support is optional and
> requires `latex` and `dvipng` to be installed.

## Credits & license

Built with [jemdoc](http://jemdoc.jaboc.net/) by Jacob Mattingley, licensed under
the GNU GPLv3; `jemdoc3.py` is a local Python 3 port of it. All other content
(text, images, documents) is personal site material.
