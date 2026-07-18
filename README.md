# symworx/.github

Special organization repository for **[symworx](https://github.com/symworx)**.

GitHub uses this public repo for:

| Path | Purpose |
|------|---------|
| [`profile/README.md`](profile/README.md) | Organization profile shown on [github.com/symworx](https://github.com/symworx) |
| [`.github/`](.github/) | Default community health files, issue/PR templates for org repos that do not define their own |
| [`docs/`](docs/) | Source for the org GitHub Pages landing site |

## GitHub Pages

The site is deployed from `docs/` with [`.github/workflows/pages.yml`](.github/workflows/pages.yml).

**Cost:** Free for this public repository (GitHub Free includes Pages on public repos). Soft limits apply (e.g. ~1 GB site size, ~100 GB/month bandwidth). No paid plan is required for a public org landing page.

After the first push:

1. Repo **Settings → Pages → Build and deployment → Source**: **GitHub Actions**
2. Site URL: [https://symworx.github.io/.github/](https://symworx.github.io/.github/)

Optional: add a custom domain under **Settings → Pages**.

If you prefer **org profile only** and no site, you can delete `docs/` and `.github/workflows/pages.yml`; keep `profile/README.md` for the Overview intro.

## Local preview

```bash
# from repo root
python -m http.server 8080 --directory docs
# open http://localhost:8080
```

## What belongs here

- Org-wide defaults (code of conduct, contributing, security, support)
- Issue and pull request templates
- Org profile README
- Lightweight marketing / landing Pages

What does **not** belong here:

- Product source code (lives in [symworx/symworx](https://github.com/symworx/symworx))
- Per-repo licenses (must live in the product repository)
