# Matthew J. Baker — Quarto academic site

A minimal personal academic website built with Quarto and designed for GitHub Pages.

## 1. Install Quarto

Download Quarto from https://quarto.org/docs/get-started/ or install it using your preferred package manager.

VS Code is optional but convenient.

## 2. Preview locally

Open a terminal in this folder and run:

```bash
quarto preview
```

The site will open in your browser. Edit any `.qmd` file and the preview will refresh.

## 3. Render the site

```bash
quarto render
```

The finished HTML site will be written to the `docs/` directory.

## 4. Put it on GitHub

Create a repository. If you want your main personal site at `https://YOURUSERNAME.github.io`, name the repository exactly:

`YOURUSERNAME.github.io`

Otherwise, any repository name works and the address will be `https://YOURUSERNAME.github.io/REPOSITORY/`.

Then initialize/push:

```bash
git init
git add .
git commit -m "Initial academic website"
git branch -M main
git remote add origin https://github.com/YOURUSERNAME/YOURREPO.git
git push -u origin main
```

On GitHub: **Settings → Pages → Build and deployment → Deploy from a branch → main → /docs → Save**.

## 5. Replace the pictures

Put your real images in `images/`. For example:

- `images/headshot.jpg`
- `images/hunter.jpg`
- `images/research.jpg`

Then change the image path in `index.qmd`. Quarto accepts JPG, PNG, SVG, and WebP.

## 6. Add a paper

Copy one of the `::: {.paper}` blocks in `research.qmd`, change the title/authors/description, and add links. That's all you need to do.
