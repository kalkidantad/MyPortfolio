# Academic portfolio (Hugo)

Hugo site for Kalkidan Tadesse’s academic portfolio. Deployed to GitHub Pages from this folder via GitHub Actions.

## Local development

```bash
# Hugo extended required (v0.148+ recommended)
hugo server -D
```

Site preview: `http://localhost:1313/MyPortfolio/` when `baseURL` includes the repo path. For a root-local preview:

```bash
hugo server -D --baseURL http://localhost:1313/ --appendPort=false
```

Or simply:

```bash
hugo server -D -b http://localhost:1313/
```

## Deploy (GitHub Pages)

You do **not** need to rename the repository to `username.github.io`.

| Repo name | Site URL |
|-----------|----------|
| `kalkidantad.github.io` | `https://kalkidantad.github.io/` (user site) |
| `MyPortfolio` (current) | `https://kalkidantad.github.io/MyPortfolio/` (project site) |

After pushing this branch / merging to `main`:

1. Repo **Settings → Pages**
2. Source: **GitHub Actions**
3. Run the **Deploy Hugo academic portfolio** workflow

Update `email` (and other fields) in `hugo.toml` before sharing publicly.
