# NebulaWeb — GitHub Pages notes

This repository contains a simple static site. I've prepared the repository so you can publish it to GitHub Pages from the repository root or from the `docs/` folder. Below are two easy options and what I changed to make deployment smoother.

Options to publish

- Publish from repository root (recommended):
	1. Commit and push the repository to GitHub (if not already pushed).
	2. In your repository on GitHub, go to Settings → Pages.
	3. Under "Build and deployment / Source" choose branch `main` and folder `/ (root)`.
	4. Save — your site will be available at `https://<your-username>.github.io/<repo-name>/`.

- Publish from `docs/` folder:
	1. Move `index.html`, `main.css`, and `images/` into a `docs/` directory (or I can do this for you).
	2. In GitHub Settings → Pages choose branch `main` and folder `/docs`.

What I changed to help:
- Added `index.html` at the repository root that fetches `main.html` and injects it so the site works when visited at `/`.
- Added `.nojekyll` to ensure GitHub Pages serves static files as-is.
- Normalized image assets into `images/` and updated `main.html` to reference `images/nebulaweb2.jpeg` and `images/untitled-4.png`.
- Updated `main.html` with small accessibility and form improvements (aria labels and `name` attributes).

Quick checklist to publish from root (one-time):

1. Commit and push all changes:

```bash
git add -A
git commit -m "Prepare site for GitHub Pages: index, .nojekyll, images"
git push origin main
```

2. Go to GitHub → Settings → Pages and set the source to `main` / `root`.

3. Wait a minute and then open `https://<your-username>.github.io/<repo-name>/`.

Notes & follow-ups I can do for you

- Move all site files into `docs/` if you prefer that workflow.
- Add a simple GitHub Action to auto-deploy (not necessary for Pages from main/root).
- Wire the contact form to a webhook or serverless endpoint.

Tell me which publishing option you prefer and I'll finish the remaining steps (move files into `docs/` or add a deploy action). 
# NebulaWeb
# NebulaWeb
