# Personal Research Website

A simple, dependency-free personal website for GitHub Pages (plain HTML + CSS, auto dark mode, mobile friendly).

## Files

```
index.html            ← all page content (edit this)
assets/style.css      ← colours, fonts, layout
assets/img/profile.jpg  ← add your photo here
assets/files/CV.pdf     ← add your CV here
.nojekyll             ← tells GitHub to serve files as-is
```

## Publish on GitHub Pages

1. Create a GitHub account (e.g. username `srinivasthota`).
2. Create a **new public repository** named exactly `<username>.github.io`.
3. Upload these files (drag-and-drop via **Add file → Upload files**, or with git):
   ```bash
   git init
   git add .
   git commit -m "Initial website"
   git branch -M main
   git remote add origin https://github.com/<username>/<username>.github.io.git
   git push -u origin main
   ```
4. In the repo: **Settings → Pages → Source: Deploy from a branch → `main` / `(root)`** → Save.
5. After a minute, the site is live at `https://<username>.github.io`.

## Editing

- Replace every `[placeholder]` in `index.html`.
- Add a publication: copy one `<li>…</li>` block inside `<ol class="pubs">`.
- Change the accent colour: edit `--accent` in `assets/style.css`.
- Custom domain (optional): Settings → Pages → Custom domain.
