# Isaac Mao Academic Homepage

This is a minimal Quarto website for a personal academic homepage. It is designed to be clean, maintainable, and suitable for deployment to GitHub Pages.

## Preview Locally

From this directory, run:

```bash
quarto preview
```

If your Quarto installation needs an explicit Python path, use:

```bash
QUARTO_PYTHON="$CONDA_PREFIX/bin/python" quarto preview
```

## Render

```bash
quarto render
```

The rendered site will be written to `_site/`.

## Publish With GitHub Pages

One simple deployment path is:

1. Create a GitHub repository.
2. Push this project to the repository.
3. In GitHub, go to **Settings > Pages**.
4. Set the source to **GitHub Actions**.
5. The included workflow at `.github/workflows/publish.yml` will render the Quarto site and publish `_site/`.

You can also publish manually with Quarto:

```bash
quarto publish gh-pages
```

## What To Edit

- Personal information, research, and publications: edit `index.qmd`, `_quarto.yml`, and `cv.qmd`.
- Pictures page: edit `pictures.qmd` and add image files under `images/pictures/`.
- Structured publication notes: edit `data/publications.yml` if you want to keep a separate data list.
- Notes: add folders under `posts/`, each with an `index.qmd`.
- CV PDF: replace `files/CV.pdf` with your real CV.
- Profile image: replace `images/profile-placeholder.jpg` with your own photo.
- Styling: edit `styles.css`.

## Suggested Workflow

1. Edit content in `.qmd` or `.yml` files.
2. Run `quarto preview` to inspect changes locally.
3. Run `quarto render` before committing.
4. Commit and push to GitHub.

Keep the site simple. Most updates should only require editing text files or replacing assets.
