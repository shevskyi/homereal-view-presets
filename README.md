# HomeReel Preset Review

Static client review page for comparing HomeReel preset renders.

## Structure

```text
.
├── .gitignore
├── .nojekyll
├── README.md
├── index.html
├── home-reel-presets-personal-2026-06-12/
│   ├── 01-vhs85/
│   ├── 02-cam92/
│   └── ...
├── home-reel-presets-2026-06-10/
│   ├── 01-vhs85/
│   ├── 02-cam92/
│   └── ...
└── home-reel-presets-modern-2026-06-10/
    ├── 01-vhs85/
    ├── 02-cam92/
    └── ...
```

## What Is Inside

- `index.html` is the GitHub Pages entry point.
- `.nojekyll` keeps GitHub Pages in plain static-file mode.
- `.gitignore` blocks local `.DS_Store` noise.
- `home-reel-presets-personal-2026-06-12/` is Version 1, rendered from `DSCF0226.JPG` and `IMG_4033.MOV`.
- `home-reel-presets-2026-06-10/` is Version 2.
- `home-reel-presets-modern-2026-06-10/` is Version 3.
- Each version folder contains preset folders directly. There is no extra `presets/`, `sources/`, `manifest.json`, or nested README inside a version folder.
- Each preset row shows video before, video after, photo before, photo after.
- The page includes tabs for all versions, single-version review, video/photo filtering, preset shortcuts, and search.
- Each version has `Open video pair` and `Open photo pair` buttons for focused before/after review.
- The focused review modal includes `Open file` links for native browser/device viewing.

## GitHub Pages

Put all files from this folder into the root of a temporary GitHub repository.

If GitHub web upload blocks more than 100 files at once, upload in four passes:

```text
1. index.html, README.md, .nojekyll, .gitignore
2. home-reel-presets-personal-2026-06-12/
3. home-reel-presets-2026-06-10/
4. home-reel-presets-modern-2026-06-10/
```

Each version folder now contains 92 media files.

Then enable:

```text
Settings -> Pages -> Deploy from a branch -> main -> /root
```

GitHub Pages will serve:

```text
https://<username>.github.io/<repo-name>/
```

No build step. No Node.js. No server code.

## Local Preview

Open `index.html` directly in a browser, or run:

```bash
python3 -m http.server 4177
```

Then open:

```text
http://127.0.0.1:4177/
```

## Do Not Rename

Keep these folder names unchanged unless you also update the paths inside `index.html`:

- `home-reel-presets-2026-06-10`
- `home-reel-presets-modern-2026-06-10`
- `home-reel-presets-personal-2026-06-12`
